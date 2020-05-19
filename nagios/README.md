# Nagios

### Documentation
- Website [https://www.nagios.org/]
- Unofficial Github [https://github.com/JasonRivers/Docker-Nagios]

### How to Run

### Install

```sh
docker pull jasonrivers/nagios:latest
```

### Running

Run with the example configuration with the following:

```sh
docker run --name nagios4 -p 0.0.0.0:8080:80 jasonrivers/nagios:latest
```

alternatively you can use external Nagios configuration & log data with the following:

```sh
docker run --name nagios4  \
  -v /path-to-nagios/etc/:/opt/nagios/etc/ \
  -v /path-to-nagios/var:/opt/nagios/var/ \
  -v /path-to-custom-plugins:/opt/Custom-Nagios-Plugins \
  -v /path-to-nagiosgraph-var:/opt/nagiosgraph/var \
  -v /path-to-nagiosgraph-etc:/opt/nagiosgraph/etc \
  -p 0.0.0.0:8080:80 jasonrivers/nagios:latest
```


### How to Access
#### Credentials

The default credentials for the web interface is `nagiosadmin` / `nagios`
- http://localhost:80

