# subsquid-worker-dashboard
Subsquid Worker and Node Metrics Dashboard. A community-created dashboard for monitoring Subsquid nodes and workers, offering key performance metrics ideal for node operations.

# Dependencies
- Grafana
- Gauge 5.0.0
- Prometheus 1.0.0
- Prometheus Alertmanager 1.2.1
- Stat 5.0.0
- Table 5.0.0
- Time series 5.0.0

# Collector
- node-exporter (default port 9100) : Install node-exporter on the machine being monitored to collect hardware and OS metrics (Docker recommended). [https://github.com/prometheus/node_exporter](https://github.com/prometheus/node_exporter)
- subsquid-worker (default port 9090) : Metrics exported by default.

# Notes:

This initial version will undergo enhancements progressively, such as alerts, better metrics ...

If you're managing more than one worker/server, you can select the job at the top left.

NOTE: Altering the default port settings for the Subsquid Prometheus exporter may impact certain variables or transformations. This dashboard is configured with the assumption that the Subsquid exporter uses port 9090 and node-exporter uses port 9100. Panel customization may be necessary if you use non-standard port configurations.
