---
author: daspek
description: ItemActionStat リソースは、一定期間にわたるアクションについての集約された詳細を提供します。
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 719a443af65fd9642feee3bc8ddbc832eb3964c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010113"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="6eeb5-103">itemActionStat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6eeb5-103">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eeb5-104">**Itemactionstat**リソースは、一定期間にわたるアクションについての集約された詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="6eeb5-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6eeb5-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6eeb5-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6eeb5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6eeb5-106">Properties</span></span>

| <span data-ttu-id="6eeb5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6eeb5-107">Property</span></span>    | <span data-ttu-id="6eeb5-108">型</span><span class="sxs-lookup"><span data-stu-id="6eeb5-108">Type</span></span>  | <span data-ttu-id="6eeb5-109">説明</span><span class="sxs-lookup"><span data-stu-id="6eeb5-109">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="6eeb5-110">actionCount</span><span class="sxs-lookup"><span data-stu-id="6eeb5-110">actionCount</span></span> | <span data-ttu-id="6eeb5-111">Int32</span><span class="sxs-lookup"><span data-stu-id="6eeb5-111">Int32</span></span> | <span data-ttu-id="6eeb5-112">アクションが行われた回数。</span><span class="sxs-lookup"><span data-stu-id="6eeb5-112">The number of times the action took place.</span></span> <span data-ttu-id="6eeb5-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6eeb5-113">Read-only.</span></span>
| <span data-ttu-id="6eeb5-114">actorCount</span><span class="sxs-lookup"><span data-stu-id="6eeb5-114">actorCount</span></span>  | <span data-ttu-id="6eeb5-115">Int32</span><span class="sxs-lookup"><span data-stu-id="6eeb5-115">Int32</span></span> | <span data-ttu-id="6eeb5-116">アクションを実行した個別のアクターの数。</span><span class="sxs-lookup"><span data-stu-id="6eeb5-116">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="6eeb5-117">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6eeb5-117">Read-only.</span></span>

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
