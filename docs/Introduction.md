---
id: introduction
title: Introduction
slug: /
---

SigNoz is an open-source observability tool that helps you monitor your applications and troubleshoot problems. It provides traces, metrics, and logs under a single pane of glass.

With SigNoz, you can do the following:

- Visualise Traces, Metrics, and Logs in a single pane of glass
- Monitor application metrics like p99 latency, error rates for your services, external API calls, and individual endpoints.
- Find the root cause of the problem by going to the exact traces which are causing the problem and see detailed flamegraphs of individual request traces.
- Run aggregates on trace data to get business-relevant metrics
- Filter and query logs, build dashboards and alerts based on attributes in logs
- Monitor infrastructure metrics such as CPU utilization or memory usage
- Record exceptions automatically in Python, Java, Ruby, and Javascript
- Easy to set alerts with DIY query builder


## Get Started

You can either self-host SigNoz or try SigNoz Cloud. Once SigNoz is up and running, you can instrument your application to send data to SigNoz.

<div class="row">
 <article class="col col--6">
    <a class="card margin-bottom--lg padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module cardContainerLink_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" href="/teams/">
      <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" title="SigNoz Cloud">SigNoz Cloud</h2>
      <div class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" title="Learn how to instrument your application">Easy way to get started with SigNoz</div>
    </a>
  </article>
  <article class="col col--6">
    <a class="card margin-bottom--lg padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module cardContainerLink_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" href="/docs/install/">
      <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" title="Self-host SigNoz">Self-host SigNoz</h2>
      <div class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" title="Learn how to install SigNoz ">Learn how to install and self-host SigNoz</div>
    </a>
  </article>
</div>


## How Does SigNoz Work?

SigNoz collects data using <a href = "https://opentelemetry.io/" rel="noopener noreferrer nofollow" target="_blank" >OpenTelemetry</a>, an open-source observability solution. OpenTelemetry is backed by Cloud Native Computing Foundation. The project aims to standardize how we instrument our applications for generating telemetry data(traces, metrics, and logs).

 SigNoz supports all the frameworks and languages supported by OpenTelemetry.  You can find the complete list of supported languages on the <a href = "https://opentelemetry.io/docs/instrumentation/" rel="noopener noreferrer nofollow" target="_blank" >instrumentation</a> page of the OpenTelemetry documentation.

Once you instrument your application with OpenTelemetry, you can send the data to SigNoz for storage, analysis, and visualization.

### Architecture

![acrhitecture-diagram-clickhouse](../static/img/architecture-signoz-clickhouse.svg)
SigNoz includes the following components:
- **OpenTelemetry Collector**: Collects telemetry data from your services and applications.
- **ClickHouse**: An open-source, high performance columnar OLAP database management system. 
- **Query Service**: The interface between the front-end and ClickHouse
- **Frontend**: The user interface, built in ReactJS and TypeScript.

To learn more about the architecture of SigNoz, see the [Architecture](/docs/architecture) page.

## Use SigNoz

The topics in this section provide details on using SigNoz to monitor your application.

<div class="row">
 
  <article class="col col--6">
    <a class="card margin-bottom--lg padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module cardContainerLink_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" href="/docs/tutorials">
      <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" title="1. Tutorials">1. Tutorials</h2>
      <div class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" title="Tutorials about monitoring your applications and infrastructure<">Tutorials about monitoring your applications and infrastructure</div>
    </a>
  </article>
  <article class="col col--6">
    <a class="card margin-bottom--lg padding--lg cardContainer_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module cardContainerLink_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" href="/docs/operate">
      <h2 class="text--truncate cardTitle_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" title="2. Operate">2. Operate</h2>
      <div class="text--truncate cardDescription_node_modules-@docusaurus-theme-classic-lib-next-theme-DocCard-styles-module" title="This section explains how to manage SigNoz">This section explains how to manage SigNoz</div>
    </a>
  </article>

</div>

