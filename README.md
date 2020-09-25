# Monitoring
Dynatrace-Confluent Platform-JMX
The Dynatrace-Confluent plugin is based on the JMX plugin and allows the 
Dynatrace OneAgent to collect JMX metrics from Confluent Components.

Note: Dynatrace Agent does not pull metrics with text value. So, I have used Synthetic HTTP   monitoring to check Connector status.

1.	Copy Script/ConnectorAPI to Dynatrace server. Refer to the below link for instructions

    https://www.dynatrace.com/support/help/how-to-use-dynatrace/synthetic-monitoring/browser-monitors/script-mode-for-browser-monitor-configuration/?script-parameters%3C-%3Escript-model=script-parameters


2.	Upload JMX extension from assets folder, Refer to the below link for instructions

    https://www.dynatrace.com/support/help/extend-dynatrace/extensions/jmx-extensions/jmx-extensions/#upload-a-jmx-extension

3.	Post dashboard json to Dynatrace server. Refer to the below link for instructions
    https://www.dynatrace.com/support/help/dynatrace-api/configuration-api/dashboards-api/post-dashboard/
