---
title: " controlScore リソースの種類"
description: このリソースには、テナントのスコアと個々 のコントロールの説明が含まれています。
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891470"
---
#  <a name="controlscore-resource-type"></a>controlScore リソースの種類

このリソースには、テナントのスコアと個々 のコントロールの説明が含まれています。

|名前 |種類 |説明 |
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
