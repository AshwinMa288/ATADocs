---
# required metadata

title: Azure Advanced Threat Protection identity security posture assessments
description: This article provides an overview of Azure ATP's identity security posture assessment reports.
keywords:
author: shsagir
ms.author: shsagir
manager: shsagir
ms.date: 09/16/2019
ms.topic: how-to
ms.collection: M365-security-compliance
ms.service: azure-advanced-threat-protection
ms.assetid: 71b15bd9-3183-4e24-b18a-705023ccc313

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: itargoet
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Azure ATP's identity security posture assessments

> [!IMPORTANT]
> Threat protection product names from Microsoft are changing. Read more about this and other updates [here](https://www.microsoft.com/security/blog/?p=91813).  We’ll be updating names in products and in the docs in the near future.

Typically, organizations of all sizes have limited visibility into whether or not their on-premises apps and services could introduce a security vulnerability to their organization. The problem of limited visibility is especially true with regards to use of unsupported or outdated components.

While your company may invest significant time and effort on hardening identities and identity infrastructure (such as Active Directory, Active Directory Connect) as an on-going project, it is easy to remain unaware of common misconfigurations and use of legacy components that represent one of the greatest threat risks to your organization. Microsoft security research reveals that most identity attacks utilize common misconfigurations in Active Directory and continued use of legacy components (such as NTLMv1 protocol) to compromise identities and successfully breach your organization. To combat this effectively, Azure ATP now offers proactive identity security posture assessments to detect and suggest improvement actions across your on-premise Active Directory configurations.

## What do Azure ATP identity security posture assessments provide?

- Detections and contextual data on known exploitable components and misconfigurations, along with relevant paths for remediation.
- Azure ATP detects not only suspicious activities, but also actively monitors your on-premise identities and identity infrastructure for weak spots, using the existing Azure ATP sensor.
- Accurate assessment reports of your current organization security posture, enabling quick response and effect monitoring in a continuous cycle.

## How do I get started?

### Access

Azure ATP security assessments are available using the Microsoft Cloud App Security portal after turning on the Azure ATP integration. To learn how to integrate Azure ATP into Cloud App Security, see [Azure ATP integration](/cloud-app-security/aatp-integration).

### Licensing

Accessing Azure ATP security assessment reports in Cloud App Security do not require a Cloud App Security license, only an Azure ATP license is required.

## Access Azure ATP using Cloud App Security

See the [Cloud App Security quick start](/cloud-app-security/getting-started-with-cloud-app-security) to familiarize yourself with the basics of using the Cloud App Security portal.

**Identity security posture assessments**

Azure ATP offers the following identity security posture assessments. Each assessment is a downloadable report with instructions for use and tools for building an action plan to remediate or resolve.

**Assessment reports**

- [Domain controllers with Print Spooler service available](cas-isp-print-spooler.md)
- [Dormant entities in sensitive groups](cas-isp-dormant-entities.md)
- [Entities exposing credentials in clear text](cas-isp-clear-text.md)
- [Microsoft LAPS usage](cas-isp-laps.md)
- [Legacy protocols usage](cas-isp-legacy-protocols.md)
- [Riskiest lateral movement paths (LMP)](cas-isp-riskiest-lmp.md)
- [Unmonitored domain controllers](cas-isp-unmonitored-domain-controller.md)
- [Unsecure account attributes](cas-isp-unsecure-account-attributes.md)
- [Unsecure Kerberos delegation](cas-isp-unconstrained-kerberos.md)
- [Unsecure SID History attributes](cas-isp-unsecure-sid-history-attribute.md)
- [Weak cipher usage](cas-isp-weak-cipher.md)

To access identity security posture assessments:

1. Open the **Microsoft Cloud App Security** portal.
    ![Access Azure ATP identity security posture reports in Cloud App Security](media/atp-cas-isp-report-1.png)
1. Select **Investigate** from the left menu, then click **Identity security posture** from the drop-down menu.
1. Click the identity security posture assessment you wish to review from the **Security assessment reports** list that opens.

## Next steps

- [Learn more about using Cloud App Security with Azure ATP](activities-filtering-mcas.md)
- [Check out the Azure ATP forum!](https://aka.ms/azureatpcommunity)