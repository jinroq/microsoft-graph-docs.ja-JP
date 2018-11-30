---
title: " averageComparativeScore リソースの種類"
description: このリソースには、さまざまなスコープ (業界 (縦)、会社の座席のサイズというように、平均での平均値など) および (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のコントロールの分類でさまざまなさまざまなデータが含まれています。
ms.openlocfilehash: 08e4ec60788b21476d8f1491ab5548c7a4ca2e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067776"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore リソースの種類

このリソースには、さまざまなスコープ (業界 (縦)、会社の座席のサイズというように、平均での平均値など) および (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のコントロールの分類でさまざまなさまざまなデータが含まれています。

|プロパティ |型 |説明 |
|:--|:--|:--|
|   単位   |   String  |   範囲の種類 (、AllTenants、合計座席数、IndustryTypes)。  |
|   averageScore    |   倍精度浮動小数点数  | 指定された基準内での平均スコアです。 |
|   deviceScore |   倍精度浮動小数点数  | 指定された基準内での平均スコアです。 |
|   dataScore   |   倍精度浮動小数点数  | 指定された基準内での平均スコアです。 |
|   identityScore   |   倍精度浮動小数点数  | 指定された基準内での平均スコアです。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
