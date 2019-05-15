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
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="435a5-103">itemActionStat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="435a5-103">itemActionStat resource type</span></span>

<span data-ttu-id="435a5-104">**Itemactionstat**リソースは、一定期間にわたるアクションについての集約された詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="435a5-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="435a5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="435a5-105">Properties</span></span>

| <span data-ttu-id="435a5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="435a5-106">Property</span></span>    | <span data-ttu-id="435a5-107">型</span><span class="sxs-lookup"><span data-stu-id="435a5-107">Type</span></span>  | <span data-ttu-id="435a5-108">説明</span><span class="sxs-lookup"><span data-stu-id="435a5-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="435a5-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="435a5-109">actionCount</span></span> | <span data-ttu-id="435a5-110">Int32</span><span class="sxs-lookup"><span data-stu-id="435a5-110">Int32</span></span> | <span data-ttu-id="435a5-111">アクションが行われた回数。</span><span class="sxs-lookup"><span data-stu-id="435a5-111">The number of times the action took place.</span></span> <span data-ttu-id="435a5-112">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="435a5-112">Read-only.</span></span>
| <span data-ttu-id="435a5-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="435a5-113">actorCount</span></span>  | <span data-ttu-id="435a5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="435a5-114">Int32</span></span> | <span data-ttu-id="435a5-115">アクションを実行した個別のアクターの数。</span><span class="sxs-lookup"><span data-stu-id="435a5-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="435a5-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="435a5-116">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="435a5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="435a5-117">JSON representation</span></span>

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
