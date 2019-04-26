---
title: プラン、contextdetails リソースの種類
description: 「 **plan the contextdetails** resource」には、プランのコンテキストに関する追加情報が含まれています。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2a63195280e7f74210ddc02f8d82b602f40343e8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344457"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="f9aa4-103">プラン、contextdetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9aa4-103">plannerPlanContextDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9aa4-104">「 **plan the contextdetails** resource」には、プランの[コンテキスト](plannerplancontext.md)に関する追加情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f9aa4-104">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f9aa4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9aa4-105">Properties</span></span>
| <span data-ttu-id="f9aa4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9aa4-106">Property</span></span>     | <span data-ttu-id="f9aa4-107">型</span><span class="sxs-lookup"><span data-stu-id="f9aa4-107">Type</span></span>   |<span data-ttu-id="f9aa4-108">説明</span><span class="sxs-lookup"><span data-stu-id="f9aa4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9aa4-109">url</span><span class="sxs-lookup"><span data-stu-id="f9aa4-109">url</span></span>|<span data-ttu-id="f9aa4-110">String</span><span class="sxs-lookup"><span data-stu-id="f9aa4-110">String</span></span>|<span data-ttu-id="f9aa4-111">関連する[プランのコンテキスト](plannerplancontext.md)によって表されるユーザーの作業の URL。</span><span class="sxs-lookup"><span data-stu-id="f9aa4-111">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9aa4-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9aa4-112">JSON representation</span></span>

<span data-ttu-id="f9aa4-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9aa4-113">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
