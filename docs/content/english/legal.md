---
title: "Legal"
subtitle: "Learn about the legal implications of Promitor"
# meta description
description: "Legal information related to Promitor"
draft: false
---

## Use of Promitor

Promitor is a product to bring your Azure metrics to where you need them.

It is offered as a free product and is not supported by Microsoft, however, read about Promitor's support policy [here](https://github.com/tomkerkhove/promitor/blob/master/SUPPORT.md).

## Tracking

### User agent

Promitor includes a user-agent for all requests sent to Microsoft APIs that include information related to the type of agent and its version.

This is done to help Microsoft support in case of incidents and track usage of Promitor based on anonymized data. At no point is any personal information collected nor sold to external parties.

### Image Pulling

Images are stored on GitHub Container Registry which provide anonymized pull information which is anonymized by GitHub. This information is public and not used for any other purpose than adoption measurement and managed by GitHub.

End-users that are installing Promitor through our [Helm chart](https://github.com/promitor/charts) are pulling Promitor's images from GitHub Container Registry through [Scarf](http://scarf.sh/)'s gateway.

It allows Promitor to be more decoupled from the physical container registry and use a custom domain under the `promitor.io` domain. Scarf does, however, provide metadata around image pulls solely to Promitor maintainers to measure adoption and be aware of where end-users are across the globe.

End-users who do not want to use Scarf's gateway can opt-in to pull images directly from GitHub Container Registry by changing the image during Helm installation.

Learn more about Scarf's gateway [here](https://about.scarf.sh/scarf-gateway).
