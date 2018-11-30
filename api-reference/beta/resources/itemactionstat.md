---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
ms.openlocfilehash: f7e9351bc4a394005cffc712aa444c999a51b363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073268"
---
# <a name="itemactionstat-resource-type"></a>itemActionStat リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**ItemActionStat**リソースでは、集計の詳細については、期間内にアクションを提供します。

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
| actionCount | Int32 | アクションが発生した回数です。 読み取り専用。
| actorCount  | Int32 | アクションを実行する異なるアクターの数です。 読み取り専用です。

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat"
} -->
