---
title: itemAttachment リソースの種類
description: '別のイベント、メッセージ、または投稿に添付された連絡先、イベント、またはメッセージです。  '
localization_priority: Priority
ms.prod: outlook
author: angelgolfer-ms
doc_type: resourcePageType
ms.openlocfilehash: 7df14ea5d6611cb3771aeb23250c1e65fb6e60a4
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484360"
---
# <a name="itemattachment-resource-type"></a>itemAttachment リソースの種類

別のイベント、メッセージ、または投稿に添付された連絡先、イベント、またはメッセージです。  

[添付ファイル](attachment.md)から派生します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[取得](../api/attachment-get.md) | [itemAttachment](itemattachment.md) |itemAttachment オブジェクトのプロパティと関係を読み取ります。|
|[Delete](../api/attachment-delete.md) | なし |itemAttachment オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|contentType|String|添付ファイルのコンテンツ タイプ。|
|id|String| 添付ファイル ID。|
|isInline|Boolean|添付ファイルがインライン (アイテムの本文に埋め込まれた画像など) の場合に、true に設定します。|
|lastModifiedDateTime|DateTimeOffset|添付ファイルが変更された最後の日時です。|
|name|String|添付ファイルの表示名。|
|size|Int32|添付ファイルのバイト単位のサイズ。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|item|[OutlookItem](outlookitem.md)|添付されたメッセージまたはイベントです。ナビゲーション プロパティです。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
