---
author: daspek
ms.author: dspektor
title: itemActionStat リソースの種類
description: ItemActionStat オブジェクトは、一定期間にわたるアクションの集約された詳細を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7eda0f6ddbed16dadf1eac4a3ea737cdd7fd2c89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036758"
---
# <a name="itemactionstat-resource-type"></a>itemActionStat リソースの種類

**Itemactionstat**リソースは、一定期間にわたるアクションについての集約された詳細を提供します。

## <a name="properties"></a>プロパティ

| プロパティ    | 型  | 説明
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | アクションが行われた回数。 読み取り専用です。
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
