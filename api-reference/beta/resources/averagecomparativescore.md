---
title: " averageComparativeScore リソースの種類"
description: このリソースには、さまざまな範囲 (たとえば、業種別の平均、企業の座席サイズ別の平均)、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) に基づいて、さまざまなスコアが含まれています。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3e2256e7edefd0670bb697ec6d89c9fb80a5beeb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013151"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore リソースの種類

このリソースには、さまざまな範囲 (たとえば、業種別の平均、企業の座席サイズ別の平均)、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) に基づいて、さまざまなスコアが含まれています。

|プロパティ |型 |説明 |
|:--|:--|:--|
|   だけ   |   String  |   範囲の種類 (AllTenants、TotalSeats、IndustryTypes)。  |
|   averageScore    |   2 行分  | 指定された基準内の平均スコア。 |
|   デバイスコア |   2 行分  | 指定された基準内の平均スコア。 |
|   dataScore   |   2 行分  | 指定された基準内の平均スコア。 |
|   「Id」   |   2 行分  | 指定された基準内の平均スコア。 |

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
