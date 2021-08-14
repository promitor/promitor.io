---
title: "Frequently Asked Questions"
subtitle: ""
# meta description
description: "This is meta description"
draft: false
---


{{< faq "Are multi-dimensional metrics supported?" >}}
Yes, every scraper supports scraping multi-dimensional metrics except for
Azure Storage queues.

You can configure the dimension you are interested in via
`azureMetricConfiguration.dimension.Name`, for more information see
our ['Metric Configuration' page](/configuration/v1.x/metrics/#metrics).

However, you can only use it with metrics in Azure Monitor that support this,
for a complete overview we recommend reading the
[official documentation](https://docs.microsoft.com/en-us/azure/azure-monitor/platform/metrics-supported).
{{</ faq >}}

{{< faq "Is scraping multiple subscriptions supported?" >}}
No, we do not support scraping multiple subscriptions as of today as we consider that to be a security boundary.

However, you can deploy multiple instances of Promitor that each scrape another subscription.

We have it on [our backlog](https://github.com/tomkerkhove/promitor/issues/761) to see if there is
 enough demand for it, feel free to give a :+1:. If that is the case, we will reconsider this limitation.
{{</ faq >}}

{{< faq "What Azure clouds are supported?" >}}
We support `Global` (default), `China`, `UsGov` & `Germany` Azure clouds.

This can be configured in the metric configuration under `azureMetadata`.

For more information see our ['Metric Configuration' page](https://promitor.io/configuration/v2.x/metrics/#metrics).
{{</ faq >}}

{{< faq "Why do Azure Blob & File Storage only report account-level information?" >}}
Azure Monitor currently only provides account-level metrics which we can serve.

As part of [#450](https://github.com/tomkerkhove/promitor/issues/450) &
 [#446](https://github.com/tomkerkhove/promitor/issues/446) we plan to provide the capability to have more granular information.
{{</ faq >}}

{{< faq "What Helm version is supported?" >}}
Promitor supports deployments with **Helm v3.0** for all versions.
{{</ faq >}}

{{< faq "What operating systems are supported?" >}}
We support running on both Linux & Windows platforms.
{{</ faq >}}

{{< faq "How does Promitor handle deleted resources?" >}}
The approach depends if you are using declarative metrics or resource discovery but we highly recommend to
 **enable Prometheus metric timestamps** in [our runtime configuration](/configuration/v2.x/runtime/scraper/#prometheus-scraping-endpoint)
  to indicate how old the metric is.

### When using declarative metrics

Promitor will scrape all resources that are configured and report the metrics accordingly. If that resource is deleted,
 we will **still serve the metrics as long as we can until it is no longer available and exceptions will be thrown**.

We **recommend to update the metrics declaration when a resource is deleted** to avoid polluting logs.

### When using resource discovery

Promitor will automatically discover all matching resources which means that **it will automatically scrape metrics for
 new/removed resources**.

Removed resources will immediately stop being scraped by Promitor, but still be reported in Prometheus scrape endpoint.
{{</ faq >}}