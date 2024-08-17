# Final_Assignment_1
Prometheus Monitoring and Alerting for Multiple EC2 Instances in Multiple Accounts with Slack Integration
# Prometheus Monitoring Setup

This repository contains all the necessary files to set up Prometheus monitoring for EC2 instances and send alerts to Slack.

## Files
- `prometheus.yml`: Prometheus server configuration
- `alert_rules.yml`: Alerting rules for Prometheus
- `alertmanager.yml`: Configuration for Alertmanager to send notifications to Slack
- `prometheus.service`: Systemd service file for Prometheus
- `node_exporter.service`: Systemd service file for Node Exporter
- `deploy.sh`: Script to deploy Prometheus and Node Exporter

## Setup Instructions
1. Clone this repository to your Prometheus server.
2. Run `deploy.sh` to install Prometheus and Node Exporter.
3. Modify the `prometheus.yml` file to include your AWS credentials and EC2 region.
4. Modify the `alertmanager.yml` file to include your Slack webhook URL.
5. Start the Prometheus and Node Exporter services using systemd.
6. Test the setup by simulating a server failure
