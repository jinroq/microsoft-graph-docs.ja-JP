---
title: Microsoft Graph Security API を使用する
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: 042c63cfee833a1f9c7493a9e35a6bbb8eb2fbaa
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643088"
---
# <a name="use-the-microsoft-graph-security-api"></a>Microsoft Graph Security API を使用する

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph Security API には、Microsoft とエコシステム パートナーのセキュリティ ソリューションを統合するための統一されたインターフェイスとスキーマが備わっています。 これにより、お客様は、増加するサイバー脅威に対するセキュリティ操作と優れた防御を効率的に行うことができます。 Security API をフェデレーション セキュリティ集約サービスとして使用することにより、オンボードのセキュリティ プロバイダーすべてに対してクエリを発行し、回答の集約情報を得ることができます。 Microsoft Graph Security API を使用して以下の処理を行うアプリケーションを構築できます。

- 複数のソースからのセキュリティの警告を統合し、関連付ける
- コンテキスト データをロック解除し、調査について通知する
- 効率を上げるためにセキュリティ操作を自動化する
- 予防的なリスク管理を可能にするため、セキュリティ データを可視化する

Microsoft Graph Security API には以下の主要なエンティティが含まれています。

## <a name="alerts"></a>アラート

アラートは、Microsoft またはパートナーのセキュリティ ソリューションが識別し、アクションまたは通知のためのフラグが設定された、お客様のテナント内における潜在的なセキュリティ問題です。 Microsoft Graph Security [アラート](alert.md) エンティティを使用すると、統合されたすべてのソリューション内のセキュリティ問題を統一して合理化できます。 これにより、アプリケーション側でも、アラートとコンテキストを関連付け、脅威保護や対応能力を向上できます。 その結果、インシデントの調査時間と解決までの時間が短縮され、セキュリティ操作の効率性が上がります。 アラート更新機能を利用すると、[アラート](alert.md) エンティティを更新することによって Microsoft Graph Security API に統合される各種セキュリティ製品とサービスにおいて特定のアラート状態を同期できます。

Microsoft Graph Security 統合ソリューションは、以下のセキュリティ プロバイダーからのアラートを受信します。

- [Azure Security Center](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft Cloud Application Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Windows Defender Advanced Threat Protection](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(プレビュー)**
- Microsoft Intune **(プライベート プレビュー)**
- Office 365 **(準備中)**
- Azure Advanced Threat Protection **(準備中)**
- Palo Alto Networks App Framework などのパートナー ソリューション

> **注:** Microsoft Graph Security エコシステムに新しいプロバイダーが継続的にオンボードされています。

## <a name="secure-score-preview"></a>セキュア スコア (プレビュー)

[Microsoft セキュア スコア](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358)は、セキュリティ ポートフォリオを可視化し、その方法を向上させるためのセキュリティ分析ソリューションです。 単一のスコアを使用することによって、Microsoft ソリューションにおいてリスクを軽減するために実行した事柄についてより良く把握できます。 また、自分のスコアを他の組織のスコアと比較したり、スコアが時間とともにどのように変化する傾向があるかも理解できます。 Microsoft Graph Security [secureScore](securescores.md) と [secureScoreControlProfiles](securescorecontrolprofiles.md) のエンティティは、ほぼ最大限のセキュリティ機能を確保しながら、組織のセキュリティと生産性のニーズに関して平衡を保つのに役立ちます。 また、セキュリティ機能を採用した後にスコアがどのように変化するかも予想できます。

## <a name="common-use-cases"></a>一般的なユース ケース

Microsoft Graph Security API の操作で最も一般的な要求の一部を以下に取り上げます。

| **ユース ケース**   | **REST リソース** | **Graph エクスプローラーで試す** |
|:---------------|:--------|:----------|
| アラートを一覧表示する | [アラートの一覧表示](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| アラートを更新する | [アラートの更新](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|セキュリティ スコアを一覧表示する|[secureScores の一覧表示](../api/securescores-list.md) (プレビュー)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|セキュア スコア制御プロファイルを一覧表示する|[secureScoreControlProfiles の一覧表示](../api/securescorecontrolprofiles-list.md) (プレビュー)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|セキュア スコア制御プロファイルを更新する|[secureScoreControlProfiles の更新](../api/securescorecontrolprofiles-update.md) (プレビュー)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Microsoft Graph [webhook](/graph/webhooks) を使用すると、Microsoft Graph Security エンティティの更新に関する通知をサブスクライブして受信できます。

## <a name="next-steps"></a>次の手順

Microsoft Graph Security API は、Microsoft およびパートナーの各種セキュリティ ソリューションを活用するための新しい手段となります。 以下の手順に従って開始しましょう。

- [アラート](alert.md)、[secureScore](securescores.md) (プレビュー)、[secureScoreControlProfiles](securescorecontrolprofiles.md) (プレビュー) について詳しく調査します。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試します。 **[サンプル クエリ]** で、**[サンプルをさらに表示]** を選択してセキュリティ カテゴリを **[オン]** に設定します。
- エンティティ変更時の[通知のサブスクライブと受信](/graph/webhooks)を試します。

さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。

## <a name="see-also"></a>関連項目

コードを作成し、以下の Microsoft Graph Security API サンプルに投稿できます。

- [ASP.NET (C#) サンプル](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python サンプル](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) サンプル](https://github.com/microsoftgraph/nodejs-security-sample)

以下のコミュニティに参加できます。

- [技術コミュニティに参加する](https://aka.ms/graphsecuritycommunity)
- [StackOverflow についてディスカッションする](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
