---
title: " controlscore リソースの種類"
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543379"
---
#  <a name="controlscore-resource-type"></a>controlscore リソースの種類

このリソースには、各コントロールのテナントのスコアと説明が含まれています。

|名前 |型 |説明 |
|:--|:--|:--|
|   controlName |   String  |   コントロールの一意の名前 |
|   score   |   倍精度浮動小数点数  |  コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。 |
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
  "score": "String",
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
