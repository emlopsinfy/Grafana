This repo is for Grafana integration with Evidently.

Grafana Repo : https://github.com/grafana/grafana

Grafana Download : https://grafana.com/grafana/download?platform=windows

Download ref : https://www.youtube.com/watch?v=QoDqxm7ybLc

Once downloaded and installed, go localhost:3000

username, password is admin by default.

##### Server Monitoring using Prometheus and Grafana

It can be done with one single UI.

Difference between monitoring techniques - logs and Metrics ?

##### Logs

Logs comes in various forms, applications will write their events and output to log files.

example, it also logs an ip address, url when someone sends a web request.

Logs are tracking events with specific details about the nature and type of it.

##### Metrics

Metrics are bit different, comes in different variations, one example is a counter so every time someone sends a new web request, we would increase a counter for that., calculate number of web requests after that.

It is something calculated.

##### We cannot do this manually for every server we are running!

So we need to have centralized server where we collecting and aggregating all these information, can be done with Prometheus.

##### Prometheus is and open source monitoring system that stores all these metrics in a giant database.

We can use it to scrape different systems and collect server or application metrics. 

##### How it works

https://www.youtube.com/watch?v=9TJx7QTrTyo&t=558s

Not followed after this.

https://www.youtube.com/watch?v=w-c3KYKQQfs&t=2648s

Started watching this video.

In DevOps now there are several phases such as continuous development continuous integration Continuous testing continuous deployment and continuous monitoring that constitute the DevOps life cycle this is where the birth of Grafana really happened.

So Grafana for continuous monitoring.

Monitoring tool that will help you visualize your real-time data in an application.

##### Why continuous monitoring ?

network visibility and transparency

clarity on state of IT Infra by automatically collecting and analysing data to reflect possible outages.

implementing an alert system.

minimizes downtime.

##### What is Grafana ?

Grafana is a visualization DevOps Tool. 

Grafana is a multi-platform open source analytics and interactive visualization web application it basically provides charts graphs and alerts for the web when connected to supported data sources Grafana is expandable through a plugin system it allows you to query visualize alert on and understand your metrics matter where they are stored create explore and share dashboards with your team and foster a data driven culture also Grafana has become the world's most popular technology.

Features - Visualize, Alert, Unify, Open Source, Extend, Collaborate.

##### Demo

go localhost 3000.

just creating new dashboard, adding panels to it.

you have lot of options, like kind of visualization.

Also has Query option, where it writes query to get data from Data Source like Prometheus.

##### Data Source

##### Time Series Databases

Prometheus, Graphite, OpenTSDB, InfluxDB - All are open source.

##### Logging & document databases

Loki - Like Prometheus but for logs. OSS logging solution from Grafana Labs.

Elasticsearch - Open source logging & analytics database.

##### Distributed tracing

Jaeger - Open source, end-to-end distributed tracing.

Zipkin - Placeholder for the distributed tracing system.

Tempo - High volume, minimal dependency trace storage. OSS tracking solution from Grafana labs.

##### SQL

MySQL - Data source for MySQL databases.

PostgreSQL - Data source for PostgreSQL and compatible databases.

Microsoft SQL Server - Data source for Microsoft SQL Server compatible databases.

##### Cloud

Google Cloud Monitoring - Data source for Google’s monitoring service (formerly named Stackdriver)

CloudWatch - Data source for Amazon AWS monitoring service.

Azure Monitor - Data source for Microsoft Azure Monitor & Application Insights.

Grafana Cloud - Hosted Graphite, Prometheus, and Loki.

##### Enterprise plugins

Wavefront - Wavefront integration and data source.

Splunk Infrastructure Monitoring - SignalFx integration and datasource.

Splunk - Visualize and explore Splunk logs.

Snowflake - Snowflake integration and data source.

ServiceNow - ServiceNow integration and data source.

Salesforce - Salesforce integration and datasource.

SAP HANA - SAP HANA integration and data source.

Oracle - Visualize and explore Oracle SQL

New Relic - New Relic integration and data source

MongoDB - MongoDB integration and data source.

Jira - Jira integration and datasource

Honeycomb - Honeycomb integration and datasource

GitLab - GitLab integration and datasource

Dynatrace - Visualize and explore Dynatrace data

DataDog - DataDog integration and data source

AppDynamics - AppDynamics integration and data source

##### Others

TestData DB - Generates test data in different forms



##### Demo

##### What are we going to do ?

so firstly we'll be creating a world map which will show us the confirmed cases of covid 19 over the past one year so all the panels that we've really created here is the data of the past one year itself.

So we need a data source first, we will be using influxDB.

https://docs.influxdata.com/influxdb/v2.0/install/?t=Windows

followed and installed, admin is username and password is adminadmin.

we can open cmd in C:\Program Files\InfluxData\influxdb

type influx

influx commands not working on windows... :( :(

if everything is perfect, we can add this influx db in Grafana data source.





