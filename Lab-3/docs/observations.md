# Lab 3 Observations

## Monitoring Stack

Prometheus, Node Exporter, and Grafana were deployed using Docker Compose.

### Prometheus
- Prometheus was exposed on port 9090.
- Node Exporter was exposed on port 9100.
- Prometheus successfully discovered and scraped both Prometheus and Node Exporter targets.
- Both targets were shown as UP in the Prometheus Target Health page.
- Prometheus queries successfully returned CPU, memory, filesystem, and network metrics.

### Grafana
- Grafana was exposed on port 3000.
- Prometheus was configured as the Grafana data source.
- A dashboard named `Lab 3 Monitoring Dashboard` was created.
- The dashboard contains panels for:
  - Network Receive Traffic
  - Memory Usage (%)
  - CPU Usage (%)
- The dashboard JSON was exported and stored in `Lab-3/grafana/dashboard.json`.

### Verification
The monitoring stack was verified using Docker Compose, Docker container status, Prometheus API queries, Prometheus Target Health, and Grafana dashboard visualizations.
