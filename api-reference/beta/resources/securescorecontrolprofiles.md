---
title: secureScoreControlProfiles リソースの種類
description: コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524430"
---
# <a name="securescorecontrolprofiles-resource-type"></a>secureScoreControlProfiles リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[secureScoreControlProfiles のリスト](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |プロパティと、secureScoreControlProfiles オブジェクトのメタデータを参照してください。|


## <a name="properties"></a>プロパティ

|名前 |型 |説明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   テナントの GUID の文字列 id。  |
|   controlName |   String  |   コントロールの名前です。 |
|   タイトル   |   String  |   コントロールのタイトルです。   |
| complianceInformation | [complianceInformation](complianceinformation.md)コレクション | 関連付けられているコンプライアンス情報の収集は、スコアのコントロールをセキュリティで保護します。 |
|   controlCategory |   String  |   コントロールのアクションのカテゴリ (アカウント、データ、デバイス、アプリケーション、インフラストラクチャ) です。  |
|   actionType  |   String  |   アクションの種類 (構成、レビュー、動作) を制御します。 |
|   service |   String  |   (Exchange、Sharepoint、Azure AD) のコントロールを所有しているサービスです。 |
|   maxScore |  String  |   現在では、指定した日付の最大のスコアを取得します。   |
|   階層 |  String  |   制御層 (コア、防御の深さ、高度な)。    |
|   userImpact |    String  | コントロール (低、中、高) を実装するためのユーザーへの影響。    |
|   implementationCost |    String  |   Implemmentating コントロール (低、中、高) のリソースのコストです。 |
|   rank |  Int32   |   マイクロソフトのコントロールのレベルを調整します。   |
|   脅威 |   String コレクション   |   コントロールを軽減する脅威の一覧 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、なりすましが行われる)。 |
|   非推奨 |    ブール値 |   コントロールで減価償却されるかどうかを示すためにフラグを設定します。   |
|   改善計画 |   String  |   どのようなコントロールの説明は、改善に役立ちます。 |
|   remediationImpact | String  |   改善のユーザーへの影響の説明です。 |
|   ActionURL | String  |   URL は、コントロールが対象になることです。 |
|   controlStateUpdates |   [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション |    テナントには、コントロールとしてのマークを指定するフラグ (無視して、レビュー、サード ・ パーティ) ([更新](../api/securescorecontrolprofiles-update.md)がサポートされています)。 |

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
