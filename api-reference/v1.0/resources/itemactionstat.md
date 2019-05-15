---
author: daspek
ms.author: dspektor
title: itemActionStat リソースの種類
description: ItemActionStat オブジェクトは、一定期間にわたるアクションの集約された詳細を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d5531fc969762219f4e2404787190649ecdaf11
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970756"
---
# <a name="itemactionstat-resource-type"></a>itemActionStat リソースの種類

**Itemactionstat**リソースは、一定期間にわたるアクションについての集約された詳細を提供します。

## <a name="properties"></a>プロパティ

| プロパティ    | 型  | 説明
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | アクションが行われた回数。 値の取得のみ可能です。
| actorCount  | Int32 | アクションを実行した個別のアクターの数。 読み取り専用です。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/itemActionStat",
  "suppressions": []
}
-->
