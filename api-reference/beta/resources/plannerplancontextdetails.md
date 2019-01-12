---
title: plannerPlanContextDetails リソースの種類
description: '**PlannerPlanContextDetails**リソースには、plannerPlanContext に関する追加情報が含まれています。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e0f26bcb25bf77a0a9907ba7e0414e57ad738cae
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968219"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="c62c4-103">plannerPlanContextDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c62c4-103">plannerPlanContextDetails resource type</span></span>

> <span data-ttu-id="c62c4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c62c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c62c4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c62c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c62c4-106">**PlannerPlanContextDetails**リソースには、 [plannerPlanContext](plannerplancontext.md)に関する追加情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c62c4-106">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c62c4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c62c4-107">Properties</span></span>
| <span data-ttu-id="c62c4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c62c4-108">Property</span></span>     | <span data-ttu-id="c62c4-109">種類</span><span class="sxs-lookup"><span data-stu-id="c62c4-109">Type</span></span>   |<span data-ttu-id="c62c4-110">説明</span><span class="sxs-lookup"><span data-stu-id="c62c4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c62c4-111">url</span><span class="sxs-lookup"><span data-stu-id="c62c4-111">url</span></span>|<span data-ttu-id="c62c4-112">String</span><span class="sxs-lookup"><span data-stu-id="c62c4-112">String</span></span>|<span data-ttu-id="c62c4-113">関連付けられた[plannerPlanContext](plannerplancontext.md)によって表されるユーザー エクスペリエンスの URL です。</span><span class="sxs-lookup"><span data-stu-id="c62c4-113">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c62c4-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c62c4-114">JSON representation</span></span>

<span data-ttu-id="c62c4-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c62c4-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
