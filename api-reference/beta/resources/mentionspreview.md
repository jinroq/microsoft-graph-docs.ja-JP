---
title: mentionsPreview リソースの種類
description: リソースのインスタンスで記載されているオブジェクトに関する情報を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 3bb087f6eb1d3c49b85213acf60393346a42b7cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949291"
---
# <a name="mentionspreview-resource-type"></a>mentionsPreview リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

リソース インスタンス内のオブジェクトの[説明](../resources/mention.md)に関する情報を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
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
