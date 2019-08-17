## Site Developer Guide {docsify-ignore}

This guide is for site developers - either consultants or in-house developers responsible for site modification.

## Annotations

### User Annotations

[User Annotations](guides/site-user/?id=annotations) were introduced in the [User Guide](guides/site-user/)
as a way for users to manage personal annotations.

These notes are entered directly onto dashboard panels, and can be edited and deleted
by users. It's a simple mechanism for noting anomalies found on charts.

### System Annotations

System annotations differ from user annotations in that the system generates them, and users
generally don't have the ability to add, edit, or delete them.

The IoT Edge server comes with two ways of creating system annotations

* **Stored annotations** - Site developers can send event logs into the Node-Red logging node
when system events are detected. These logs have date/time stamps and can contain tags for
associating events with places, devices, products, etc.

* **Data sourced annotations** - Site developers can expose custom annotations in
[custom data sources](guides/site-developer/?id=custom-data-sources) when event data is stored
outside of these common annotation databases.

## Custom Data Sources

Site **metrics** are stored in the [Graphite](https://graphiteapp.org/) time-series database,
and site **events** are stored in the [Loki](https://grafana.com/loki) logging database.
Both of these databases have built-in exposure to Grafana dashboards.

When data is stored outside of these standard databases, a custom
[Grafana Data Source](https://grafana.com/docs/features/datasources/)
can be built to expose that data to the Grafana UI.

The IoT Edge server simplifies the process of getting custom data into dashboards
with a built-in data source called **Edge API**. This lets site developers build
Node-Red nodes to serve dashboard data without the complexity of writing a Grafana data source.
