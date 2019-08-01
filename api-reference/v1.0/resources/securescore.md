---
title: secureScore リソースの種類
description: テナントとコントロールレベルでのスコアデータの1日あたりのテナントのセキュリティスコアを表します。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 395c5ed0594d1f509bb664b5aee6ea18bb42af0a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034483"
---
# <a name="securescore-resource-type"></a>secureScore リソースの種類

テナントとコントロールレベルでのスコアデータの1日あたりのテナントのセキュリティスコアを表します。 既定では、90日間のデータが保持されます。 このデータは、新しい**日付**から最も古い日付までの日付で並べ替えられます。 これにより、$top = n (n は取得するデータの日数) を使用して、応答をページに表示できます。 


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[secureScores のリスト](../api/security-list-securescores.md) | [secureScores](securescore.md)コレクション |SecureScore オブジェクトのコレクションを取得します。|
|[secureScore の取得](../api/securescore-get.md) | [secureScore](securescore.md) |SecureScore オブジェクトのプロパティとメタデータを読み取ります。 | 



## <a name="properties"></a>プロパティ

|プロパティ |型 |説明 |
|:--|:--|:--|
|id |String|プロバイダーによって生成された GUID/一意の識別子。 読み取り専用です。 必須です。|
|   azureTenantId   |   String  |   テナント ID の GUID 文字列。  |
|   activeUserCount |   Int32   |   指定したテナントのアクティブなユーザー数。  |
|   createdDateTime |   DateTimeOffset  |   エンティティが作成された日付。  |
|   currentScore    |   2 行分  |   指定された日付における現在のテナントのスコア。    |
|   enabledServices |   文字列コレクション   |   テナントの Microsoft 提供のサービス (Exchange online、Skype、Sharepoint など)。   |
|   licensedUserCount   |   Int32   |   指定したテナントのライセンスされたユーザーカウント。    |
|   maxScore |  2 行分  |   指定した日付の有効なテナントの最大スコア。    |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md)コレクション    |範囲内の別のスコープ (たとえば、業種別平均、座席の平均)、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) の平均スコア。 |
|   controlScores | [Controlscore](controlscore.md)コレクション  |   一連のコントロールのテナントスコアを含みます。   |
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = SecureScore)。 必須です。|


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
"id": "String (identifier)",
"azureTenantId": "String",
"activeUserCount": "Int32",
"createdDateTime": "String (timestamp)",
"currentScore": "Double",
"enabledServices": ["String"],
"licensedUserCount": "Int32",
"maxScore": "Double",
"averageComparativeScores": [{"@odata.type": "microsoft.graph.averageComparativeScore"}],
"controlScores": [{"@odata.type": "microsoft.graph.controlScore"}],
"vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
