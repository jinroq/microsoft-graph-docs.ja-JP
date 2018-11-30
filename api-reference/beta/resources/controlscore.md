---
title: " controlScore リソースの種類"
description: このリソースには、テナントのスコアと個々 のコントロールの説明が含まれています。
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067808"
---
#  <a name="controlscore-resource-type"></a>controlScore リソースの種類

このリソースには、テナントのスコアと個々 のコントロールの説明が含まれています。

|名前 |型 |説明 |
|:--|:--|:--|
|   controlName |   String  |   コントロールの一意の名前 |
|   score   |   倍精度浮動小数点数  |  テナントは、コントロールの (日単位によって異なりますコントロール上のテナントの操作) のスコアを達成しました。 |
|   controlCategory |   String  |  コントロールのアクションのカテゴリ (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) です。 |
|   説明 |   String  |  コントロールの説明です。 |

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
