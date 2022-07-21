# Awesome OpenTelemetry 🎉
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A carefully curated list of open source content related to OpenTelemetry. 

<img width="686" alt="OTel_full" src="https://user-images.githubusercontent.com/52788043/179937064-9e3a201a-0a04-41c4-9079-0d64c9f39e8e.png">


## What is OpenTelemetry?

**OpenTelemetry** or OTel is an open-source project, which allows you to collect, export, and generate *traces*, *logs*, and, *metrics* (also known as the three pillars of observability). It is a set of APIs and SDKs.

> “When we announced the OpenTelemetry project in 2019, we envisioned it as the next major version of both OpenTracing and OpenCensus,” said Ben Sigelman, one of the co-creators of both OpenTracing and OpenTelemetry. 


## Contents
- [Awesome OpenTelemetry 🎉](#awesome-opentelemetry-)
  - [What is OpenTelemetry?](#what-is-opentelemetry)
  - [Contents](#contents)
  - [OpenTelemetry Instrumentation 🎺](#opentelemetry-instrumentation-)
    - [Supported Languages](#supported-languages)
    - [Supported Databases](#supported-databases)
    - [OpenTelemetry Registry](#opentelemetry-registry)
    - [Secure your POD](#secure-your-pod)
  - [Distributed Tracing Solutions](#distributed-tracing-solutions)
    - [Open Source Tools](#open-source-tools)
    - [Opentelemetry Vendors](#opentelemetry-vendors)
  - [Terminology](#terminology)
  - [Statistics](#statistics)
  - [Current Status](#current-status)
  - [Main Components](#main-components)
  - [Tools](#tools)
  - [Books 📚](#books-)
    - [Case Studies](#case-studies)
  - [Blog By Vendors:](#blog-by-vendors)
  - [Video Tutorials](#video-tutorials)
    - [OpenTelemetry C++](#opentelemetry-c)
    - [OpenTelemetry .NET](#opentelemetry-net)
    - [OpenTelemetry Erlang/Elixir](#opentelemetry-erlangelixir)
    - [OpenTelemetry Go](#opentelemetry-go)
    - [OpenTelemetry Java](#opentelemetry-java)
    - [OpenTelemetry JavaScript](#opentelemetry-javascript)
      - [By SigNoz:](#by-signoz)
      - [Others:](#others)
    - [OpenTelemetry PHP](#opentelemetry-php)
    - [OpenTelemetry Python](#opentelemetry-python)
      - [By SigNoz:](#by-signoz-1)
      - [Others:](#others-1)
    - [OpenTelemetry Ruby](#opentelemetry-ruby)
    - [OpenTelemetry Rust](#opentelemetry-rust)
    - [OpenTelemetry Swift](#opentelemetry-swift)
  - [Join the Community](#join-the-community)
    - [Newsletters 📰](#newsletters-)
    - [Podcasts](#podcasts)
    - [Events](#events)
    - [StackOverflow](#stackoverflow)
    - [Twitter](#twitter)
    - [Slack](#slack)
 

Here starts the list of awesome resources! Enjoy. 

---

## OpenTelemetry Instrumentation 🎺

### Supported Languages 
| Language                                                                        | Client Repo                                                              | Contrib Repo                                                               | API and SDK                                                           | Auto Instrumentation                                                                                   |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------ | -------------------------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| [C++](https://opentelemetry.io/docs/instrumentation/cpp/)                       | [Client ](https://github.com/open-telemetry/opentelemetry-cpp)           | [Contrib](https://github.com/open-telemetry/opentelemetry-cpp-contrib)     |
| [.NET](https://opentelemetry.io/docs/instrumentation/net/automatic/)            | [Client ](https://github.com/open-telemetry/opentelemetry-dotnet)        | [Contrib ](https://github.com/open-telemetry/opentelemetry-dotnet-contrib) |                                                                       | [Auto Instrumentation Support](https://github.com/open-telemetry/opentelemetry-dotnet-instrumentation) |
| [Erlang/Elixir](https://opentelemetry.io/docs/instrumentation/erlang/)          |                                                                          | [Contrib](https://github.com/open-telemetry/opentelemetry-erlang-contrib)  | [SDK](https://github.com/open-telemetry/opentelemetry-erlang)         |                                                                                                        |
| [Go](https://opentelemetry.io/docs/instrumentation/go/getting-started/)         |                                                                          | [Contrib ](https://github.com/open-telemetry/opentelemetry-go-contrib)     | [API and SDK](https://github.com/open-telemetry/opentelemetry-go)     |
| [Java](https://opentelemetry.io/docs/instrumentation/java/automatic/)           |                                                                          | [ Contrib](https://github.com/open-telemetry/opentelemetry-java-contrib)   | [SDK](https://github.com/open-telemetry/opentelemetry-java)           | [Auto Instrumentation Support](https://github.com/open-telemetry/opentelemetry-java-instrumentation)   |
| [JavaScript](https://opentelemetry.io/docs/instrumentation/js/instrumentation/) | [Client ](https://github.com/open-telemetry/opentelemetry-js)            | [Contrib ](https://github.com/open-telemetry/opentelemetry-js-contrib)     | [API](https://github.com/open-telemetry/opentelemetry-js-api)         | Auto Instrumentation Support                                                                           |
| [PHP](https://opentelemetry.io/docs/instrumentation/php/getting_started/)       | [monorepo](https://github.com/open-telemetry/opentelemetry-php)          | [Contrib](https://github.com/open-telemetry/opentelemetry-php-contrib)     |                                                                       |
| [Python](https://opentelemetry.io/docs/instrumentation/python/getting-started/) |                                                                          | [Contrib ](https://github.com/open-telemetry/opentelemetry-python-contrib) | [API and SDK](https://github.com/open-telemetry/opentelemetry-python) | Auto Instrumentation Support                                                                           |
| [Ruby](https://opentelemetry.io/docs/instrumentation/ruby/automatic/)           | [Contrib ](https://github.com/open-telemetry/opentelemetry-ruby-contrib) |                                                                            | [API and SDK](https://github.com/open-telemetry/opentelemetry-ruby)   | Auto Instrumentation Support                                                                           |
| [Rust](https://opentelemetry.io/docs/instrumentation/rust/)                     | [Github]()                                                               |                                                                            | [API and SDK](https://github.com/open-telemetry/opentelemetry-rust)   |
| [Swift](https://opentelemetry.io/docs/instrumentation/swift/)                   | [Github]()                                                               |                                                                            | [API](https://github.com/open-telemetry/opentelemetry-swift)          |


**[`^ back to top ^`](#contents)**

### Supported Databases 

| Value        | Description                        |     | Value           | Description               |
| ------------ | ---------------------------------- | --- | --------------- | ------------------------- |
| `other_sql`  | Some other SQL database            |     | `mariadb`       | MariaDB                   |
| `mssql`      | Microsoft SQL Server               |     | `netezza`       | Netezza                   |
| `mysql`      | MySQL                              |     | `pervasive`     | Pervasive PSQL            |
| `oracle`     | Oracle Database                    |     | `pointbase`     | PointBase                 |
| `db2`        | IBM Db2                            |     | `sqlite`        | SQLite                    |
| `postgresql` | PostgreSQL                         |     | `sybase`        | Sybase                    |
| `redshift`   | Amazon Redshift                    |     | `teradata`      | Teradata                  |
| `hive`       | Apache Hive                        |     | `vertica`       | Vertica                   |
| `cloudscape` | Cloudscape                         |     | `h2`            | H2                        |
| `hsqldb`     | HyperSQL DataBase                  |     | `coldfusion`    | ColdFusion IMQ            |
| `progress`   | Progress Database                  |     | `cassandra`     | Apache Cassandra          |
| `maxdb`      | SAP MaxDB                          |     | `hbase`         | Apache HBase              |
| `hanadb`     | SAP HANA                           |     | `mongodb`       | MongoDB                   |
| `ingres`     | Ingres                             |     | `redis`         | Redis                     |
| `firstsql`   | FirstSQL                           |     | `couchbase`     | Couchbase                 |
| `edb`        | EnterpriseDB                       |     | `couchdb`       | CouchDB                   |
| `cache`      | InterSystems Caché                 |     | `cosmosdb`      | Microsoft Azure Cosmos DB |
| `adabas`     | Adabas (Adaptable Database System) |     | `dynamodb`      | Amazon DynamoDB           |
| `firebird`   | Firebird                           |     | `neo4j`         | Neo4j                     |
| `derby`      | Apache Derby                       |     | `geode`         | Apache Geode              |
| `filemaker`  | FileMaker                          |     | `elasticsearch` | Elasticsearch             |
| `informix`   | Informix                           |     | `memcached`     | Memcached                 |
| `instantdb`  | InstantDB                          |     | `cockroachdb`   | CockroachDB               |
| `interbase`  | InterBase                          |     |



Check full list [here.](https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/trace/semantic_conventions/database.md)


**[`^ back to top ^`](#contents)**

---

If you are using Kubernetes, you can use the [OpenTelemetry Operator for Kubernetes](https://github.com/open-telemetry/opentelemetry-operator) to [inject auto-instrumentation libraries](https://github.com/open-telemetry/opentelemetry-operator#opentelemetry-auto-instrumentation-injection) for Java, Node.js and Python into your application.



### OpenTelemetry Registry 
The [OpenTelemetry Registry](https://opentelemetry.io/registry/) allows you to search for instrumentation libraries, tracer implementations, utilities, and other useful projects in the OpenTelemetry ecosystem.


### Secure your POD 
- [Secure OpenTelemetry Collector - Medium](https://medium.com/opentelemetry/securing-your-opentelemetry-collector-1a4f9fa5bd6f)

- [ConfigAuth](https://github.com/open-telemetry/opentelemetry-collector/tree/main/config/configauth)

- [PromQL Cheat SHeet](https://promlabs.com/promql-cheat-sheet/)


**[`^ back to top ^`](#contents)**

---

## Distributed Tracing Solutions

### Open Source Tools 

- [SigNoz](https://signoz.io/) | [Github]()
- [OpenTelemetry](https://opentelemetry.io) | [Github]()
- [OpenTracing](https://opentracing.io) - *Deprecated* | [Github]()
- [OpenCensus](https://opencensus.io) - *Deprecated* | [Github](https://github.com/census-instrumentation)
- [Jaeger](https://www.jaegertracing.io) | [Github]()
- [Zipkin](https://zipkin.io) | [Github]()
- [Grafana](https://grafana.com/docs/agent/latest/) | [Github](https://github.com/grafana/) 
- [Loki](https://github.com/grafana/loki) - Like Prometheus, but for logs.
- [Tempo](https://github.com/grafana/tempo) - Grafana Tempo is a high volume, minimal dependency distributed tracing backend.
- [mimir](https://github.com/grafana/mimir) - the most scalable Prometheus backend.


### Opentelemetry Vendors 
Distributions and vendors who natively support OpenTelemetry in their commercial products.
- [SigNoz - Open Source APM ![](https://camo.githubusercontent.com/8354ae23fed92d21e4c27db64b4dfb654a1dffb56d20b2642ffc1db1135381e7/68747470733a2f2f63646e2e7261776769742e636f6d2f417765736f6d652d57696e646f77732f417765736f6d652f6d61737465722f6d656469612f4f53532e737667)](https://signoz.io) - Understand issues in your deployed applications & solve them quickly ⚡️.
- [AppDynamics](https://www.appdynamics.com) - Observe what matters.
- [Aspecto](https://www.aspecto.io/) - Troubleshoot performance bottlenecks and errors within your microservices.
- [AWS](https://aws-otel.github.io/) - A secure, production-ready, AWS-supported distribution of the OpenTelemetry project.
- [Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/app/opentelemetry-overview)
- [Datadog](https://docs.datadoghq.com/tracing/setup_overview/open_standards) - Modern monitoring & security.
- [Dynatrace](https://www.dynatrace.com/support/help/how-to-use-dynatrace/transactions-and-services/service-monitoring-settings/opentelemetry/) - Digitally transform faster, smarter, and easier.
- [Elastic](https://www.elastic.co/guide/en/apm/get-started/current/open-telemetry-elastic.html) - Search. Solve. Succeed.
- [F5](https://github.com/open-telemetry/opentelemetry-collector-contrib/tree/main/exporter/f5cloudexporter)
- [Grafana Labs](https://grafana.com/oss/opentelemetry/) - Operational dashboards for your data here, there, or anywhere.
- [Honeycomb](https://docs.honeycomb.io/getting-data-in/) - Find your most perplexing application issues.
- [Instana](https://www.ibm.com/docs/en/instana-observability) - Designed to help IT operations, development, and DevOps teams operate more efficiently.
- [Lightstep](https://github.com/lightstep?q=launcher) - Monitoring, observability, and incident response for the world’s most reliable systems.
- [LogicMonitor](https://www.logicmonitor.com/support/tracing/getting-started-with-tracing) - Unified observability to transform what’s next.
- [Logz.io](https://docs.logz.io/shipping/tracing-sources/opentelemetry.html#overview) - End-to-end cloud monitoring built for scale.
- [Lumingo](https://docs.lumigo.io/docs/opentelemetry) - Monitoring and Debugging for Modern Cloud Applications.
- [New Relic](https://newrelic.com/solutions/opentelemetry) - Instrument once, analyze everything in one place.
- [Promscale](https://www.timescale.com/promscale/) - Observability powered by SQL.
- [Sentry Software](https://www.sentrysoftware.com/products/hardware-sentry-opentelemetry-collector.html) - Monitor the processors, disks, controllers, network adapters, temperature sensors, etc.
- [Splunk](https://www.splunk.com/en_us/blog/conf-splunklive/announcing-native-opentelemetry-support-in-splunk-apm.html) - The Unified Security and Observability Platform.
- [Sumo Logic](https://help.sumologic.com/Traces/Getting_Started_with_Transaction_Tracing) - Making the world’s apps reliable and secure. Cloud-native SaaS analytics.
- [Uptrace](https://uptrace.dev/) - All-in-one tool to optimize performance and monitor errors & logs.

[Click here for full list of vendors that supports OpenTelemetry.](https://opentelemetry.io/vendors/)



## Terminology 
- [Components](https://www.jaegertracing.io/docs/1.30/architecture/#terminology)
- [Glossary](https://opentelemetry.io/docs/concepts/glossary/)

## Statistics 
- [DevStats - Opentelemetry](https://opentelemetry.devstats.cncf.io/d/8/dashboards?orgId=1&refresh=15m)
- [Google Trends](https://trends.google.com/trends/explore?date=today%205-y&q=opentelemetry)


##  Current Status 

| Name        | API                    | SDK    | Protocol |
| ----------- | ---------------------- | ------ | -------- |
| **Tracing** | Stable, feature-freeze | Stable | Stable   |
| **Metrics** | Stable                 | Mixed  | Stable   |
| **Baggage** | Stable, feature-freeze | Stable | N/A      |
| **Logging** | Draft                  | Draft  | Stable   |

[Latest here.](https://opentelemetry.io/status/)



## Main Components 

- **OpenTelemetry Protocol (OTLP)** specification describes the encoding, transport, and delivery mechanism of telemetry data between telemetry sources, intermediate nodes such as collectors, and telemetry backends.
- **OpenTelemetry Collector** offers a vendor-agnostic implementation on receiving, processing, and exporting telemetry data and removing the need to run, operate, and maintain multiple agents/collectors.
- **APIs and SDKs** in 11 different languages, enabling users to easily integrate and extend the project.


**[`^ back to top ^`](#contents)**

---


## Tools 
- [BindPlane OP](https://github.com/observIQ/bindplane-op) - open source observability pipeline that gives you the ability to collect, refine, and ship metrics, logs, and traces to any destination.
- [Trace Test](https://github.com/kubeshop/tracetest) - End-to-end Tests Powered by  Your OpenTelemetry Traces.
- [Vector](https://github.com/vectordotdev/vector) - A lightweight, ultra-fast tool for building observability pipelines by Datadog. 

## Books 📚

- [Observability Engineering](https://www.oreilly.com/library/view/observability-engineering/9781492076438/)
- [Mastering Distributed Tracing](https://www.oreilly.com/library/view/mastering-distributed-tracing/9781788628464/)
- [Distributed Tracing in Practice](https://www.oreilly.com/library/view/distributed-tracing-in/9781492056621/)
- [Distributed Systems Observability](https://www.oreilly.com/library/view/distributed-systems-observability/9781492033431/)
- [The Future of Observability with OpenTelemetry](https://www.oreilly.com/library/view/the-future-of/9781098118433/)
- [Distributed Tracing with Jaeger, Kubernetes, and Istio](https://www.manning.com/liveprojectseries/distributed-tracing-ser)
- [Cloud-Native Observability with OpenTelemetry](https://www.oreilly.com/library/view/cloud-native-observability-with/9781801077705/)
- [Go for DevOps - Chapter #9](https://www.oreilly.com/library/view/go-for-devops/9781801818896/)
- [🔍 Search OpenTelemetry at O'Reilly](https://www.oreilly.com/search/?query=OpenTelemetry&formats=book)



### Case Studies 
- [CNCF](https://www.cncf.io/case-studies/)
- [How Lightstep Implemented Observability](https://www.oreilly.com/videos/how-lightstep-implemented/0636920623601/)



**[`^ back to top ^`](#contents)**


## Blog By Vendors:

- [SigNoz](https://signoz.io/opentelemetry/) - Instrumentation Blogs.
- [New Relic](https://developer.newrelic.com/opentelemetry-masterclass/) - OpenTelemetry Masterclass from New Relic.
- [Honeycomb](https://www.honeycomb.io/blog/) - Blog posts about observability, monitoring, OpenTelemetry.
- [Aspecto](https://www.aspecto.io/blog/) - Guides on how to use OpenTelemetry.
- [Aspecto Medium](https://medium.com/aspecto)
- [Jaeger](https://medium.com/jaegertracing/latest) - Posts from Jaeger.
- [Dev.to](https://dev.to/search?q=OpenTelemetry) - Posts about OpenTelemetry.
- [Lightstep](https://lightstep.com/blog) - Blog posts and latest updates of OpenTelemetry.



## Video Tutorials
- [Opentelemetry Offical YouTube](https://www.youtube.com/channel/UCHZDBZTIfdy94xMjMKz-_MA/playlists)
- [CNCF OTel Community Day 2022 Playlist](https://www.youtube.com/playlist?list=PLj6h78yzYM2P6ia87Y6mOd38Chd2E1Exo)
- [OpenTelemetry Instrumentation with SigNoz Playlist](https://www.youtube.com/playlist?list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP)
- [The OpenTelemetry Bootcamp](https://www.aspecto.io/opentelemetry-bootcamp/) | [Github](https://github.com/aspecto-io/opentelemetry-bootcamp)
- [freeCodeCamp OpenTelemetry Course](https://www.youtube.com/watch?v=r8UvWSX3KA8)
- [Udemy - Microservices Observability, Resilience, Monitoring on .Net](https://www.udemy.com/course/microservices-observability-resilience-monitoring-on-net/)
- [OpenTelemetry Tutorial .NET](https://www.youtube.com/playlist?list=PLdvI3YlPDGgdFG2mlXOy403V0J3MhRHeE)
- [LightStep Opentelemetry Playlist 30 Videos](https://www.youtube.com/playlist?list=PLv9DlQuUaXQc7PWxyGuJJnHE856zJYpse)


### OpenTelemetry C++
- [Opentelemetry C/C++ SIG Playlist](https://www.youtube.com/playlist?list=PLVYDBkQ1TdyyldLnfc3kHRVYaj1AomFNy)
- [OpenTelemetry 2019-10-21 C++ SIG meeting](https://www.youtube.com/watch?v=5TVtrpMEj1E)


### OpenTelemetry .NET
- [OpenTelemetry .NET SIG Playlist](https://www.youtube.com/playlist?list=PLVYDBkQ1TdyyWZv3XVKuAFm5-FL1z2b3q)
- [.NET - Monitor a .NET Application with OpenTelemetry and SigNoz](https://www.youtube.com/watchv=9SwL5kMDcvY)
- [OpenTelemetry with Minimal APIs in .NET 6](https://www.youtube.com/watch?v=djLCqEzf72o)
- [Get Started With OpenTelemetry Tracing and ASP.NET Core](https://www.youtube.com/watch?v=g0G9M6AuTdo)
- [Using OpenTelemetry for distributed tracing in microservices Implemented in ASP.NET 6 and C# 10](https://www.youtube.com/watch?v=vas3TjFUkds)
- [OpenTelemetry in .NET Explained](https://www.youtube.com/watch?v=LPh1YzIc39U)
- [Better Observability with Open Telemetry in .NET](https://www.youtube.com/watch?v=Sb3p4AHytG8)
- [Distributed Tracing Made Easy with .NET 5, with Jimmy Bogard](https://www.youtube.com/watch?v=N0r5NSY3ZIQ)
- [Metrics in .NET has never been easier - OpenTelemetry](https://www.youtube.com/watch?v=Gx8zNOcQSm8)
  

### OpenTelemetry Erlang/Elixir
- [Elixir - Monitor your Elixir Application with OpenTelemetry and SigNoz](https://www.youtube.com/watch?v=wLMrV-LtHFU)
- [Monitoring Elixir With OpenTelemetry | Kamil Kowalski | ElixirConf EU 2021](https://www.youtube.com/watch?v=4OBtc_eIKIE)
  

### OpenTelemetry Go
- [OpenTelemetry Go SIG Playlist](https://www.youtube.com/playlist?list=PLVYDBkQ1Tdyw1JXfQkL7erhN4CpKNssV-)
- [Go instrumentation - OpenTelemetry in Go applications : Complete Tutorial with SigNoz](https://www.youtube.com/watch?v=kTHW4VYnISQ&t=3s)
- [OpenTelemetry Deep Dive: Golang](https://www.youtube.com/watch?v=yQpyIrdxmQc)
- [Golang Microservices: Observability using OpenTelemetry](https://www.youtube.com/watch?v=bytCFQJ43DE)
- [Monitoring Go Applications with OpenTelemetry | Johannes Liebermann](https://www.youtube.com/watch?v=R3A3BjpMi6k)
- [GopherCon UK 2021: Chris Reeves - Instrumenting GO Applications](https://www.youtube.com/watch?v=Xo7S5fQq2V8)
- [Workshop: Getting started with OpenTelemetry and Distributed Tracing in Golang](https://www.youtube.com/watch?v=p73-PvchUl8)
- [Distributed Tracing on Go using OpenTelemetry - Fahri Yardımcı - GopherCon Turkey 2020](https://www.youtube.com/watch?v=I7pQWjYl6nM)


### OpenTelemetry Java
- [OpenTelemetry Java SIG Playlist](https://www.youtube.com/playlist?list=PLVYDBkQ1TdywnpttVBGlxxkzHMqhpmIev)
- [Spring Boot - Monitor your Spring Boot Application with OpenTelemetry & SigNoz](https://www.youtube.com/watch?v=YxZb17_LYwQ)
- [Monitor your Tomcat Java Application in 20 mins with OpenTelemetry & SigNoz](https://www.youtube.com/watch?v=4obQilMqU4E)
- [Tutorial: OpenTelemetry Java Instrumentation with Spring Boot in under 5 minutes](https://www.youtube.com/watch?v=_Px-Xn0jEGY)
- [OpenTelemetry Deep Dive: Java](https://www.youtube.com/watch?v=2v4yYhGgK_E&t=8s)
- [Getting Started with OpenTelemetry and Distributed Tracing in Java](https://www.youtube.com/watch?v=7h9LTTrGL28)
- [Tutorial: Auto-instrumentation of a Java app by OpenTelemetry for K8s Environment](https://www.youtube.com/watch?v=P_74rhI1M30)
- [OpenTelemetry Java Auto-Instrumentation SIG 2020/03/19](https://www.youtube.com/watch?v=88ZjCbT6LPc)
- [Observability in Java Getting Started with OpenTelemetry](https://www.youtube.com/watch?v=tsaT4L3DF3Q)


### OpenTelemetry JavaScript
- [OpenTelemetry JavaScript SIG Playlist](https://www.youtube.com/playlist?list=PLVYDBkQ1Tdyz-EZEjVRb3BX_s4jEgHaWd)

#### By SigNoz:
- [Angular Instrumentation - Monitor your Angular application with Opentelemetry and SigNoz](https://www.youtube.com/watch?v=g-I-v1FtMoM&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=3)
- [React Instrumentation - Implementing OpenTelemetry in React applications | Tutorial](https://www.youtube.com/watch?v=IsOQxc3wqyc&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=5)
- [NestJS - Monitoring your NestJS Application using OpenTelemetry and SigNoz](https://www.youtube.com/watch?v=tpNDrJAjcto&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=9)
- [NodeJs Instrumentation Monitor Custom Metrics from your application using OpenTelemetry & SigNoz](https://www.youtube.com/watch?v=7Ni78SajFLM&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=11&t=93s)
- [NodeJS Application Monitoring with OpenTelemetry & SigNoz](https://www.youtube.com/watch?v=au7ef1tJwEM&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=12)
- [Express - Monitoring your Express Application using OpenTelemetry and SigNoz](https://www.youtube.com/watch?v=AKu1rlP6j_w&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=14)
- [NodeJs OpenTelemetry - Implementing Distributed Tracing in a NodeJS Application using OpenTelemetry](https://www.youtube.com/watch?v=CgByZJeuRZY&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=17)
- [NextJS - Monitoring your NextJS application using OpenTelemetry and SigNoz](https://www.youtube.com/watch?v=sC1xNIcItTM&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=23)

#### Others:
- [OpenTelemetry 2019-10-23 JavaScript SIG](https://www.youtube.com/watch?v=JOgSzSPt-F0)
- [Workshop: Getting Started with OpenTelemetry in Javascript with Express and React](https://www.youtube.com/watch?v=RhVXCpEKMkg)
- [Tutorial: OpenTelemetry Node.js Instrumentation in 5 Minutes](https://www.youtube.com/watch?v=n-Ar0nnho3s)
- [Distributed tracing for Node.js using OpenTelemetry | Michael Haberman | Conf42 JavaScript 2021](https://www.youtube.com/watch?v=yqHxcm0soTU)
- [Workshop: Getting Started with OpenTelemetry and Distributed Tracing in Node.js](https://www.youtube.com/watch?v=LIzHgDffvjU)
- [Getting Started with OpenTelemetry and Distributed Tracing in Node.js](https://www.youtube.com/watch?v=whibfYKeA5Q)
- [Node.js Meetup - Trace-Based Testing with OpenTelemetry - Michael Haberman](https://www.youtube.com/watch?v=sTpNiAFnENE)
  


### OpenTelemetry PHP
- [OpenTelemetry PHP SIG Playlist](https://www.youtube.com/playlist?list=PLVYDBkQ1Tdyw5ccPWGur1s2Ohnt9f6eEO)
- [PHP - Monitoring a PHP application with OpenTelemetry and SigNoz](https://www.youtube.com/watch?v=BhoVFt9z5wk)

### OpenTelemetry Python
- [OpenTelemetry Python SIG Playlist](https://www.youtube.com/playlist?list=PLVYDBkQ1TdyzMaMC7Rqr7dLRISyhtU7hR)


#### By SigNoz:
- [Python Instrumentation - Monitor your Python application using OpenTelemetry and SigNoz](https://www.youtube.com/watch?v=oZkFfMN57yI)
- [FastAPI - Monitoring your FastAPI Application using OpenTelemetry with SigNoz](https://www.youtube.com/watch?v=R2VX2T1WB-I)
- [Flask OpenTelemetry - Monitoring your Flask application using OpenTelemetry](https://www.youtube.com/watch?v=_URJaj0dYz8&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=18&)
- [Django - Monitoring Django Application performance with OpenTelemetry](https://www.youtube.com/watch?v=fmDLpaF1xFc&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=19&)
- [Falcon - Monitoring apps based on Falcon Web Framework with OpenTelemetry](https://www.youtube.com/watch?v=ntW_3t5J34g&list=PL0N8FjJpzGl_VLU-PedUdnWXUybA90pcP&index=24)
  

#### Others:  
- [Getting Started with OpenTelemetry in Python](https://www.youtube.com/watch?v=WS-iDN2BOMs)
- [Getting Started with OpenTelemetry and Distributed Tracing in Python](https://www.youtube.com/watch?v=0ANtbk5fNbI)
- [OpenTelemetry and Distributed Tracing in Python](https://www.youtube.com/watch?v=tmoCZHUOUgc)
- [OpenTelemetry Deep Dive: Python](https://www.youtube.com/watch?v=SZlrq9_CZVg)
- [OpenTelemetry for Python Developers](https://www.youtube.com/watch?v=RJeJWdTGieM)
- [Workshop: Getting Started with OpenTelemetry in Python and Django](https://www.youtube.com/watch?v=uIImfoLUi24)
- [The Fundamentals of OpenTelemetry in Python | Live Workshop](https://www.youtube.com/watch?v=XQnssN02NkE)
- [Code instrumentation with Python and OpenTelemetry | Python Medellín](https://www.youtube.com/watch?v=jon8hicqROo)
- [Adding Observability To Your Python Applications With OpenTelemetry](https://www.youtube.com/watch?v=OT8gXklqW2E)



### OpenTelemetry Ruby
- [OpenTelemetry Ruby SIG Playlist](https://www.youtube.com/playlist?list=PLVYDBkQ1Tdywzk5WGUYE2wJuzyrOCBBdz)
- [Ruby - Tracing a Ruby application with OpenTelemetry for performance monitoring](https://www.youtube.com/watch?v=sNMIyQh7Oyo)
- [OpenTelemetry for Rubyists by Francis Wang](https://www.youtube.com/watch?v=0XIB9KF9w2w)



### OpenTelemetry Rust 

- [Rust - Implementing OpenTelemetry in a Rust application for performance monitoring](https://www.youtube.com/watch?v=yPt1Pc3_tls) 
- [Rust Dublin July 2021 - OpenTelemetry and Rust](https://www.youtube.com/watch?v=DURrAo9lPFA)
- [Observe with Rust: OpenTelemetry and Tremor - Gary White Jr., Wayfair](https://www.youtube.com/watch?v=RI9cy8OJQmY)
- [The Rust Programming Language - OpenTelemetry and Rust](https://www.youtube.com/watch?v=6iz9xCCPNPA)
- [OpenTelemetry for Rust Developers](https://www.youtube.com/watch?v=JNZoo_8XeaE)


### OpenTelemetry Swift
- Did not find any videos. 

--- 

## Join the Community 
- [Join the Community](https://opentelemetry.io/community/)
- [Mailing Lists](https://github.com/open-telemetry/community#mailing-lists)
- [Community GitHub](https://github.com/open-telemetry/community)
- [Calendar - OpenTelemetry](https://calendar.google.com/calendar/embed?src=google.com_b79e3e90j7bbsa2n2p5an5lf60%40group.calendar.google.com)
- [Reddit](https://www.reddit.com/r/OpenTelemetry/)
- [Gitter](https://gitter.im/open-telemetry/community?at=5fdb93b299256527beb7c619) *- archived*
- [Twitch](https://www.twitch.tv/opentelemetry)
- [Offical YouTube](https://www.youtube.com/channel/UCHZDBZTIfdy94xMjMKz-_MA/playlists)





### Newsletters 📰
- [o11y news!](https://o11y.news) -  Newsletter about Observability.
- [Observability news](https://buttondown.email/o11y.news) - Updates around observability (o11y) with a special focus on open source.
- [The new stack](https://thenewstack.io/category/monitoring/) - A newsletter digest of the week’s most important stories & analyses.


### Podcasts 
- [Changelog]( https://changelog.com/topic/observability)
- [StackOverflow Podcast #343](https://stackoverflow.blog/2021/06/01/podcast-343-unpacking-observability-and-opentelemetry-with-spiros-xanthos-of-splunk/)

### Events 
- [CNCF](https://www.cncf.io/events/) - CNCF Events
- [SREcon](https://www.usenix.org/conference/srecon22americas)
- [Opentelemetery Community Days]()
- [GrafanaCON](https://grafana.com/about/events/grafanacon/2022/)



### StackOverflow 
- [OpenTelemetry Tagged Questions](https://stackoverflow.com/tags/open-telemetry/new)
- [StackOverflow Podcast #343](https://stackoverflow.blog/2021/06/01/podcast-343-unpacking-observability-and-opentelemetry-with-spiros-xanthos-of-splunk/)
- [StackOverflow Blog](https://stackoverflow.blog/2021/09/08/observability-is-key-to-the-future-of-software-and-your-devops-career/)

### Twitter
- [SigNoz]()
- [Opentelemetry](https://twitter.com/opentelemetry)
- [Opentelemetry Bot](https://twitter.com/theotelbot)
- [Opentracing](https://twitter.com/opentracing)
- [Opencensusio](https://twitter.com/opencensusio)
- [CNCF](https://twitter.com/CloudNativeFdn)

<br>

- [JaegerTracing](https://twitter.com/JaegerTracing)
- [PrometheusMonitoring](https://twitter.com/PrometheusIO)
- [Grafana](https://twitter.com/grafana)
- [Zipkin](https://twitter.com/zipkinproject)
- [gRPC](https://twitter.com/grpcio)
- [Helm](https://twitter.com/HelmPack) 

<br>

- [SREcon](https://twitter.com/srecon)
- [LightstepHQ](https://twitter.com/LightstepHQ)
- [DynaTrace]()
- [HoneyComb](https://twitter.com/honeycombio)
- [Dyte](https://twitter.com/dyte_io)
- [Aspecto](https://twitter.com/AspectoInc)
- [tracetest_io](https://twitter.com/tracetest_io) - End-to-end tests powered by your OpenTelemetry Traces.
- [OpsMatters](https://twitter.com/opsmatters_uk)


<br>

- [Ted Young](https://twitter.com/tedsuo) - Co-founded the OpenTelemetry Project
- [Ben Sigelman](https://twitter.com/el_bhs) - Co-created OpenTelemetry & OpenTracing
- [Alolita Sharma](https://twitter.com/alolita)
- [Liz Fong-Jones](https://twitter.com/lizthegrey) - Governance OpenTelemetry
- [Juraci Paixão Kröhling](https://twitter.com/jpkrohling) -  Opentelemetry Maintainer.
- [Alex Boten](https://twitter.com/codeboten)
- [Sam Xie](https://twitter.com/SamXieHere) - Opentelemetry Member
- [Yoshi](https://twitter.com/ymotongpoo) 


### Slack
- [SigNoz](https://join.slack.com/t/signoz-community/shared_invite/zt-lrjknbbp-J_mI13rlw8pGF4EWBnorJA)
- [Opentelemetry - CNCF](https://cloud-native.slack.com/?redir=%2Farchives%2FCJFCJHG4Q)


**[`^ back to top ^`](#contents)**

---



**Special Mention:** [Awesome Opentelemetry](https://github.com/magsther/awesome-opentelemetry) - A curated list of OpenTelemetry resources.

**Maintainer** - Priyansh Khodiyar ([@zriyansh](https://github.com/zriyansh)) creator of [awesome-os](https://github.com/zriyansh/awesome-os).

**[`^ back to top ^`](#contents)**



