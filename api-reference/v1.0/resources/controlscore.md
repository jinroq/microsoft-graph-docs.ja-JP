---
title: controlScore リソースの種類
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 68e4bf278b7d1b6ea6f00f75192847abab1ae3a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032845"
---
#  <a name="controlscore-resource-type"></a>controlScore リソースの種類

各コントロールのテナントのスコアと説明が含まれます。

## <a name="properties"></a>プロパティ

|名前 |型 |説明 |
|:--|:--|:--|
|controlName|String|一意の名前を制御します。|
|score|2 行分|コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。|
|controlCategory|String|コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。|
|description|String| コントロールの説明。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
