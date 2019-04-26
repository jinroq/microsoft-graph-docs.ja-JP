---
title: Microsoft Graph Security API の警告と SIEM の統合
description: Microsoft Graph Security API は、単一の REST エンドポイントを介して、すべての Microsoft セキュリティ製品 (Microsoft Graph Security プロバイダーと呼ばれる) から出力されるセキュリティの警告を管理する機能を提供します。 組織によっては、Azure Monitor によって Azure 固有のログ データが SIEM ソリューションに既に取り込まれている場合があります。 統合を簡略化するため、Microsoft Graph のセキュリティ API から使用できるセキュリティの警告は、ユーザーが自分のサブスクリプションに対して Azure Monitor 経由でプロビジョニングすることもできます。 Azure Monitor と SIEM ソリューションの統合が既に構成されている組織では、組織のセキュリティの警告を Azure Monitor で利用できる既存のデータに加えて簡単にストリーミングできます。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 92a5416f68ccbc6fbbd0001c473f1daf2fe21187
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556931"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Microsoft Graph Security API の警告と SIEM の統合

Microsoft Graph Security API は、単一の REST エンドポイントを介して、すべての Microsoft セキュリティ製品 (Microsoft Graph Security プロバイダーと呼ばれる) から出力されるセキュリティの警告を管理する機能を提供します。 組織によっては、Azure Monitor によって Azure 固有のログ データが SIEM ソリューションに既に取り込まれている場合があります。 統合を簡略化するため、Microsoft Graph のセキュリティ API から使用できるセキュリティの警告は、ユーザーが自分のサブスクリプションに対して Azure Monitor 経由でプロビジョニングすることもできます。 Azure Monitor と SIEM ソリューションの統合が既に構成されている組織では、組織のセキュリティの警告を Azure Monitor で利用できる既存のデータに加えて簡単にストリーミングできます。

次のセキュリティ プロバイダーからのアラートは、SIEM 統合により入手できます。

- [Azure Security Center](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts)
- [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(プレビュー)**
- [Azure Advanced Threat Protection](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) **(プレビュー)**
- [Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(プレビュー)**

Azure Monitor は、複数の SIEM 製品へのコネクタをサポートします。 サポートされている SIEM 製品のリストについては、[イベント ハブへの監視データの送信](https://docs.microsoft.com/ja-JP/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)を参照してください。 現在、Microsoft Graph Security API の統合は、[Splunk](https://splunkbase.splunk.com/) と [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) で使用できます。

特定の SIEM ソリューションに対する Microsoft Graph Security API の統合については、次を参照してください。

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
