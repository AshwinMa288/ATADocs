---
# required metadata

title: Tag sensitive accounts with Azure ATP
description: Describes how to tag sensitive accounts using Azure Advanced Threat Protection (ATP)
keywords:
author: shsagir
ms.author: shsagir
manager: shsagir
ms.date: 02/16/2020
ms.topic: conceptual
ms.collection: M365-security-compliance
ms.service: azure-advanced-threat-protection
ms.assetid: 43e57f87-ca85-4922-8ed0-9830139fe7cb

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
ms.reviewer: itargoet
ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom:

---

# Working with sensitive accounts

## Sensitive entities

The following list of groups are considered **Sensitive** by Azure ATP. Any entity that is a member of one of these groups is considered sensitive:

- Administrators
- Power Users
- Account Operators
- Server Operators
- Print Operators
- Backup Operators
- Replicators
- Network Configuration Operators
- Incoming Forest Trust Builders
- Domain Admins
- Domain Controllers
- Group Policy Creator Owners
- read-only Domain Controllers
- Enterprise Read-only Domain Controllers
- Schema Admins
- Enterprise Admins
- Microsoft Exchange Servers

  > [!NOTE]
  > Until September, 2018, Remote Desktop Users were also automatically considered Sensitive by Azure ATP. Remote Desktop entities or groups added after this date are no longer automatically marked as sensitive while Remote Desktop entities or groups added before this date may remain marked as Sensitive. This Sensitive setting can now be changed manually.

In addition to these groups, Azure ATP identifies the following high value asset servers and automatically tags them as **Sensitive**:

- Certificate Authority Server
- DHCP Server
- DNS Server
- Microsoft Exchange Server

## Tagging sensitive accounts

In addition to these groups, you can manually tag groups or accounts as sensitive to enhance detections. This is important because Some Azure ATP detections, such as sensitive group modification detection and lateral movement paths, rely on which groups and accounts are considered sensitive. You can manually tag other users or groups as sensitive, such as board members, company executives, director of sales, etc., and Azure ATP considers them sensitive.

1. In the Azure ATP portal, click the **Configuration** cog in the menu bar.

1. Under **Detection** click **Entity tags**.

    ![Azure ATP entity tags](media/entity-tags.png)

1. In the **Sensitive** section, type the name of the **Sensitive accounts** and **Sensitive groups** and then click **+** sign to add them.

    ![Azure ATP sensitive account sample](media/sensitive-account-sample.png)

1. Click **Save**.

## See also

- [Working with suspicious activities](working-with-suspicious-activities.md)
- [Check out the Azure ATP forum!](https://aka.ms/azureatpcommunity)
