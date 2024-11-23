# Prometheus Monitoring

Prometheus is an open-source systems monitoring and alerting toolkit designed for reliability and scalability. This setup includes Prometheus, Node Exporter, and Grafana for monitoring system resources.

---

## 📦 Setup Instructions

### Prerequisites
- Docker and Docker Compose installed on your system.
- Basic knowledge of Docker and networking.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/prometheus-monitoring.git
   cd prometheus-monitoring

2. Start the services using Docker Compose:
   docker-compose up -d
3. Access Prometheus at:
   http://<YOUR_SERVER_IP>:3000
4. Add Grafana (if included) and access it at:
   http://<YOUR_SERVER_IP>:3000


🛠 Configuration
Prometheus Configuration File
Prometheus uses prometheus.yml for its configuration. Below is an example of the scrape configuration for Node Exporter:

global:
  scrape_interval: 15s

scrape_configs:
  - job_name: 'node_exporter'
    static_configs:
      - targets: ['node-exporter:9100']

📊 Monitoring Metrics
Example Queries
Here are some useful Prometheus queries to monitor system performance:

Node Exporter Health

🖥 Grafana Dashboard
Import the JSON configuration file for a pre-built Grafana dashboard from the grafana/ directory.
Connect Grafana to Prometheus by adding a new data source:
Type: Prometheus
URL: http://prometheus:9090

🤝 Contribution
Feel free to fork this repository, create issues, or submit pull requests to improve the setup.

📄 License
This project is licensed under the MIT License.

