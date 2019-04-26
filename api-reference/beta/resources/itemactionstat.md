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
# <a name="itemactionstat-resource-type"></a><span data-ttu-id="861da-102">itemactionstat リソースの種類</span><span class="sxs-lookup"><span data-stu-id="861da-102">itemActionStat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="861da-103">**itemactionstat**リソースは、一定期間にわたるアクションについての集約された詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="861da-103">The **itemActionStat** resource provides aggregate details about an action over a period of time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="861da-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="861da-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="861da-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="861da-105">Properties</span></span>

| <span data-ttu-id="861da-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="861da-106">Property</span></span>    | <span data-ttu-id="861da-107">型</span><span class="sxs-lookup"><span data-stu-id="861da-107">Type</span></span>  | <span data-ttu-id="861da-108">説明</span><span class="sxs-lookup"><span data-stu-id="861da-108">Description</span></span>
|:------------|:------|:-------------------------------------------------------
| <span data-ttu-id="861da-109">actioncount</span><span class="sxs-lookup"><span data-stu-id="861da-109">actionCount</span></span> | <span data-ttu-id="861da-110">Int32</span><span class="sxs-lookup"><span data-stu-id="861da-110">Int32</span></span> | <span data-ttu-id="861da-111">アクションが行われた回数。</span><span class="sxs-lookup"><span data-stu-id="861da-111">The number of times the action took place.</span></span> <span data-ttu-id="861da-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="861da-112">Read-only.</span></span>
| <span data-ttu-id="861da-113">actorCount</span><span class="sxs-lookup"><span data-stu-id="861da-113">actorCount</span></span>  | <span data-ttu-id="861da-114">Int32</span><span class="sxs-lookup"><span data-stu-id="861da-114">Int32</span></span> | <span data-ttu-id="861da-115">アクションを実行した個別のアクターの数。</span><span class="sxs-lookup"><span data-stu-id="861da-115">The number of distinct actors that performed the action.</span></span> <span data-ttu-id="861da-116">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="861da-116">Read-only.</span></span>

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
