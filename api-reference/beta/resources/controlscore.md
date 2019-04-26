---
title: " controlscore リソースの種類"
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
ms.openlocfilehash: 34e94128ff3993a01d37770bea1ad046f936405f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341184"
---
#  <a name="controlscore-resource-type"></a>controlscore リソースの種類

このリソースには、各コントロールのテナントのスコアと説明が含まれています。

|名前 |型 |説明 |
|:--|:--|:--|
|   controlName |   String  |   コントロールの一意の名前 |
|   score   |   2 行分  |  コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。 |
|   controlcategory |   String  |  コントロールアクションカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ)。 |
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
