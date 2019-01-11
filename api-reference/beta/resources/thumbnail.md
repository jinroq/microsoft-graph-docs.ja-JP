---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: サムネイル
localization_priority: Normal
ms.openlocfilehash: 22602d534c3fd1f308a5e2bb67992bd76086c4fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863225"
---
# <a name="thumbnail-resource-type"></a>サムネイル リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

| プロパティ     | 種類   | 説明                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| height       | Int32  | サムネイルの高さ (ピクセル単位)。                                                                                     |
| sourceItemId | String | サムネイルを提供したアイテムの一意識別子。フォルダーのサムネイルが要求された場合にのみ利用可能です。 |
| url          | String | サムネイルのコンテンツをフェッチするために使用する URL。                                                                                |
| width        | Int32  | サムネイルの幅 (ピクセル単位)。                                                                                      |

## <a name="relationships"></a>関係

| 名前    | 種類   | 説明                           |
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
