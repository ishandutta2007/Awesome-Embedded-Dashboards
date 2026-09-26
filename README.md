# Awesome-Embedded-Dashboards

# 📊 Top Embedded Analytics Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Embedded Dashboards, Embedded Analytics, Customer-Facing BI, White-Label Analytics, Multi-Tenant Analytics & Data Apps*
**Last updated: September 2026**

This repository tracks notable **SaaS/Hosted platforms** and **open-source GitHub projects** for **embedded analytics and embedded dashboards**.

Embedded analytics allows software companies to place **dashboards, reports, charts, self-service analytics and data exploration directly inside their own applications**, allowing customers to consume analytics without leaving the product.

Typical capabilities include **white-labeling, multi-tenancy, row-level security, embedded dashboards, interactive charts, self-service exploration, dashboard builders, semantic layers, APIs/SDKs, SSO, customer-specific data access, analytics portals and developer-controlled customization**.

**Examples** include Explo, Toucan Toco, GoodData, Sisense, Looker Embedded, Reveal BI, Bold BI, Logi Analytics, Metabase Enterprise and Holistics.

**Open-source emphasis:** This repository places particular emphasis on **self-hosted and open-source alternatives**, including complete BI platforms that support embedding, embedded analytics SDKs, semantic layers, dashboard builders, visualization libraries and data infrastructure that can be assembled into a customer-facing analytics product.

A useful distinction is that an open-source embedded analytics stack does **not necessarily need to be a single product**:

```text
                    YOUR SaaS APPLICATION
                            │
             ┌──────────────┴──────────────┐
             │                             │
             ▼                             ▼
        Application UI                Analytics UI
             │                             │
             └──────────────┬──────────────┘
                            ▼
                  Embedded Analytics Layer
                            │
              ┌─────────────┼─────────────┐
              ▼             ▼             ▼
          Dashboards    Semantic Layer   APIs/SDK
              │             │             │
              └─────────────┼─────────────┘
                            ▼
                       Data Warehouse
                            │
              PostgreSQL / ClickHouse / DuckDB
```

For example, **Apache Superset** provides an Embedded SDK for placing Superset dashboards inside another application, while **Metabase** provides modular embedding and React/web-component approaches. **Lightdash** provides an open-source BI platform with embedding capabilities, and **Cube Core** provides an open-source semantic layer specifically designed to power embedded analytics and other downstream applications.

Contributions welcome! Add new embedded analytics platforms, self-hosted BI systems, embedding SDKs, semantic layers, visualization libraries and related open-source projects.

---

## Table of Contents

* [SaaS/Hosted Platforms](#saashosted-platforms)
* [Open-Source GitHub Projects](#open-source-github-projects)

  * [Complete Open-Source BI & Embedded Analytics Platforms](#complete-open-source-bi--embedded-analytics-platforms)
  * [Open-Source Embedded Analytics Engines](#open-source-embedded-analytics-engines)
  * [Semantic Layers](#semantic-layers)
  * [Dashboard & Visualization Frameworks](#dashboard--visualization-frameworks)
  * [Embedded Analytics SDKs & Components](#embedded-analytics-sdks--components)
  * [Additional Strong Open-Source Options](#additional-strong-open-source-options)
* [Commercial → Open-Source Capability Mapping](#commercial--open-source-capability-mapping)
* [Framework for Building a Self-Hosted Embedded Analytics Platform](#framework-for-building-a-self-hosted-embedded-analytics-platform)
* [How to Contribute](#how-to-contribute)
* [Disclaimer](#disclaimer)

---

## SaaS/Hosted Platforms

* **[Explo](https://www.explo.co/)**
  Developer-focused embedded analytics platform for embedding dashboards and reports into SaaS applications, with APIs, SDKs, customization and customer-specific analytics.

* **[Toucan Toco](https://www.toucantoco.com/)**
  Embedded analytics platform focused on customer-facing analytics, white-labeling, guided data experiences, multi-tenancy and native-looking analytics experiences. Toucan describes its embedded product as supporting web components/SDKs, white-labeling, row-level security and token-based tenant isolation.

* **[GoodData](https://www.gooddata.ai/)**
  Embedded analytics platform providing dashboards, visualizations, self-service analytics, AI-assisted analytics, white-labeling and multi-tenant embedded analytics.

* **[Sisense](https://www.sisense.com/)**
  Embedded analytics platform for integrating governed analytics, dashboards, self-service exploration and AI-powered analytics into applications using APIs, SDKs and customizable components.

* **[Looker](https://cloud.google.com/looker)**
  Google Cloud's BI and analytics platform with embedded analytics capabilities, governed semantic modeling and APIs for integrating analytics into applications.

* **[Reveal Embedded Analytics](https://www.revealbi.io/)**
  Embedded BI platform designed for integrating interactive dashboards, reports and analytics into applications using SDKs and developer-oriented embedding capabilities.

* **[Bold BI](https://www.boldbi.com/)**
  Embedded analytics platform providing interactive dashboards, JavaScript SDKs, REST APIs, white-labeling, theming, filtering and multi-tenant embedding.

* **[Logi Analytics](https://www.logianalytics.com/)**
  Embedded analytics platform for integrating dashboards, reports, data visualizations and self-service analytics into software products.

* **[Metabase](https://www.metabase.com/)**
  Open-core BI platform with embedded analytics capabilities for dashboards, questions and interactive data exploration. Its current embedding system supports view-only, interactive and editable embedding, with advanced interactive embedding available on paid plans.

* **[Holistics](https://www.holistics.io/)**
  BI and embedded analytics platform supporting embedded dashboards and portals, white-labeling, self-service exploration, signed URLs, authentication and multi-tenant row-level permissions.

* **[Luzmo](https://www.luzmo.com/)**
  Embedded analytics platform designed for SaaS applications with customizable dashboards, self-service analytics and developer-friendly embedding.

* **[Embeddable](https://embeddable.com/)**
  Developer-focused embedded analytics platform for building customizable customer-facing dashboards and analytics experiences directly into applications.

* **[Tableau Embedded](https://www.tableau.com/developer/tools/embedding)**
  Tableau's embedding capabilities for integrating Tableau visualizations and analytics into applications and portals.

* **[Power BI Embedded](https://azure.microsoft.com/products/power-bi-embedded/)**
  Microsoft Azure service for embedding Power BI reports, dashboards and analytics into applications.

* **[Sigma Computing](https://www.sigmacomputing.com/)**
  Cloud analytics platform with embedded analytics capabilities for integrating interactive data experiences into applications.

* **[Domo Embedded](https://www.domo.com/product/embedded-analytics)**
  Embedded analytics offering for integrating Domo-powered analytics and data experiences into customer-facing applications.

* **[Qlik Embedded Analytics](https://www.qlik.com/us/products/embedded-analytics)**
  Embedded analytics capabilities from Qlik for integrating interactive analytics, visualizations and governed data experiences into applications.

* **[ThoughtSpot Embedded](https://www.thoughtspot.com/product/embedded-analytics)**
  Embedded analytics platform focused on search-driven, AI-assisted and self-service analytics inside SaaS products.

* **[Yellowfin](https://www.yellowfinbi.com/)**
  BI and analytics platform supporting embedded analytics, dashboards, data storytelling and self-service analytics.

* **[Preset](https://preset.io/)**
  Hosted Apache Superset platform providing managed BI and analytics capabilities based on the open-source Superset ecosystem.

* **[Holistics](https://www.holistics.io/)**
  Embedded BI and analytics platform with dashboard embedding and full embedded portals, including multi-tenant row-level permissions and white-labeling.

---

## Open-Source GitHub Projects

> **Open-source emphasis:** The projects below are intentionally broader than direct SaaS replacements. The first group contains complete BI/analytics platforms that can be self-hosted and embedded. The later groups contain semantic layers, SDKs, dashboard frameworks, visualization engines and infrastructure that can be combined into a full Explo/Toucan/GoodData-style embedded analytics stack.

### Complete Open-Source BI & Embedded Analytics Platforms

* **[Apache Superset](https://github.com/apache/superset)**
  Open-source modern BI and data-exploration platform supporting dashboards, charts, SQL exploration, APIs and an official Embedded SDK. The Embedded SDK allows Superset dashboards to be inserted into applications using the host application's authentication.

* **[Metabase](https://github.com/metabase/metabase)**
  Open-source BI platform with dashboards, query building and embedding capabilities. Metabase supports modular embedding of dashboards, questions and the query builder, including React and web-component approaches.

* **[Lightdash](https://github.com/lightdash/lightdash)**
  Open-source BI platform built around governed metrics and dbt, with dashboards, data apps, SDK-based embedding, permissions and self-hosting. Lightdash explicitly supports embedding dashboards, AI agents and Data Apps into products.

* **[Redash](https://github.com/getredash/redash)**
  Open-source data visualization and dashboarding platform designed around querying databases and building interactive visualizations and dashboards.

* **[Rill Developer](https://github.com/rilldata/rill)**
  Open-source developer-oriented BI platform for building dashboards and analytics applications from data models and metrics.

* **[Evidence](https://github.com/evidence-dev/evidence)**
  Open-source code-based BI platform where dashboards and reports can be built from SQL and version-controlled like software.

* **[Streamlit](https://github.com/streamlit/streamlit)**
  Open-source Python framework for turning data scripts into interactive data applications and dashboards, useful for building custom analytics portals.

* **[Dash](https://github.com/plotly/dash)**
  Open-source Python framework for building interactive analytical web applications and dashboards.

* **[Shiny](https://github.com/rstudio/shiny)**
  Open-source framework for building interactive data applications, dashboards and analytical interfaces using R or Python.

* **[Grafana](https://github.com/grafana/grafana)**
  Open-source dashboard and visualization platform with extensive data-source support, plugins and APIs; useful as a foundation for embedded operational analytics.

* **[Apache Superset Embedded SDK](https://github.com/apache/superset/tree/master/superset-embedded-sdk)**
  Dedicated open-source SDK for embedding Superset dashboards into applications with guest-token authentication and configurable dashboard UI.

### Open-Source Embedded Analytics Engines

* **[Apache Superset](https://github.com/apache/superset)**
  Full open-source BI platform with an official embedding SDK and API ecosystem.

* **[Metabase](https://github.com/metabase/metabase)**
  Open-source BI platform that can be embedded into applications through modular and full-app embedding approaches.

* **[Lightdash](https://github.com/lightdash/lightdash)**
  Open-source BI and data-app platform with SDK-based embedding, user attributes and row-level security capabilities.

* **[Rill](https://github.com/rilldata/rill)**
  Open-source analytics application platform optimized for fast dashboard creation over analytical datasets.

* **[Redash](https://github.com/getredash/redash)**
  Open-source query and visualization platform suitable for building customer-facing dashboards around SQL data.

* **[Grafana](https://github.com/grafana/grafana)**
  Open-source analytics and observability platform that can serve as the visualization layer for an embedded analytics architecture.

### Semantic Layers

* **[Cube](https://github.com/cube-js/cube)**
  Open-source semantic layer for embedded analytics, BI and AI applications. Cube Core lets developers define metrics, dimensions, joins and access rules once and expose them through SQL, REST and GraphQL APIs. It is explicitly designed to power custom embedded analytics experiences.

* **[Lightdash](https://github.com/lightdash/lightdash)**
  Open-source BI platform with a governed context/semantic layer for defining metrics, dimensions, joins, permissions and business logic.

* **[MetricFlow](https://github.com/dbt-labs/metricflow)**
  Open-source semantic-layer technology for defining metrics and querying them consistently across analytics applications.

* **[Transform](https://github.com/transform-data/transform)**
  Open-source semantic layer project for defining metrics and dimensions and serving them to downstream analytics applications.

* **[Malloy](https://github.com/malloydata/malloy)**
  Open-source analytical language and modeling system designed for reusable data definitions and analytical queries.

* **[Metric Store / Semantic Layer projects](https://github.com/topics/semantic-layer)**
  GitHub ecosystem of open-source semantic-layer implementations useful for creating governed embedded analytics architectures.

### Dashboard & Visualization Frameworks

* **[Grafana](https://github.com/grafana/grafana)**
  Open-source dashboarding platform supporting multiple data sources, panels, plugins, APIs and extensive visualization capabilities.

* **[Apache ECharts](https://github.com/apache/echarts)**
  Open-source JavaScript visualization library for building highly customized interactive charts and dashboards.

* **[Plotly.js](https://github.com/plotly/plotly.js)**
  Open-source JavaScript visualization library for interactive charts and analytical applications.

* **[Vega](https://github.com/vega/vega)**
  Open-source visualization grammar for creating declarative, interactive visualizations.

* **[Vega-Lite](https://github.com/vega/vega-lite)**
  High-level declarative visualization grammar useful for creating reusable analytics components.

* **[Observable Plot](https://github.com/observablehq/plot)**
  Open-source JavaScript visualization library optimized for exploratory and analytical graphics.

* **[D3.js](https://github.com/d3/d3)**
  Open-source JavaScript visualization framework for building fully custom embedded analytics interfaces.

* **[Nivo](https://github.com/plouc/nivo)**
  React-based open-source visualization component library useful for building custom embedded dashboards.

* **[Recharts](https://github.com/recharts/recharts)**
  React charting library useful for building lightweight custom analytics interfaces.

* **[Tremor](https://github.com/tremorlabs/tremor)**
  React component library for rapidly constructing dashboard and analytics interfaces.

### Embedded Analytics SDKs & Components

* **[Apache Superset Embedded SDK](https://github.com/apache/superset/tree/master/superset-embedded-sdk)**
  Official open-source SDK for embedding Superset dashboards inside host applications.

* **[Metabase Embedding](https://github.com/metabase/metabase)**
  Metabase provides web components and React-based embedding for dashboards, questions and the query builder.

* **[Cube Core](https://github.com/cube-js/cube)**
  Headless open-source semantic layer that exposes analytics through APIs and can be used to build custom embedded analytics experiences.

* **[Lightdash SDK](https://github.com/lightdash/lightdash)**
  Open-source Lightdash platform with SDK-based embedding for dashboards, Data Apps and analytics experiences.

* **[React Admin](https://github.com/marmelab/react-admin)**
  Open-source React framework for data-driven applications that can be used as a foundation for custom analytics portals and customer-facing admin interfaces.

* **[Apache Arrow](https://github.com/apache/arrow)**
  Open-source columnar data standard and ecosystem useful for high-performance analytical data transport between backend and visualization layers.

* **[Apache Arrow DataFusion](https://github.com/apache/datafusion)**
  Open-source query engine that can serve as an analytical backend for custom embedded analytics products.

### Additional Strong Open-Source Options

* **[ClickHouse](https://github.com/ClickHouse/ClickHouse)**
  High-performance open-source analytical database suitable for multi-tenant embedded analytics workloads and high-volume event data.

* **[DuckDB](https://github.com/duckdb/duckdb)**
  Open-source analytical database that can be embedded directly into applications, making it useful for local or application-level analytics.

* **[PostgreSQL](https://github.com/postgres/postgres)**
  Open-source relational database suitable for application data, tenant metadata, analytics data and row-level security implementations.

* **[Apache Druid](https://github.com/apache/druid)**
  Open-source real-time analytical database designed for high-performance slice-and-dice analytics.

* **[Apache Pinot](https://github.com/apache/pinot)**
  Open-source real-time OLAP datastore suitable for low-latency customer-facing analytics.

* **[Trino](https://github.com/trinodb/trino)**
  Open-source distributed SQL query engine capable of querying multiple heterogeneous data sources.

* **[Apache Spark](https://github.com/apache/spark)**
  Open-source distributed data-processing engine useful for large-scale analytical data preparation.

* **[dbt-core](https://github.com/dbt-labs/dbt-core)**
  Open-source analytics engineering framework useful for transforming raw customer data into governed models and metrics.

* **[Airbyte](https://github.com/airbytehq/airbyte)**
  Open-source data-integration platform useful for ingesting application and customer data into the analytics warehouse.

* **[Meltano](https://github.com/meltano/meltano)**
  Open-source ELT platform useful for building reproducible analytics data pipelines.

* **[Apache Airflow](https://github.com/apache/airflow)**
  Open-source workflow orchestration platform for scheduling analytics pipelines and data transformations.

* **[Dagster](https://github.com/dagster-io/dagster)**
  Open-source data orchestration framework suitable for building reliable embedded analytics data pipelines.

* **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)**
  Open-source metadata platform useful for data discovery, governance and lineage in analytics environments.

* **[OpenLineage](https://github.com/OpenLineage/OpenLineage)**
  Open-source standard for tracking data lineage across analytics pipelines.

* **[MinIO](https://github.com/minio/minio)**
  Open-source S3-compatible object storage useful for analytics data lakes.

* **[Keycloak](https://github.com/keycloak/keycloak)**
  Open-source identity and access-management platform useful for SSO and authentication around embedded analytics applications.

* **[n8n](https://github.com/n8n-io/n8n)**
  Open-source workflow automation platform useful for connecting analytics events, alerts, customer workflows and application systems.

---

## Commercial → Open-Source Capability Mapping

| Commercial Platform      | Primary Focus                                     | Open-Source Equivalents / Building Blocks       |
| ------------------------ | ------------------------------------------------- | ----------------------------------------------- |
| **Explo**                | Developer-first embedded dashboards               | Apache Superset + Embedded SDK + Cube + ECharts |
| **Toucan Toco**          | White-label embedded analytics + storytelling     | Lightdash + Cube + ECharts + custom React       |
| **GoodData**             | Enterprise embedded analytics + semantic layer    | Lightdash + Cube + Superset + PostgreSQL        |
| **Sisense**              | Enterprise embedded analytics + AI                | Lightdash + Cube + Superset + ClickHouse        |
| **Looker Embedded**      | Governed BI + semantic modeling + embedding       | Cube + Lightdash + Superset + dbt-core          |
| **Reveal BI**            | Embedded dashboards + self-service BI             | Superset + Metabase + ECharts                   |
| **Bold BI**              | Embedded dashboards + SDK/API + multi-tenancy     | Superset + Cube + ECharts + Keycloak            |
| **Logi Analytics**       | Embedded BI + developer customization             | Superset + Cube + React + ECharts               |
| **Metabase Enterprise**  | Embedded BI + self-service analytics              | Metabase OSS + Cube + PostgreSQL                |
| **Holistics**            | Embedded dashboards + portals + semantic modeling | Lightdash + Cube + Superset                     |
| **Luzmo**                | SaaS embedded analytics                           | Lightdash + Cube + ECharts                      |
| **Embeddable**           | Developer-first embedded analytics                | Cube + Superset + custom React                  |
| **Tableau Embedded**     | Rich visual analytics                             | Superset + ECharts + Vega                       |
| **Power BI Embedded**    | Enterprise BI embedding                           | Superset + Lightdash + Cube                     |
| **ThoughtSpot Embedded** | Search/AI-driven analytics                        | Cube + Lightdash + LLM layer + ECharts          |
| **Qlik Embedded**        | Governed associative analytics                    | Cube + Superset + ClickHouse                    |
| **Grafana**              | Operational analytics dashboards                  | Grafana OSS                                     |
| **Redash**               | SQL analytics + dashboards                        | Redash + PostgreSQL                             |
| **Evidence**             | Code-based analytics                              | Evidence + dbt-core + DuckDB                    |

> **Important:** These mappings are **capability-oriented rather than feature-for-feature replacements**. Commercial embedded analytics products generally bundle embedding, authentication, tenant isolation, semantic modeling, dashboards, self-service exploration, SDKs, white-labeling, support and enterprise controls. A self-hosted implementation will usually require several open-source components.

---

## Framework for Building a Self-Hosted Embedded Analytics Platform

A practical open-source architecture for building an **Explo / Toucan / GoodData / Sisense / Looker Embedded-style analytics platform** can be assembled from the following components:

| Layer                | Open-Source Technologies                                                    |
| -------------------- | --------------------------------------------------------------------------- |
| Frontend             | React · Next.js · Vue                                                       |
| Dashboard UI         | Superset · Metabase · Lightdash                                             |
| Custom Charts        | ECharts · D3.js · Plotly.js · Vega                                          |
| Embedded Analytics   | Superset Embedded SDK · Metabase Embedding · Lightdash SDK                  |
| Semantic Layer       | Cube Core · Lightdash · MetricFlow · Transform                              |
| Data Modeling        | dbt-core · SQL                                                              |
| Query Engine         | Trino · DataFusion · DuckDB                                                 |
| Analytics Database   | ClickHouse · Apache Druid · Apache Pinot                                    |
| Application Database | PostgreSQL                                                                  |
| Data Integration     | Airbyte · Meltano                                                           |
| Orchestration        | Airflow · Dagster                                                           |
| Object Storage       | MinIO                                                                       |
| Data Format          | Apache Arrow · Parquet                                                      |
| Authentication       | Keycloak                                                                    |
| Multi-Tenancy        | PostgreSQL RLS · Cube Security Context · Application-level tenant isolation |
| Visualization        | ECharts · D3 · Vega · Plotly                                                |
| API                  | FastAPI · Django · Node.js                                                  |
| Cache                | Redis                                                                       |
| Search               | OpenSearch                                                                  |
| Analytics            | DuckDB · Polars                                                             |
| Deployment           | Docker · Kubernetes                                                         |

### Recommended Architecture

```text
                         CUSTOMER'S APPLICATION
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
                    ▼                           ▼
              SaaS Application            Embedded Analytics
                    │                           │
                    │                  ┌────────┴────────┐
                    │                  │                 │
                    │                  ▼                 ▼
                    │             Dashboard UI      Custom Charts
                    │                  │                 │
                    │          Superset / Lightdash   ECharts
                    │          Metabase / Custom       D3.js
                    │                  │
                    └──────────────────┼─────────────────┘
                                       │
                                       ▼
                            EMBEDDING / API LAYER
                                       │
                         ┌─────────────┼─────────────┐
                         │             │             │
                         ▼             ▼             ▼
                       REST          GraphQL        SDK
                         │             │             │
                         └─────────────┼─────────────┘
                                       │
                                       ▼
                              SEMANTIC LAYER
                                       │
                             Cube Core / Lightdash
                                       │
                                       ▼
                              QUERY / SQL LAYER
                                       │
                    ┌──────────────────┼──────────────────┐
                    ▼                  ▼                  ▼
                ClickHouse          Trino             DuckDB
                    │                  │                  │
                    └──────────────────┼──────────────────┘
                                       │
                                       ▼
                              DATA TRANSFORMATION
                                       │
                               dbt-core / SQL
                                       │
                                       ▼
                              DATA INGESTION
                                       │
                         Airbyte / Meltano / Airflow
                                       │
                                       ▼
                             CUSTOMER DATA SOURCES
```

### Multi-Tenant Architecture

A production embedded analytics platform needs strong tenant isolation:

```text
                         APPLICATION USER
                                │
                                ▼
                         Authentication
                          Keycloak / SSO
                                │
                                ▼
                         Tenant Resolution
                                │
                     ┌──────────┴──────────┐
                     │                     │
                     ▼                     ▼
                  tenant_id            user_id
                     │                     │
                     └──────────┬──────────┘
                                ▼
                         Security Context
                                │
                                ▼
                         Semantic Layer
                       Cube / Lightdash
                                │
                                ▼
                         Row-Level Security
                                │
                                ▼
                       Analytics Database
                                │
              ┌─────────────────┼─────────────────┐
              ▼                 ▼                 ▼
           Tenant A          Tenant B          Tenant C
           Data Only        Data Only          Data Only
```

### Embedded Analytics Request Flow

```text
User Opens SaaS Application
            ↓
Application Authenticates User
            ↓
Resolve customer / tenant
            ↓
Generate signed analytics token
            ↓
Pass tenant + user context
            ↓
Embedded Dashboard / SDK
            ↓
Semantic Layer
            ↓
Apply Row-Level Security
            ↓
Generate SQL
            ↓
Query Analytics Warehouse
            ↓
Return Customer-Specific Data
            ↓
Render Dashboard Inside SaaS
```

---

## Open-Source Embedded Analytics Stack

```text
                         ┌────────────────────────┐
                         │     SaaS PRODUCT       │
                         │                        │
                         │ React / Next.js / Vue  │
                         └────────────┬───────────┘
                                      │
                                      ▼
                         ┌────────────────────────┐
                         │ EMBEDDED EXPERIENCE    │
                         │                        │
                         │ Superset SDK           │
                         │ Metabase Embedding     │
                         │ Lightdash SDK          │
                         │ Custom React            │
                         └────────────┬───────────┘
                                      │
                                      ▼
                         ┌────────────────────────┐
                         │    SEMANTIC LAYER      │
                         │                        │
                         │ Cube Core               │
                         │ Lightdash               │
                         │ MetricFlow              │
                         └────────────┬───────────┘
                                      │
                                      ▼
                         ┌────────────────────────┐
                         │     QUERY ENGINE       │
                         │                        │
                         │ Trino · DataFusion     │
                         │ DuckDB                 │
                         └────────────┬───────────┘
                                      │
                                      ▼
                         ┌────────────────────────┐
                         │ ANALYTICAL DATABASE    │
                         │                        │
                         │ ClickHouse             │
                         │ Pinot · Druid          │
                         │ PostgreSQL              │
                         └────────────┬───────────┘
                                      │
                                      ▼
                         ┌────────────────────────┐
                         │ DATA TRANSFORMATION    │
                         │                        │
                         │ dbt-core                │
                         └────────────┬───────────┘
                                      │
                                      ▼
                         ┌────────────────────────┐
                         │      DATA INGESTION    │
                         │                        │
                         │ Airbyte · Meltano      │
                         │ Airflow · Dagster      │
                         └────────────────────────┘
```

---

## Embedded Analytics Capability Matrix

| Capability                 | Commercial Embedded BI | Open-Source Options                 |
| -------------------------- | ---------------------- | ----------------------------------- |
| Embedded Dashboards        | ✓                      | Superset · Metabase · Lightdash     |
| Interactive Charts         | ✓                      | ECharts · D3 · Vega · Plotly        |
| Self-Service Analytics     | ✓                      | Metabase · Superset · Lightdash     |
| Dashboard Builder          | ✓                      | Metabase · Superset · Lightdash     |
| White Labeling             | ✓                      | Custom UI · CSS · SDKs              |
| Multi-Tenancy              | ✓                      | Cube · PostgreSQL RLS · Keycloak    |
| Row-Level Security         | ✓                      | Cube · PostgreSQL RLS · Superset    |
| SSO                        | ✓                      | Keycloak · OAuth · OIDC             |
| Signed Embedding           | ✓                      | Superset · Custom JWT               |
| REST API                   | ✓                      | Cube · Superset · Metabase          |
| GraphQL                    | ✓                      | Cube                                |
| React SDK                  | ✓                      | Metabase · custom React · Lightdash |
| Semantic Layer             | ✓                      | Cube · Lightdash · MetricFlow       |
| Metric Definitions         | ✓                      | Cube · Lightdash · dbt              |
| SQL Analytics              | ✓                      | Superset · Metabase · Redash        |
| Real-Time Analytics        | ✓                      | ClickHouse · Pinot · Druid          |
| High-Concurrency Analytics | ✓                      | ClickHouse · Pinot · Cube           |
| Embedded AI                | ✓                      | Cube + LLM · Lightdash              |
| Custom Visualization       | ✓                      | ECharts · D3 · Vega                 |
| Data Apps                  | ✓                      | Lightdash · Streamlit · Dash        |
| Data Pipelines             | ✓                      | Airbyte · Meltano                   |
| Transformation             | ✓                      | dbt-core                            |
| Query Federation           | ✓                      | Trino                               |
| Embedded Database          | ✓                      | DuckDB                              |
| Data Lake                  | ✓                      | MinIO                               |
| Workflow Orchestration     | ✓                      | Airflow · Dagster                   |
| Metadata / Governance      | ✓                      | OpenMetadata                        |
| Data Lineage               | ✓                      | OpenLineage                         |
| BI Dashboards              | ✓                      | Superset · Metabase · Grafana       |
| API-First Analytics        | ✓                      | Cube · Superset                     |
| Self-Hosting               | Varies                 | ✓                                   |
| Source Code Access         | Varies                 | ✓                                   |

---

## How to Contribute

1. Fork the repository.

2. Add or edit entries in `README.md` following the existing format.

3. Include the official website or GitHub repository.

4. Clearly identify whether the project is **SaaS/Hosted**, **Open Source**, **Embedded BI**, **Dashboarding**, **Semantic Layer**, **Visualization**, **Data Platform**, or a **Supporting Building Block**.

5. Prefer actively maintained open-source repositories.

6. Include the project's license when known.

7. Distinguish complete embedded analytics platforms from visualization libraries and backend infrastructure.

8. Add new self-hosted embedded analytics platforms.

9. Add open-source dashboard embedding SDKs.

10. Add semantic layers suitable for customer-facing analytics.

11. Add projects supporting multi-tenancy, row-level security and white-labeling.

12. Add new visualization and dashboard-building frameworks.

13. Submit a pull request with a short explanation of the addition or update.

⭐ **Star the repository if you find it useful!**

---

## Disclaimer

* This repository is a **curated directory**, not a ranking or endorsement of any particular product.
* Commercial products and features change frequently; verify current capabilities, pricing, licensing and integrations with the vendor.
* Open-source projects vary substantially in maturity, maintenance activity, documentation, scalability and production readiness.
* A project such as **Cube Core, Apache Superset or Metabase** can provide an important foundation for embedded analytics, but a complete commercial embedded-analytics platform may include additional proprietary functionality around authentication, tenant management, white-labeling, support, governance and enterprise controls.
* Visualization libraries such as **ECharts, D3.js and Vega** are not complete embedded BI platforms by themselves.
* Semantic layers such as **Cube Core** provide the analytical/business-logic layer but do not replace the entire customer-facing dashboard experience.
* Multi-tenant analytics requires careful implementation of authentication, authorization, row-level security and data isolation.
* Embedded analytics can expose sensitive customer data; review security, privacy, tenant isolation and access-control requirements before deployment.
* Always review the license of each open-source project before using it commercially.
* Project links, features and availability may change over time.

---

**Made for SaaS companies, developers, data teams, product teams & builders exploring the open-source embedded analytics ecosystem.**
**Let's make customer-facing analytics more programmable, composable and self-hostable.**
