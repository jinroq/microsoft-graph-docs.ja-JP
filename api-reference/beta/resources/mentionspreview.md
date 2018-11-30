---
title: mentionsPreview リソースの種類
description: リソースのインスタンスで記載されているオブジェクトに関する情報を表します。
ms.openlocfilehash: cf6bed3cdfb2d3f541438da0c06fcf8f4873c17e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073098"
---
# <a name="mentionspreview-resource-type"></a>mentionsPreview リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

リソース インスタンス内のオブジェクトの[説明](../resources/mention.md)に関する情報を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| isMentioned | Boolean | ログインしているユーザーが親リソース インスタンスでメンションされている場合は true です。読み取り専用。フィルターがサポートされています。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
