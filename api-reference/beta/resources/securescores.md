---
title: secureScore リソースの種類
description: 'top = n、n は取得するデータの日数を指定します。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d1db0e97c88f4532bad2052f77a3513084c74aa7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008587"
---
# <a name="securescore-resource-type"></a>secureScore リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントとコントロールレベルでのスコアデータの1日あたりのテナントのセキュリティスコアを表します。 既定では、90日間のデータが保持されます。 このデータは、新しい**日付**から最も古い日付までの日付で並べ替えられます。 これにより、$top = n (n は取得するデータの日数) を使用して、応答をページに表示できます。 


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[secureScores のリスト](../api/securescores-list.md) | [secureScores](securescores.md) |SecureScores オブジェクトのプロパティとメタデータを読み取ります。|


## <a name="properties"></a>プロパティ
テナントのセキュリティスコアのプロパティを含むエンティティ型 (毎日のスナップショットデータ)。

|プロパティ |型 |説明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   テナント ID の GUID 文字列。  |
|   createdDateTime |   DateTimeOffset  |   エンティティが作成された日付。  |
|   id  |   文字列  |   AzureTenantId_createdDateTime の組み合わせ。   |
|   licensedUserCount   |   Int32   |   指定したテナントのライセンスされたユーザーカウント。    |
|   activeUserCount |   Int32   |   指定したテナントのアクティブなユーザー数。  |
|   currentScore    |   2 行分  |   指定された日付における現在のテナントのスコア。    |
|   maxScore |  2 行分  |   指定した日付の有効なテナントの最大スコア。    |
|   enabledServices |   文字列コレクション   |   テナントの Microsoft 提供のサービス (Exchange online、Skype、Sharepoint など)。   |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md)コレクション    |範囲内の別のスコープ (たとえば、業種別平均、座席の平均)、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) の平均スコア。 |
|   controlScores | [Controlscore](controlscore.md)コレクション  |   一連のコントロールのテナントスコアを含みます。   |


## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
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
  "createdDateTime": "2019-02-07T20:33:53.156Z"
}

```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
