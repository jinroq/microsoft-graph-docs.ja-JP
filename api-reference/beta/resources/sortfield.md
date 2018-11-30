---
title: SortField リソースの種類
description: 並べ替え操作の条件を表します。
ms.openlocfilehash: bb5915e9d9637912b97c0425819acd15a6ed40ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072235"
---
# <a name="sortfield-resource-type"></a>SortField リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

並べ替え操作の条件を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ascending|ブール値|昇順の方法で並べ替えを行うかどうかを表します。|
|color|文字列|並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。|
|dataOption|文字列|このフィールドのその他の並べ替えオプションを表します。可能な値は、`Normal`、`TextAsNumber` です。|
|Key|int|条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。|
|sortOn|文字列|この条件の並べ替えの種類を表します。可能な値は、`Value`、`CellColor`、`FontColor`、`Icon` です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|アイコン|[Icon](icon.md)|並べ替えがセルのアイコンで行われるときに条件の対象となるアイコンを表します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->