<!SLIDE bullets transition=scrollUp>
# Handler

* Takes action on event data.

* Several types: execute a script, open a socket ...

## [Pipe, TCP, UDP, AMQP, Set]

<!SLIDE code medium transition=scrollUp>
    @@@
    {
      "handlers": {
        "awsdecommission": {
          "type": "pipe",
          "command": "/etc/sensu/handlers/awsdecomm.rb",
          "severities": [
            "ok",
            "warning",
            "critical"
          ]
        }
      }
    }

<!SLIDE small center transition=scrollUp>
# The good

* Keepalives

* Compatible with nagios plugins

* It can utilize bash, ruby, python, etc (anything)

* Deep merging of configuration files

* Groups/Sets

* Aggregates

* Community Plugins
