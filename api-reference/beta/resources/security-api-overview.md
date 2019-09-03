---
title: Microsoft Graph Security API を使用する
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Priority
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 37645217c9ef410dafa9eea0c9b8a9156c4c868f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965244"
---
# <a name="use-the-microsoft-graph-security-api"></a>Microsoft Graph Security API を使用する

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|[Microsoft Defender Advanced Threat Protection](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/attack-simulations)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Advanced Threat Protection](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) *| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|Office 365 <ul><li> [Default](https://docs.microsoft.com/ja-JP/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud App Security](https://docs.microsoft.com/ja-JP/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(プレビュー)**| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(プレビュー)**| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Palo Alto Networks](https://docs.paloaltonetworks.com/pan-os/9-0/pan-os-web-interface-help/monitor/monitor-logs/log-types.html)| <p align="center">&#x2713;</p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [ファイルの問題](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
> **注:** Microsoft Graph Security エコシステムに新しいプロバイダーが継続的に加わっています。 新しいプロバイダーにサポートを要請したり、既存のプロバイダーからのサポートを拡張したりするよう要請するには、[Microsoft Graph セキュリティ GitHub リポジトリに問題についてのファイルを登録](https://github.com/microsoftgraph/security-api-solutions/issues/new)します。

\*Microsoft Cloud App Security 統合を使用して Azure Advanced Threat Protection アラートを利用できます。 つまり、[統合された SecOps プレビュー プログラム](https://techcommunity.microsoft.com/t5/Enterprise-Mobility-Security/Unified-SecOps-Investigation-for-Hybrid-Environments/ba-p/360850)に参加済みで、Azure Advanced Threat Protection が Microsoft Cloud App Security に接続されている場合のみ、Azure Advanced Threat Protection アラートを取得できます。

## <a name="threat-indicators-preview"></a>脅威インジケーター (プレビュー)

脅威インジケーター (侵害のインジケーター (IoCs) とも呼ばれる) は、悪意のあるファイル、URL、ドメイン、IP アドレスなどの、既知の脅威に関するデータを表します。 お客様は、内部のさまざまな脅威インテリジェンスからインジケーターを作成したり、脅威インテリジェンス コミュニティ、ライセンスを取得したフィード、およびその他のソースからインジケーターを取得したりすることができます。 これらのインジケーターは、関連する脅威から保護するためにさまざまなセキュリティ ツールで使用されます。

Microsoft Graph セキュリティ [tiIndicators](tiindicator.md) エンティティにより、脅威インジケーターを Microsoft のセキュリティ ソリューションにフィードし、悪意のある活動をブロックしたり警告するようにしたり、組織に関連しないと判断されるインジケーターに対するアクションを行わないようにしたりできます。 インジケーターを送信する際は、インジケーターを利用する Microsoft のソリューションとそのインジケーターに対して実行されるアクションの両方が指定されます。

[tiIndicator](tiindicator.md) エンティティをアプリケーションに統合するか、次の統合された脅威インテリジェンス プラットフォーム (TIP) のいずれかを使用できます。

- [Palo Alto Networks MineMeld Threat Intelligence Sharing](https://www.paloaltonetworks.com/products/secure-the-network/subscriptions/minemeld)
- [TI サンプル](https://aka.ms/tipmispsample) により利用できる [MISP Open Source Threat Intelligence Platform](http://www.misp-project.org/)

Microsoft Graph Security API 経由で送信された脅威インジケーターは現時点で、[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/overview) (プレビュー) で利用でき、脅威インジケーターをログ データを関連付けて悪意のあるアクティビティについてのアラートを取得できます。 Azure Firewall などの他の Microsoft のセキュリティ サービスのサポートは間もなく提供されます。

## <a name="security-actions-preview"></a>セキュリティ アクション (プレビュー)

Microsoft Graph のセキュリティの [securityAction](securityaction.md) エンティティを使用して、脅威から保護するためのアクションをただちに実行します。 セキュリティ アナリストが、悪意のあるファイル、URL、ドメイン、IP アドレスなどの新しいインジケーターを発見した場合、Microsoft のセキュリティ ソリューションでそれらに対する保護をすぐに有効にできます。 特定のプロバイダーのアクションを呼び出し、実行されるすべての操作を表示し、必要な場合は操作を取り消します。 [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) でセキュリティ アクションを実行し、アラートに表示されるプロパティまたは調査中に特定されるプロパティを使用して Windows のエンドポイントの悪意のあるアクティビティをブロックします。

  > **注:** 現在、セキュリティ アクションでサポートされているのは、アプリケーションのアクセス許可のみです。

## <a name="secure-score"></a>セキュリティ スコア

[Microsoft セキュア スコア](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358)は、セキュリティ ポートフォリオを可視化し、その方法を向上させるためのセキュリティ分析ソリューションです。 単一のスコアを使用することによって、Microsoft ソリューションにおいてリスクを軽減するために実行した事柄についてより良く把握できます。 また、自分のスコアを他の組織のスコアと比較したり、スコアが時間とともにどのように変化する傾向があるかも理解できます。 Microsoft Graph Security [secureScore](securescores.md) と [secureScoreControlProfile](securescorecontrolprofiles.md) のエンティティは、ほぼ最大限のセキュリティ機能を確保しながら、組織のセキュリティと生産性のニーズに関して平衡を保つのに役立ちます。 また、セキュリティ機能を採用した後にスコアがどのように変化するかも予想できます。

## <a name="common-use-cases"></a>一般的なユース ケース

Microsoft Graph Security API の操作で最も一般的な要求の一部を以下に取り上げます。

| **ユース ケース**   | **REST リソース** | **Graph エクスプローラーで試す** |
|:---------------|:--------|:----------|
| アラートを一覧表示する | [アラートの一覧表示](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| アラートを更新する | [警告の更新](../api/alert-update.md) </br> [複数のアラートを更新する](../api/alert-updatealerts.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) </br> [https://graph.microsoft.com/beta/security/alerts/updateAlerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/updateAlerts&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| セキュリティ アクションを取得する | [セキュリティ アクションを取得する](../api/securityaction-get.md) (プレビュー)|[https://graph.microsoft.com/beta/security/securityActions/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|セキュリティ アクションを一覧表示する| [セキュリティ アクションを一覧表示する](../api/securityactions-list.md) (プレビュー)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|セキュリティ アクションを作成する|[セキュリティ アクションを作成する](../api/securityactions-post.md) (プレビュー)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|セキュリティ アクションをキャンセルする|[セキュリティ アクションをキャンセルする](../api/securityaction-cancelsecurityaction.md) (プレビュー)| [https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}/cancelSecurityAction&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|TI インジケーターを取得する|[tiIndicator を取得する](../api/tiindicator-get.md) (プレビュー)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|TI インジケーターを一覧表示する | [TI インジケーターを一覧表示する](../api/tiindicators-list.md) (プレビュー) | [https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|TI インジケーターを作成する|[TI インジケーターを作成する](../api/tiindicators-post.md) (プレビュー)|[https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|TI インジケーターを送信する|[TI インジケーターを送信する](../api/tiindicator-submittiindicators.md) (プレビュー)| [https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/submitTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|TI インジケーターを更新する|[tiIndicator を更新する](../api/tiindicator-update.md) (プレビュー) </br>[複数の tiIndicator を更新する](../api/tiindicator-updatetiindicators.md) (プレビュー)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) </br>[https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/updateTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|TI インジケーターを削除する|[tiIndicator を削除する](../api/tiindicator-delete.md) (プレビュー) </br>[複数の tiIndicator を削除する](../api/tiindicator-deletetiindicators.md) (プレビュー) </br>[externalId で tiIndicator を削除する](../api/tiindicator-deletetiindicatorsbyexternalid.md) (プレビュー)| DELETE </br>[https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=DELETE&version=beta&GraphUrl=https://graph.microsoft.com) </br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)</br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicatorsByExternalId&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|セキュリティ スコアを一覧表示する|[secureScores のリスト](../api/securescores-list.md)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|セキュリティ スコアの制御プロファイルを一覧表示する|[secureScoreControlProfiles のリスト](../api/securescorecontrolprofiles-list.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|セキュア スコア制御プロファイルを更新する|[secureScoreControlProfiles の更新](../api/securescorecontrolprofiles-update.md)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Microsoft Graph [webhook](/graph/webhooks) を使用すると、Microsoft Graph Security API エンティティの更新に関する通知をサブスクライブして受信できます。

## <a name="next-steps"></a>次のステップ

Microsoft Graph Security API は、Microsoft およびパートナーの各種セキュリティ ソリューションを活用するための新しい手段となります。 以下の手順に従って開始しましょう。

- [アラート](alert.md)、[tiIndicator](tiindicator.md) (プレビュー)、[securityAction](securityaction.md) (プレビュー)、[secureScore](securescores.md)、[secureScoreControlProfiles](securescorecontrolprofiles.md)について詳しく調査します。
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
