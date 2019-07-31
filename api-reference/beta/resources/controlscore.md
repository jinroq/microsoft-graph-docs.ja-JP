---
title: " controlScore リソースの種類"
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 89e448d828f1f7caef73b14586b06d1df238f100
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973934"
---
#  <a name="controlscore-resource-type"></a>controlScore リソースの種類

このリソースには、各コントロールのテナントのスコアと説明が含まれています。

|名前 |型 |説明 |
|:--|:--|:--|
|   controlName |   String  |   コントロールの一意の名前 |
|   score   |   2 行分  |  コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。 |
|   controlCategory |   String  |  コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。 |
|   description |   String  |  コントロールの説明。 |

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
