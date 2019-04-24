---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
localization_priority: Normal
ms.openlocfilehash: df2e7e8cea9e1b2e6a6d1011029a1898e2794f45
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585308"
---
# <a name="itembody-resource-type"></a>itemBody リソースの種類

メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|content|String|アイテムのコンテンツ。|
|contentType|bodyType|コンテンツの種類。 可能な値は、`text` と `HTML` です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
