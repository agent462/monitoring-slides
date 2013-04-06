<!SLIDE transition=scrollUp>
# Collectd

## [The system statistics collection daemon]

<!SLIDE bullets>
* Written in C

* Over 90 plugins

* Get all your system metrics here

* Outputs to graphite

* Easy setup

* Each plugin can run at different intervals

<!SLIDE code small>
    @@@
    [bbrandau@ip-10-2-12-10 plugins]# cat memcached.conf
    LoadPlugin "memcached"

    <Plugin "memcached">
      Host  "127.0.0.1"
      Port  "11211"
    </Plugin>
