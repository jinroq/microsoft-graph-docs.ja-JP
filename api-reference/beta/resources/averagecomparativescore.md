---
title: " averageComparativeScore リソースの種類"
description: このリソースには、さまざまなスコープ (業界 (縦)、会社の座席のサイズというように、平均での平均値など) および (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のコントロールの分類でさまざまなさまざまなデータが含まれています。
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834595"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore リソースの種類

このリソースには、さまざまなスコープ (業界 (縦)、会社の座席のサイズというように、平均での平均値など) および (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のコントロールの分類でさまざまなさまざまなデータが含まれています。

|プロパティ |種類 |説明 |
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
