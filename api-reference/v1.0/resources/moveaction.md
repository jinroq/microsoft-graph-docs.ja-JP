---
author: daspek
ms.author: dspektor
title: moveAction リソースの種類
description: MoveAction オブジェクトは、アイテムを移動したアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 525558d040109e637e2f3532d16c308a197e45fb
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970777"
---
# <a name="moveaction-resource-type"></a>moveAction リソースの種類

[**Itemactivity**] [ activity]に**moveaction**リソースが存在することは、アクティビティがアイテムを移動したことを示します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[activity]: itemactivity.md

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明
|:--------------|:-------|:----------------------------------------------------
| from          | string | アイテムの移動元の場所の名前。
| to            | string | アイテムの移動先の場所の名前。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
