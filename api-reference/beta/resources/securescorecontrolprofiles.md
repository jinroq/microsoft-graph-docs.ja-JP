---
title: secureScoreControlProfiles リソースの種類
description: コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。
ms.openlocfilehash: e02c9ae3b1431b131576e2e0e115377dd3480bc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071878"
---
# <a name="securescorecontrolprofiles-resource-type"></a>secureScoreControlProfiles リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[リスト secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |プロパティと、secureScoreControlProfiles オブジェクトのメタデータを参照してください。|


## <a name="properties"></a>プロパティ

|名前 |型 |説明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   テナントの GUID の文字列 id。  |
|   controlName |   String  |   コントロールの名前です。 |
|   タイトル   |   String  |   コントロールのタイトルです。   |
|   controlCategory |   String  |   コントロールのアクションのカテゴリ (アカウント、データ、デバイス、アプリケーション、インフラストラクチャ) です。  |
|   actionType  |   String  |   アクションの種類 (構成、レビュー、動作) を制御します。 |
|   service |   String  |   (Exchange、Sharepoint、Azure AD) のコントロールを所有しているサービスです。 |
|   maxScore |  String  |   現在では、指定した日付の最大のスコアを取得します。   |
|   層 |  String  |   制御層 (コア、防御の深さ、高度な)。    |
|   userImpact |    String  | コントロール (低、中、高) を実装するためのユーザーへの影響。    |
|   implementationCost |    String  |   Implemmentating コントロール (低、中、高) のリソースのコストです。 |
|   rank |  Int32   |   マイクロソフトのコントロールのレベルを調整します。   |
|   脅威 |   文字列コレクション   |   コントロールを軽減する脅威の一覧 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、なりすましが行われる)。 |
|   非推奨 |    ブール値 |   コントロールで減価償却されるかどうかを示すためにフラグを設定します。   |
|   改善計画 |   String  |   どのようなコントロールの説明は、改善に役立ちます。 |
|   remediationImpact | String  |   改善のユーザーへの影響の説明です。 |
|   actionUrl | String  |   URL は、コントロールが対象になることです。 |
|   controlStateUpdates |   String  |   テナントには、コントロールとしてのマークを指定するフラグ (無視して、レビュー、サード ・ パーティ) ([更新](../api/securescorecontrolprofiles-update.md)がサポートされています)。 |
|   tenantNote |    String  |   テナントは、制御用コメント ([更新](../api/securescorecontrolprofiles-update.md)) ごとに設定できます。 |
|   担当者 |    String  |   テナントは、([更新](../api/securescorecontrolprofiles-update.md)) を個別にコントロールを割り当てることができます。 |
|   updatedBy | String  |   コントロールの状態に変更を行ったユーザーのユーザー プリンシパルの名前です。 |

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
