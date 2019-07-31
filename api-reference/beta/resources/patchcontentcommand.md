---
title: 実行時 Contentcommand リソースの種類
description: PATCH 要求で OneNote ページに加えられた変更。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2408d08434b97f865ae19cbc70fd1dc16ff6868b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009210"
---
# <a name="patchcontentcommand-resource-type"></a>実行時 Contentcommand リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

PATCH 要求で OneNote ページに加えられた変更。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。これは、 [PATCH pages/{id} '](../api/page-update.md)要求の本文で送信されます。 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|action|String|ターゲット要素で実行するアクション。 可能な値は、`replace`、`append`、`delete`、`insert`、`prepend` です。|
|content|String|ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。 コンテンツにバイナリデータが含まれている場合は、 `multipart/form-data`コンテンツタイプを使用して要求を "Commands" パートで送信する必要があります。 |
|position|String|指定されたコンテンツを追加する位置を、ターゲット要素を基準にして指定します。 可能な値は`after`次のとおりです`before`。 (既定値) または。|
|target|String|更新する要素。 `#<data-id>`または、また`body`はのいずれ`title`か`<id>`のキーワードを指定する必要があります。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
