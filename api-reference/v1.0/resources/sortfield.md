---
title: SortField リソースの種類
description: 並べ替え操作の条件を表します。
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561300"
---
# <a name="sortfield-resource-type"></a>SortField リソースの種類

並べ替え操作の条件を表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ascending|ブール値|昇順の方法で並べ替えを行うかどうかを表します。|
|color|string|並べ替えがフォントまたはセルの色で行われるときに条件の対象となる色を表します。|
|dataOption|string|このフィールドのその他の並べ替えオプションを表します。 使用可能な値は`Normal`、 `TextAsNumber`、です。|
|Key|int|条件の対象とする列 (または行。並べ替えの方向によって異なります) を表します。最初の列 (または行) からのオフセットとして表します。|
|sortOn|string|この条件の並べ替えの種類を表します。 使用可能な値は`Value`、 `CellColor`、 `FontColor`、 `Icon`、です。|
|アイコン|[WorkbookIcon](icon.md)|並べ替えがセルのアイコンで行われる場合に、条件の対象となるアイコンを表します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
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
