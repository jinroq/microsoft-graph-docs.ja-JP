---
title: teamsUserActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 8a48a80992d8370a3b6b198862a3af901737fa04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836660"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="e2449-103">teamsUserActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2449-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e2449-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2449-104">Properties</span></span>

| <span data-ttu-id="e2449-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2449-105">Property</span></span>            | <span data-ttu-id="e2449-106">種類</span><span class="sxs-lookup"><span data-stu-id="e2449-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="e2449-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e2449-107">reportRefreshDate</span></span>   | <span data-ttu-id="e2449-108">日付</span><span class="sxs-lookup"><span data-stu-id="e2449-108">Date</span></span>   |
| <span data-ttu-id="e2449-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="e2449-109">reportDate</span></span>          | <span data-ttu-id="e2449-110">日付</span><span class="sxs-lookup"><span data-stu-id="e2449-110">Date</span></span>   |
| <span data-ttu-id="e2449-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="e2449-111">teamChatMessages</span></span>    | <span data-ttu-id="e2449-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e2449-112">Int64</span></span>  |
| <span data-ttu-id="e2449-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="e2449-113">privateChatMessages</span></span> | <span data-ttu-id="e2449-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e2449-114">Int64</span></span>  |
| <span data-ttu-id="e2449-115">呼び出し</span><span class="sxs-lookup"><span data-stu-id="e2449-115">calls</span></span>               | <span data-ttu-id="e2449-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e2449-116">Int64</span></span>  |
| <span data-ttu-id="e2449-117">会議</span><span class="sxs-lookup"><span data-stu-id="e2449-117">meetings</span></span>            | <span data-ttu-id="e2449-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e2449-118">Int64</span></span>  |
| <span data-ttu-id="e2449-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="e2449-119">otherActions</span></span>        | <span data-ttu-id="e2449-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e2449-120">Int64</span></span>  |
| <span data-ttu-id="e2449-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e2449-121">reportPeriod</span></span>        | <span data-ttu-id="e2449-122">String</span><span class="sxs-lookup"><span data-stu-id="e2449-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2449-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2449-123">JSON representation</span></span>

<span data-ttu-id="e2449-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2449-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
