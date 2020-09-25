# cp-jmx-dynatrace
The Dynatrace-Confluent plugin is based on the JMX plugin and allows the 
Dynatrace OneAgent to collect JMX metrics from Confluent Components.
By default, Dynatrace OneAgent identifies Kafka installation on pull the broker metrics. This metrics are available under “Settings->Monitoring->Monitored technologies-> Kafka JMX’. The Kafka Brokers dashboard is created with these metrics, and for the rest of the cp components metrics below setup is needed.

Note: Dynatrace Agent does not pull metrics with text value. So, I have used Synthetic HTTP   monitoring to check Connector Statuses.

## Installation

1.	Copy Script/ConnectorAPI to Dynatrace server. Refer to the below link for instructions

https://www.dynatrace.com/support/help/how-to-use-dynatrace/synthetic-monitoring/browser-monitors/script-mode-for-browser-monitor-configuration/?script-parameters%3C-%3Escript-model=script-parameters


2.	Upload JMX extension from assets folder, Refer to the below link for instructions

https://www.dynatrace.com/support/help/extend-dynatrace/extensions/jmx-extensions/jmx-extensions/#upload-a-jmx-extension

3.	Post dashboard json to Dynatrace server. Refer to the below link for instructions
https://www.dynatrace.com/support/help/dynatrace-api/configuration-api/dashboards-api/post-dashboard/

If the above steps are successful, you can see dash boards added to Dynatrace server.

## Dashboards
![Dash boards](/images/Dashboards.png)

## Connector Dashboard

![Connectors Monitoring Dashboard](/images/Connectors.png)

![Connectors Monitoring Dashboard](/images/Connectors-1.png)


## Schema Registry

![Schema Registry Monitoring Dashboard](/images/SR.png)


## Kafka Rest Proxy

![Kafka Resct Proxy Monitoring Dashboard](/images/KafkaRest.png)


## KSQL DB

![KSQL DB Monitoring Dashboard](/images/KsqlDB.png)
