# Awesome OpenTelemetry 🎉
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A carefully curated list of open source content related to OpenTelemetry. 



## What is OpenTelemetry?

**OpenTelemetry** or OTel is an open-source project, which allows you to collect, export, and generate *traces*, *logs*, and, *metrics* (also known as the three pillars of observability). It is a set of APIs and SDKs.

> “When we announced the OpenTelemetry project in 2019, we envisioned it as the next major version of both OpenTracing and OpenCensus,” said Ben Sigelman, one of the co-creators of both OpenTracing and OpenTelemetry. 


## Contents
- [Awesome OpenTelemetry 🎉](#awesome-opentelemetry-)
  - [What is OpenTelemetry?](#what-is-opentelemetry)
  - [Contents](#contents)
  - [OpenTelemetry Instrumentation](#opentelemetry-instrumentation)
    - [Supported Languages](#supported-languages)
    - [Supported Databases 💿](#supported-databases-)
    - [OpenTelemetry Registry](#opentelemetry-registry)
    - [Secure your POD 🔐](#secure-your-pod-)
  - [Distributed Tracing Solutions](#distributed-tracing-solutions)
    - [Open Source Tools ⚙️](#open-source-tools-️)
    - [Opentelemetry Vendors](#opentelemetry-vendors)
  - [Terminology 📙](#terminology-)
  - [Statistics 📊](#statistics-)
  - [Main Components 🏛](#main-components-)
  - [Tools 🛠](#tools-)
  - [Books 📚](#books-)
    - [Case Studies 📑](#case-studies-)
  - [Join the Community ✅](#join-the-community-)
  - [Stay in Touch 💻](#stay-in-touch-)
    - [Newsletters 📰](#newsletters-)
    - [Podcasts 🎙](#podcasts-)
    - [Events 🎪](#events-)
    - [StackOverflow](#stackoverflow)
    - [Twitter](#twitter)
    - [Slack](#slack)
 

Here starts the list of awesome resources! Enjoy. 

---

## OpenTelemetry Instrumentation

### Supported Languages 
| Language                                                                        | Client Repo                                                                  | Contrib Repo                                                                   | API and SDK                                                          | Auto Instrumentation                                                                                   |
| ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ------------------------------------------------------------------------------ | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| [C++](https://opentelemetry.io/docs/instrumentation/cpp/)                       | [Client ](https://github.com/open-telemetry/opentelemetry-cpp)           | [Contrib](https://github.com/open-telemetry/opentelemetry-cpp-contrib)         |
| [.NET](https://opentelemetry.io/docs/instrumentation/net/automatic/)            | [Client ](https://github.com/open-telemetry/opentelemetry-dotnet)        | [Contrib ](https://github.com/open-telemetry/opentelemetry-dotnet-contrib) |                                                                      | [Auto Instrumentation Support](https://github.com/open-telemetry/opentelemetry-dotnet-instrumentation) |
| [Erlang/Elixir](https://opentelemetry.io/docs/instrumentation/erlang/)          |                                                                              | [Contrib](https://github.com/open-telemetry/opentelemetry-erlang-contrib)      | [SDK](https://github.com/open-telemetry/opentelemetry-erlang) |                                                                                                        |
| [Go](https://opentelemetry.io/docs/instrumentation/go/getting-started/)         |                                                                              | [Contrib ](https://github.com/open-telemetry/opentelemetry-go-contrib)     | [API and SDK](https://github.com/open-telemetry/opentelemetry-go)    |
| [Java](https://opentelemetry.io/docs/instrumentation/java/automatic/)    |       | [ Contrib](https://github.com/open-telemetry/opentelemetry-java-contrib) |  [SDK](https://github.com/open-telemetry/opentelemetry-java)               |                                                                      | [Auto Instrumentation Support](https://github.com/open-telemetry/opentelemetry-java-instrumentation)   |
| [JavaScript](https://opentelemetry.io/docs/instrumentation/js/instrumentation/) | [Client ](https://github.com/open-telemetry/opentelemetry-js)            | [Contrib ](https://github.com/open-telemetry/opentelemetry-js-contrib)     | [API](https://github.com/open-telemetry/opentelemetry-js-api)        | Auto Instrumentation Support                                                                           |
| [PHP](https://opentelemetry.io/docs/instrumentation/php/getting_started/)       | [Github](https://github.com/open-telemetry/opentelemetry-php)                | [Contrib](https://github.com/open-telemetry/opentelemetry-php-contrib)         |                                                                      |
| [Python](https://opentelemetry.io/docs/instrumentation/python/getting-started/) |        | [Contrib ](https://github.com/open-telemetry/opentelemetry-python-contrib) | [API and SDK](https://github.com/open-telemetry/opentelemetry-python)  | Auto Instrumentation Support                                         |
| [Ruby](https://opentelemetry.io/docs/instrumentation/ruby/automatic/)           | [Contrib ](https://github.com/open-telemetry/opentelemetry-ruby-contrib) |                                                                                | [API and SDK](https://github.com/open-telemetry/opentelemetry-ruby)  | Auto Instrumentation Support                                                                           |
| [Rust](https://opentelemetry.io/docs/instrumentation/rust/)                     | [Github]()                                                                   |                                                                                | [API and SDK](https://github.com/open-telemetry/opentelemetry-rust)  |
| [Swift](https://opentelemetry.io/docs/instrumentation/swift/)                   | [Github]()                                                                   |                                                                                | [API](https://github.com/open-telemetry/opentelemetry-swift)         |

### Supported Databases 💿

| Value           | Description                                        |
| --------------- | -------------------------------------------------- |
| `other_sql`     | Some other SQL database. Fallback only. See notes. |
| `mssql`         | Microsoft SQL Server                               |
| `mysql`         | MySQL                                              |
| `oracle`        | Oracle Database                                    |
| `db2`           | IBM Db2                                            |
| `postgresql`    | PostgreSQL                                         |
| `redshift`      | Amazon Redshift                                    |
| `hive`          | Apache Hive                                        |
| `cloudscape`    | Cloudscape                                         |
| `hsqldb`        | HyperSQL DataBase                                  |
| `progress`      | Progress Database                                  |
| `maxdb`         | SAP MaxDB                                          |
| `hanadb`        | SAP HANA                                           |
| `ingres`        | Ingres                                             |
| `firstsql`      | FirstSQL                                           |
| `edb`           | EnterpriseDB                                       |
| `cache`         | InterSystems Caché                                 |
| `adabas`        | Adabas (Adaptable Database System)                 |
| `firebird`      | Firebird                                           |
| `derby`         | Apache Derby                                       |
| `filemaker`     | FileMaker                                          |
| `informix`      | Informix                                           |
| `instantdb`     | InstantDB                                          |
| `interbase`     | InterBase                                          |
| `mariadb`       | MariaDB                                            |
| `netezza`       | Netezza                                            |
| `pervasive`     | Pervasive PSQL                                     |
| `pointbase`     | PointBase                                          |
| `sqlite`        | SQLite                                             |
| `sybase`        | Sybase                                             |
| `teradata`      | Teradata                                           |
| `vertica`       | Vertica                                            |
| `h2`            | H2                                                 |
| `coldfusion`    | ColdFusion IMQ                                     |
| `cassandra`     | Apache Cassandra                                   |
| `hbase`         | Apache HBase                                       |
| `mongodb`       | MongoDB                                            |
| `redis`         | Redis                                              |
| `couchbase`     | Couchbase                                          |
| `couchdb`       | CouchDB                                            |
| `cosmosdb`      | Microsoft Azure Cosmos DB                          |
| `dynamodb`      | Amazon DynamoDB                                    |
| `neo4j`         | Neo4j                                              |
| `geode`         | Apache Geode                                       |
| `elasticsearch` | Elasticsearch                                      |
| `memcached`     | Memcached                                          |
| `cockroachdb`   | CockroachDB                                        |


Check full list [here.](https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/trace/semantic_conventions/database.md)

---

If you are using Kubernetes, you can use the [OpenTelemetry Operator for Kubernetes](https://github.com/open-telemetry/opentelemetry-operator) to [inject auto-instrumentation libraries](https://github.com/open-telemetry/opentelemetry-operator#opentelemetry-auto-instrumentation-injection) for Java, Node.js and Python into your application.



### OpenTelemetry Registry 
The [OpenTelemetry Registry](https://opentelemetry.io/registry/) allows you to search for instrumentation libraries, tracer implementations, utilities, and other useful projects in the OpenTelemetry ecosystem.


### Secure your POD 🔐
- [Secure OpenTelemetry Collector - Medium](https://medium.com/opentelemetry/securing-your-opentelemetry-collector-1a4f9fa5bd6f)

- [ConfigAuth](https://github.com/open-telemetry/opentelemetry-collector/tree/main/config/configauth)

- [PromQL Cheat SHeet](https://promlabs.com/promql-cheat-sheet/)


**[`^ back to top ^`](#contents)**

---

## Distributed Tracing Solutions

### Open Source Tools ⚙️

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
- [SigNoz - Open Source APM](https://signoz.io)
- [AppDynamics](https://www.appdynamics.com)
- [Aspecto](https://www.aspecto.io/)
- [AWS](https://aws-otel.github.io/)
- [Azure](https://docs.microsoft.com/azure/azure-monitor/app/opentelemetry-overview)
- [Datadog](https://docs.datadoghq.com/tracing/setup_overview/open_standards)
- [Dynatrace](https://www.dynatrace.com/support/help/how-to-use-dynatrace/transactions-and-services/service-monitoring-settings/opentelemetry/)
- [Elastic](https://www.elastic.co/guide/en/apm/get-started/current/open-telemetry-elastic.html)
- [F5](https://github.com/open-telemetry/opentelemetry-collector-contrib/tree/main/exporter/f5cloudexporter)
- [Grafana Labs](https://grafana.com/oss/opentelemetry/)
- [Honeycomb](https://docs.honeycomb.io/getting-data-in/)
- [Instana](https://www.ibm.com/docs/en/instana-observability)
- [Lightstep](https://github.com/lightstep?q=launcher)
- [LogicMonitor](https://www.logicmonitor.com/support/tracing/getting-started-with-tracing)
- [Logz.io](https://docs.logz.io/shipping/tracing-sources/opentelemetry.html#overview)
- [Lumingo](https://docs.lumigo.io/docs/opentelemetry)
- [New Relic](https://newrelic.com/solutions/opentelemetry)
- [Promscale](https://www.timescale.com/promscale/)
- [Sentry Software](https://www.sentrysoftware.com/products/hardware-sentry-opentelemetry-collector.html)
- [Splunk](https://www.splunk.com/en_us/blog/conf-splunklive/announcing-native-opentelemetry-support-in-splunk-apm.html)
- [Sumo Logic](https://help.sumologic.com/Traces/Getting_Started_with_Transaction_Tracing)
- [Uptrace](https://uptrace.dev/)

[Click here for full list of vendors that supports OpenTelemetry.](https://opentelemetry.io/vendors/)



## Terminology 📙
- [Components](https://www.jaegertracing.io/docs/1.30/architecture/#terminology)
- [Glossary](https://opentelemetry.io/docs/concepts/glossary/)

## Statistics 📊
- [DevStats - Opentelemetry](https://opentelemetry.devstats.cncf.io/d/8/dashboards?orgId=1&refresh=15m)
- [Google Trends](https://trends.google.com/trends/explore?date=today%205-y&q=opentelemetry)


## Main Components 🏛

- **OpenTelemetry Protocol (OTLP)** specification describes the encoding, transport, and delivery mechanism of telemetry data between telemetry sources, intermediate nodes such as collectors, and telemetry backends.
- **OpenTelemetry Collector** offers a vendor-agnostic implementation on receiving, processing, and exporting telemetry data and removing the need to run, operate, and maintain multiple agents/collectors.
- **APIs and SDKs** in 11 different languages, enabling users to easily integrate and extend the project.


**[`^ back to top ^`](#contents)**

---


## Tools 🛠
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



### Case Studies 📑
- [CNCF](https://www.cncf.io/case-studies/)
- [How Lightstep Implemented Observability](https://www.oreilly.com/videos/how-lightstep-implemented/0636920623601/)



**[`^ back to top ^`](#contents)**


--- 

## Join the Community ✅
- [Join the Community](https://opentelemetry.io/community/)
- [Mailing Lists](https://github.com/open-telemetry/community#mailing-lists)
- [Community GitHub](https://github.com/open-telemetry/community)
- [Calendar - OpenTelemetry](https://calendar.google.com/calendar/embed?src=google.com_b79e3e90j7bbsa2n2p5an5lf60%40group.calendar.google.com)
- [Reddit](https://www.reddit.com/r/OpenTelemetry/)
- [Gitter](https://gitter.im/open-telemetry/community?at=5fdb93b299256527beb7c619) *- archived*
- [Twitch](https://www.twitch.tv/opentelemetry)
- [Current Status](https://opentelemetry.io/status/)



## Stay in Touch 💻

### Newsletters 📰
- [o11y news!](https://o11y.news) -  Newsletter about Observability.
- [Observability news](https://buttondown.email/o11y.news) - Updates around observability (o11y) with a special focus on open source.
- [The new stack](https://thenewstack.io/category/monitoring/) - A newsletter digest of the week’s most important stories & analyses.


### Podcasts 🎙
- [Changelog]( https://changelog.com/topic/observability)
- [StackOverflow Podcast #343](https://stackoverflow.blog/2021/06/01/podcast-343-unpacking-observability-and-opentelemetry-with-spiros-xanthos-of-splunk/)

### Events 🎪
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
- 

<br>

- [SREcon](https://twitter.com/srecon)
- [LightstepHQ](https://twitter.com/LightstepHQ)
- [DynaTrace]()
- [HoneyComb](https://twitter.com/honeycombio)
- [Dyte](https://twitter.com/dyte_io)
- [Aspecto](https://twitter.com/AspectoInc)

<br>

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
- 

### Slack
- [SigNoz](https://join.slack.com/t/signoz-community/shared_invite/zt-lrjknbbp-J_mI13rlw8pGF4EWBnorJA)
- [Opentelemetry - CNCF](https://cloud-native.slack.com/?redir=%2Farchives%2FCJFCJHG4Q)


**[`^ back to top ^`](#contents)**

---



**Special Mention:** [Awesome Opentelemetry](https://github.com/magsther/awesome-opentelemetry) - A curated list of OpenTelemetry resources *(repo stagnant)*

**Maintainer** - Priyansh Khodiyar ([@zriyansh](https://github.com/zriyansh)) creator of [awesome-os](https://github.com/zriyansh/awesome-os).

**[`^ back to top ^`](#contents)**