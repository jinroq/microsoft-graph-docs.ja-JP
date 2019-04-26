---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: itemactionstat
localization_priority: Normal
ms.openlocfilehash: a0e3bc3f217308d96eaadf6ab367431c7f1b8c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345450"
---
# <a name="itemactionstat-resource-type"></a>itemactionstat リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**itemactionstat**リソースは、一定期間にわたるアクションについての集約された詳細を提供します。

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

## <a name="properties"></a>プロパティ

| プロパティ    | 型  | 説明
|:------------|:------|:-------------------------------------------------------
| actioncount | Int32 | アクションが行われた回数。 読み取り専用です。
| actorCount  | Int32 | アクションを実行した個別のアクターの数。 値の取得のみ可能です。

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": []
}
-->
