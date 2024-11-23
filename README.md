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
   git clone https://github.com/ashkanramedani/prometheus.git
   cd prometheus
   
2. Start the services using Docker Compose:
   ```bash
   docker-compose up -d
   Access Prometheus at:

3. arduino
   ```bash
   http://<YOUR_SERVER_IP>:9090
   Add Grafana (if included) and access it at:

4. arduino
   ```bash
   http://<YOUR_SERVER_IP>:3000
