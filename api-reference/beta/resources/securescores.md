---
title: secureScores リソースの種類
description: 'top = n、n は取得するデータの日数を指定します。 '
localization_priority: Normal
ms.openlocfilehash: 8b4be9822b782303efe38dbdf5bd43e1ee543421
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549203"
---
# <a name="securescores-resource-type"></a>secureScores リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントとコントロールレベルでのスコアデータの1日あたりのテナントのセキュリティスコアを表します。 既定では、90日間のデータが保持されます。 このデータは、新しい**日付**から最も古い日付までの日付で並べ替えられます。 これにより、$top = n (n は取得するデータの日数) を使用して、応答をページに表示できます。 


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[secureScores のリスト](../api/securescores-list.md) | [secureScores](securescores.md) |secureScores オブジェクトのプロパティとメタデータを読み取ります。|


## <a name="properties"></a>プロパティ
テナントのセキュリティスコアのプロパティを含むエンティティ型 (毎日のスナップショットデータ)。

|プロパティ |型 |説明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   テナント ID の GUID 文字列。  |
|   createdDateTime |   DateTimeOffset  |   エンティティが作成された日付。  |
|   id  |   String  |   azureTenantId_createdDateTime の組み合わせ。   |
|   licensedUserCount   |   Int32   |   指定したテナントのライセンスされたユーザーカウント。    |
|   activeusercount |   Int32   |   指定したテナントのアクティブなユーザー数。  |
|   currentscore    |   倍精度浮動小数点数  |   指定された日付における現在のテナントのスコア。    |
|   maxscore |  倍精度浮動小数点数  |   指定した日付の有効なテナントの最大スコア。    |
|   enabledservices |   String collection   |   テナントの Microsoft 提供のサービス (Exchange online、Skype、Sharepoint など)。   |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md)コレクション    |範囲内の別のスコープ (たとえば、業種別平均、座席の平均)、コントロールカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ) の平均スコア。 |
|   controlscores | [controlscore](controlscore.md)コレクション  |   一連のコントロールのテナントスコアを含みます。   |


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
"id": "String",
"azureTenantId": "Guid",
"createdDate": "DateTimeOffset",
"licensedUserCount": "Int32",
"activeUserCount": "Int32",
"currentScore": "Int32",
"maxScore": "Int32",
"averageScore": "Double",
"enabledServices": "Collection(string)",
"averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
"controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
