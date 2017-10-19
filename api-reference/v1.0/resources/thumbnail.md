---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "サムネイル"
ms.openlocfilehash: 065c6ae7bbd4f6aca3172afd4399f0a1b5ff3d25
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnail-resource-type"></a>Thumbnail リソース型

**サムネイル** リソースの種類は、ビットマップ表示を含む画像、ビデオ、ドキュメント、任意のアイテムのサムネイルを表します。

## <a name="json-representation"></a>JSON 表記

以下は、**サムネイル** リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a>プロパティ

| プロパティ     | 型   | 説明                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| height       | Int32  | サムネイルの高さ (ピクセル単位)。                                                                                     |
| sourceItemId | String | サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。 |
| url          | String | サムネイルのコンテンツをフェッチするために使用する URL。                                                                                |
| width        | Int32  | サムネイルの幅 (ピクセル単位)。                                                                                      |

## <a name="relationships"></a>関係

| 名前    | 型   | 説明                           |
| :------ | :----- | :------------------------------------ |
| content | Stream | サムネイルのコンテンツ ストリーム。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
