---
title: averageComparativeScore リソースの種類
description: 異なる範囲に基づいてさまざまなスコアが含まれています。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 59faa1c3dcf3f7f2b70807a74878dab796ae4d54
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629328"
---
#  <a name="averagecomparativescore-resource-type"></a>averageComparativeScore リソースの種類

さまざまな範囲に基づいてさまざまなスコアが格納されています (たとえば、業種別の平均、企業座席の平均サイズなど)。また、コントロールカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ) に基づいています。

## <a name="properties"></a>プロパティ

|プロパティ |型 |説明 |
|:--|:--|:--|
|だけ|String|範囲の種類。 使用可能な値: `AllTenants`、`TotalSeats`、`IndustryTypes`。|
|averageScore|2 行分|指定された基準内の平均スコア。|

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
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
