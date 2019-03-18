---
title: Microsoft Graph Security API を使用する
description: Microsoft Graph Security API には、Microsoft とエコシステム パートナーのセキュリティ ソリューションを統合するための統一されたインターフェイスとスキーマが備わっています。 これにより、お客様は、増加するサイバー脅威に対するセキュリティ操作と優れた防御を効率的に行うことができます。 Security API をフェデレーション セキュリティ集約サービスとして使用することにより、オンボードのセキュリティ プロバイダーすべてに対してクエリを発行し、回答の集約情報を得ることができます。 Microsoft Graph Security API を使用して以下の処理を行うアプリケーションを構築できます。
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: bd208067c2194766bb5f3d93d0caa21be086dca0
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644266"
---
# <a name="use-the-microsoft-graph-security-api"></a>Microsoft Graph Security API を使用する

Microsoft Graph Security API には、Microsoft とエコシステム パートナーのセキュリティ ソリューションを統合するための統一されたインターフェイスとスキーマが備わっています。 これにより、お客様は、増加するサイバー脅威に対するセキュリティ操作と優れた防御を効率的に行うことができます。 Microsoft Graph Security API は、すべての稼働中のセキュリティ プロバイダーへのクエリを統合し対応を集計します。 Microsoft Graph Security API を使用して以下の処理を行うアプリケーションを構築できます。

- 複数のソースからのセキュリティの警告を統合し、関連付ける
- コンテキスト データをロック解除し、調査について通知する
- セキュリティ タスク、ビジネス プロセス、ワークフロー、レポート作成を自動化する
- Microsoft 製品に対してカスタマイズされた検出の脅威インジケーターを送信する
- 新たな脅威に対応するアクションを呼び出す
- 予防的なリスク管理を可能にするため、セキュリティ データを可視化する

Microsoft Graph Security API には以下の主要なエンティティが含まれています。

## <a name="alerts"></a>アラート

アラートは、Microsoft またはパートナーのセキュリティ ソリューションが識別し、アクションまたは通知のためのフラグが設定された、お客様のテナント内における潜在的なセキュリティ問題です。 Microsoft Graph Security [アラート](alert.md) エンティティを使用すると、統合されたすべてのソリューション内のセキュリティ問題の管理を統一して合理化できます。 これにより、アプリケーション側でも、アラートとコンテキストを関連付け、脅威保護や対応能力を向上できます。 アラート更新機能を利用すると、[アラート](alert.md) エンティティを更新することによって Microsoft Graph Security API に統合される各種セキュリティ製品とサービスにおいて特定のアラート状態を同期できます。

次のプロバイダーからのアラートは、Microsoft Graph Security API を使って利用できます。 GET アラート、PATCH アラート (更新プログラムは Microsoft Graph Security API で利用できますが、プロバイダーの管理操作環境では公開されない)、サブスクライブ (webhooks 経由) のサポート状況を次の表に示します。

| セキュリティ プロバイダー | <p align="center">GET アラート</p>| <p align="center">PATCH アラート</p>| <p align="center">アラートへのサブスクライブ</p>|
|:------------------|:---------|:-----------|:------------------|
|[Azure Security Center](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
| [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts) | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Windows Defender Advanced Threat Protection](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Advanced Threat Protection](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories)| <p align="center">&#x2713;</p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|Office 365 <ul><li> [Default](https://docs.microsoft.com/ja-JP/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud App Security](https://docs.microsoft.com/ja-JP/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(プレビュー)**| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(プレビュー)**| <p align="center">&#x2713;</p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Palo Alto Networks](https://docs.paloaltonetworks.com/pan-os/9-0/pan-os-web-interface-help/monitor/monitor-logs/log-types.html)| <p align="center">&#x2713;</p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
> **注:** Microsoft Graph Security エコシステムに新しいプロバイダーが継続的に加わっています。 新しいプロバイダーにサポートを要請したり、既存のプロバイダーからのサポートを拡張したりするよう要請するには、[Microsoft Graph セキュリティ GitHub リポジトリに問題についてのファイルを登録](https://github.com/microsoftgraph/security-api-solutions/issues/new)します。

## <a name="common-use-cases"></a>一般的なユース ケース

Microsoft Graph Security API の操作で最も一般的な要求の一部を以下に取り上げます。

| **ユース ケース**   | **REST リソース** | **Graph エクスプローラーで試す** |
|:---------------|:--------|:----------|
| アラートを一覧表示する | [アラートの一覧表示](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| アラートを更新する | [警告の更新](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

Microsoft Graph [webhook](/graph/webhooks) を使用すると、Microsoft Graph Security エンティティの更新に関する通知をサブスクライブして受信できます。

## <a name="resources"></a>リソース

コードを作成し、以下の Microsoft Graph Security API サンプルに投稿できます。

- [ASP.NET (C#) サンプル](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python サンプル](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) サンプル](https://github.com/microsoftgraph/nodejs-security-sample)

以下のコミュニティに参加できます。

- [技術コミュニティに参加する](https://aka.ms/graphsecuritycommunity)
- [StackOverflow についてディスカッションする](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>次のステップ

Microsoft Graph Security API は、Microsoft およびパートナーの各種セキュリティ ソリューションを活用するための新しい手段となります。 以下の手順に従って開始しましょう。

- [アラート](alert.md)にドリルダウンします。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。 **[サンプル クエリ]** で、**[サンプルをさらに表示]** を選択してセキュリティ カテゴリを **[オン]** に設定します。
- エンティティ変更時の[通知のサブスクライブと受信](/graph/webhooks)を試します。

さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。

## <a name="see-also"></a>関連項目

以下の Microsoft Graph Security API サンプルに、[コードを作成して投稿します](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md)。

- [ASP.NET (C#) サンプル](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python サンプル](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) サンプル](https://github.com/microsoftgraph/nodejs-security-sample)
- [PowerShell サンプル](https://aka.ms/graphsecuritypowershellsample)
- [その他のサンプルまたは新しいサンプルの投稿](https://aka.ms/graphsecurityapicode)

Microsoft Graph Security API に接続するその他のオプション調べます。

- [Logic Apps、Flow、PowerApps 用の Microsoft Graph セキュリティ コネクタ](https://aka.ms/graphsecurityconnectors)
- [Power BI 用の Microsoft Graph セキュリティ コネクタ](https://aka.ms/graphsecuritypowerbiconnectordoc)
- [Jupyter ノートブックのサンプル](https://aka.ms/graphsecurityjupyternotebooks)

以下のコミュニティに参加できます。

- [技術コミュニティに参加する](https://aka.ms/graphsecuritycommunity)
- [StackOverflow についてディスカッションする](https://stackoverflow.com/questions/tagged/microsoft-graph-security)