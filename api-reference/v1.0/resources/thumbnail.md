---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サムネイル
ms.openlocfilehash: ff111f44101bb03b3d8475e2567d6e1b2b4a753d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264974"
---
# <a name="thumbnail-resource-type"></a>サムネイル リソースの種類

**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。

## <a name="json-representation"></a>JSON 表記

以下は、**サムネイル** リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a>プロパティ

| プロパティ     | 型   | 説明
| :----------- | :----- | :----------------------------------------------------
| 高さ       | Int32  | サムネイルの高さ (ピクセル単位)。
| sourceItemId | 文字列 | サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。
| url          | 文字列 | サムネイルのコンテンツをフェッチするために使用する URL。
| width        | Int32  | サムネイルの幅 (ピクセル単位)。
| コンテンツ      | ストリーム | サムネイルのコンテンツ ストリーム。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
