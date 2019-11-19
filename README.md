# vrops-exporter
Prometheus exporter to scrape metrics from vRealize Operations Manager

## Running the exporter

The container is defaulting to /vrops-exporter path. Use vrops-exporter.py with one of the two ways of specifying the necessary credentials. They could also be mixed of course.

1. CLI

```
Usage: vrops-exporter.py [options]

Options:
  -h, --help            show this help message and exit
  -u USER, --user=USER  specify user to log in
  -p PASSWORD, --password=PASSWORD
                        specify password to log in
  -o PORT, --port=PORT  specify exporter port
  -d, --debug           enable debug
```

2. Enviroment variables

```
USER
PASSWORD
PORT
```

## Service discovery way of querying
Query with: ``http://localhost:1234/?target=yourDNSName``

