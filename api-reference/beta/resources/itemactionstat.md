---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
ms.openlocfilehash: 1d2ab438e7aaf5b0a6aede99290394a9a4ea7f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879528"
---
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="fef48-102">itemActionStat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fef48-102">itemActionStat resource type</span></span>

> <span data-ttu-id="fef48-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fef48-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fef48-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fef48-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fef48-105">**ItemActionStat**リソースでは、集計の詳細については、期間内にアクションを提供します。</span><span class="sxs-lookup"><span data-stu-id="fef48-105">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fef48-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fef48-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fef48-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fef48-107">Properties</span></span>

| <span data-ttu-id="fef48-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fef48-108">Property</span></span>    | <span data-ttu-id="fef48-109">種類</span><span class="sxs-lookup"><span data-stu-id="fef48-109">Type</span></span>  | <span data-ttu-id="fef48-110">説明</span><span class="sxs-lookup"><span data-stu-id="fef48-110">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="fef48-111">actionCount</span><span class="sxs-lookup"><span data-stu-id="fef48-111">actionCount</span></span> | <span data-ttu-id="fef48-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fef48-112">Int32</span></span> | <span data-ttu-id="fef48-113">アクションが発生した回数です。</span><span class="sxs-lookup"><span data-stu-id="fef48-113">The number of times the action took place.</span></span> <span data-ttu-id="fef48-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fef48-114">Read-only.</span></span>
| <span data-ttu-id="fef48-115">actorCount</span><span class="sxs-lookup"><span data-stu-id="fef48-115">actorCount</span></span>  | <span data-ttu-id="fef48-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fef48-116">Int32</span></span> | <span data-ttu-id="fef48-117">アクションを実行する異なるアクターの数です。</span><span class="sxs-lookup"><span data-stu-id="fef48-117">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="fef48-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fef48-118">Read-only.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat"
} -->
