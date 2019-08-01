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
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="7d79e-103">itemActionStat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7d79e-103">itemActionStat resource type</span></span>

<span data-ttu-id="7d79e-104">**Itemactionstat**リソースは、一定期間にわたるアクションについての集約された詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="7d79e-104">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="properties"></a><span data-ttu-id="7d79e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d79e-105">Properties</span></span>

| <span data-ttu-id="7d79e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d79e-106">Property</span></span>    | <span data-ttu-id="7d79e-107">型</span><span class="sxs-lookup"><span data-stu-id="7d79e-107">Type</span></span>  | <span data-ttu-id="7d79e-108">説明</span><span class="sxs-lookup"><span data-stu-id="7d79e-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="7d79e-109">actionCount</span><span class="sxs-lookup"><span data-stu-id="7d79e-109">actionCount</span></span> | <span data-ttu-id="7d79e-110">Int32</span><span class="sxs-lookup"><span data-stu-id="7d79e-110">Int32</span></span> | <span data-ttu-id="7d79e-111">アクションが行われた回数。</span><span class="sxs-lookup"><span data-stu-id="7d79e-111">The number of times the action took place.</span></span> <span data-ttu-id="7d79e-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7d79e-112">Read-only.</span></span>
| <span data-ttu-id="7d79e-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="7d79e-113">actorCount</span></span>  | <span data-ttu-id="7d79e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7d79e-114">Int32</span></span> | <span data-ttu-id="7d79e-115">アクションを実行した個別のアクターの数。</span><span class="sxs-lookup"><span data-stu-id="7d79e-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="7d79e-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7d79e-116">Read-only.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d79e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d79e-117">JSON representation</span></span>

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
