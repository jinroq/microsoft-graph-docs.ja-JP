---
title: controlScore リソースの種類
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 64b5377fce01273ab31d7ec293f5dc7a6e1342ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629286"
---
#  <a name="controlscore-resource-type"></a>controlScore リソースの種類

各コントロールのテナントのスコアと説明が含まれます。

## <a name="properties"></a>プロパティ

|名前 |型 |説明 |
|:--|:--|:--|
|controlName|String|一意の名前を制御します。|
|score|2 行分|コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。|
|controlCategory|String|コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。|
|説明|String| コントロールの説明。|

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
