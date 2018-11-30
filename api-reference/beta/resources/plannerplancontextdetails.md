---
title: plannerPlanContextDetails リソースの種類
description: '**PlannerPlanContextDetails**リソースには、plannerPlanContext に関する追加情報が含まれています。'
ms.openlocfilehash: 44c1099c1155372a23029cd0cc6a4decd68c5bc0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067387"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="44403-103">plannerPlanContextDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44403-103">plannerPlanContextDetails resource type</span></span>

> <span data-ttu-id="44403-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44403-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44403-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44403-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44403-106">**PlannerPlanContextDetails**リソースには、 [plannerPlanContext](plannerplancontext.md)に関する追加情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="44403-106">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="44403-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44403-107">Properties</span></span>
| <span data-ttu-id="44403-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44403-108">Property</span></span>     | <span data-ttu-id="44403-109">型</span><span class="sxs-lookup"><span data-stu-id="44403-109">Type</span></span>   |<span data-ttu-id="44403-110">説明</span><span class="sxs-lookup"><span data-stu-id="44403-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44403-111">url</span><span class="sxs-lookup"><span data-stu-id="44403-111">url</span></span>|<span data-ttu-id="44403-112">String</span><span class="sxs-lookup"><span data-stu-id="44403-112">String</span></span>|<span data-ttu-id="44403-113">関連付けられた[plannerPlanContext](plannerplancontext.md)によって表されるユーザー エクスペリエンスの URL です。</span><span class="sxs-lookup"><span data-stu-id="44403-113">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44403-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44403-114">JSON representation</span></span>

<span data-ttu-id="44403-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44403-115">The following is a JSON representation of the resource.</span></span>

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
