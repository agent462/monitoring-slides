<!SLIDE small transition=scrollUp>
# How to log effectively
* Time Formats
  * Time formats ISO 8601
  * Time at the beginning of the line
  * YYYY-MM-DDThh:mm:ss.fffz where fff represents milliseconds
* Unique Identifiers
  * Correlate to user
  * Include non PII user data

<!SLIDE small transition=scrollUp>
* Categorization
  * Multiple levels (INFO, WARN, etc)
  * Assign priority (P1, P2, etc)

* Profiling Data
  * Record Timings for Model, View, Controller processing times.
  * Record Timings for external dependency calls (API, etc)
  * Is host1 processing X in the same amount of time as host2
  * Has the render for X increased after this deployment

<!SLIDE smaller code transition=scrollUp>
# Log Structure
      @@@
      time=2012-03-05T16:45:01:999Z ip=192.168.1.1, username=bryan.brandau, \
      level=info, priority=p3, view="profile parser", \
      message="The programmer did something bad"


