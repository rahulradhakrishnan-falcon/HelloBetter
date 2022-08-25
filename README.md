# HelloBetter


# Architecture:
![alt text](https://github.com/rahulradhakrishnan-falcon/HelloBetter/blob/main/HelloBetter.jpg?raw=true)

# Technology Used:

1. Open Telecom cloud - as primary cloud provider
2. Kubernetes - For hosting the microservices
3. Prometheus - For monitoring and observibility
4. Grafana - For Metrics Dashboards
5. Elasticsearch/Logstash/Beat - Centralised Log 
6. Slack/Mail/PagerDuty - Alert notification channels

# Application Flow:

The microservices are hosted in kubernetes and are served using ingress controller to the external customer.

We have a common relational database which is used for application and prometheus.

The metrics shipper in the pods will push the logs and metrics to prometheus and ELK .

Grafana dashboards give the detailed overview of the metrics.

Alert manager pushes the alerts to the respective channels .
