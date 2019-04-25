---
title: securescorecontrolprofiles のリソースの種類
description: テナントのセキュリティスコア (コントロールデータごと) を表します。 既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549175"
---
# <a name="securescorecontrolprofiles-resource-type"></a>securescorecontrolprofiles のリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントのセキュリティスコア (コントロールデータごと) を表します。 既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[secureScoreControlProfiles のリスト](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |securescorecontrolprofiles のオブジェクトのプロパティとメタデータを読み取ります。|


## <a name="properties"></a>プロパティ

|名前 |型 |説明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   テナント ID の GUID 文字列。  |
|   controlName |   String  |   コントロールの名前を指定します。 |
|   title   |   String  |   コントロールのタイトルを指定します。   |
| complianceInformation | [complianceInformation](complianceinformation.md)コレクション | セキュリティで保護されたスコアコントロールに関連付けられているコンプライアンス情報のコレクション |
|   controlcategory |   String  |   コントロールアクションカテゴリ (アカウント、データ、デバイス、アプリ、インフラストラクチャ)。  |
|   actionType  |   String  |   アクションの種類 (Config、Review、Behavior) を制御します。 |
|   service |   String  |   コントロールを所有するサービス (Exchange、Sharepoint、Azure AD)。 |
|   maxscore |  String  |   指定された日付における現在の取得最高スコア。   |
|   層 |  String  |   Control 層 (コア、多層防御、詳細)    |
|   userimpact |    String  | 制御を実装するユーザーへの影響 (低、中、高)。    |
|   implementationCost |    String  |   implemmentating コントロールのリソースコスト (低、中、高)。 |
|   rank |  Int32   |   Microsoft のスタックランキング。   |
|   主 |   String コレクション   |   統制によって軽減される脅威のリスト (accountbreach、datadeletion、dataexのフィルター、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordcracking、phishingOrWhaling、スプーフィング)。 |
|   予定 |    ブール値 |   コントロールが減価償却されているかどうかを示すフラグです。   |
|   修復 |   String  |   修復に役立つコントロールの説明。 |
|   remediationImpact | String  |   修復のユーザーへの影響についての説明。 |
|   actionUrl | String  |   コントロールを actioned できる場所の URL。 |
|   controlstateupdates |   [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション |    テナントがコントロールをマークした場所を示すフラグ (ignore、thirdParty、レビュー済み) ([更新プログラム](../api/securescorecontrolprofiles-update.md)をサポート)。 |

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
