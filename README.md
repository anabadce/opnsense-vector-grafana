# Vector - Loki - Grafana stack for OPNsense logs

Vector - Loki - Grafana stack running in Docker to process OPNsense logs

OPNsense, using its builtin `syslog`, needs to be configured to remote send logs over the network to this stack. 

## Stack components

- *Vector* acts as the high-performance collector and transformer, equivalent to agents like Promtail or Fluent Bit or Logstash to gather, parse, and route logs.
- *Loki* serves as the log aggregation and storage engine (database), equivalent to Elasticsearch, to index, server searches.
- *Grafana* provides the user interface for exploring querying the database.
