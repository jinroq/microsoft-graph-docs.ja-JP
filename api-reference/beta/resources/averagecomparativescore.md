---
title: " averageComparativeScore リソースの種類"
description: このリソースには、さまざまな範囲 (たとえば、業種別の平均、企業の座席サイズ別の平均)、コントロールカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ) に基づいて、さまざまなスコアが含まれています。
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535439"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore リソースの種類

このリソースには、さまざまな範囲 (たとえば、業種別の平均、企業の座席サイズ別の平均)、コントロールカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ) に基づいて、さまざまなスコアが含まれています。

|プロパティ |型 |説明 |
|:--|:--|:--|
|   だけ   |   String  |   範囲の種類 (alltenants、totalseats、IndustryTypes)。  |
|   averageScore    |   倍精度浮動小数点数  | 指定された基準内の平均スコア。 |
|   デバイスコア |   倍精度浮動小数点数  | 指定された基準内の平均スコア。 |
|   datascore   |   倍精度浮動小数点数  | 指定された基準内の平均スコア。 |
|   「id」   |   倍精度浮動小数点数  | 指定された基準内の平均スコア。 |

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
