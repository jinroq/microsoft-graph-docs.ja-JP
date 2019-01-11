---
title: teamsUserActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c7351795f6b3dafbac996844fc1ac11cd24bbc03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886591"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="995dc-103">teamsUserActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="995dc-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="995dc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="995dc-104">Properties</span></span>

| <span data-ttu-id="995dc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="995dc-105">Property</span></span>            | <span data-ttu-id="995dc-106">種類</span><span class="sxs-lookup"><span data-stu-id="995dc-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="995dc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="995dc-107">reportRefreshDate</span></span>   | <span data-ttu-id="995dc-108">日付</span><span class="sxs-lookup"><span data-stu-id="995dc-108">Date</span></span>   |
| <span data-ttu-id="995dc-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="995dc-109">reportDate</span></span>          | <span data-ttu-id="995dc-110">日付</span><span class="sxs-lookup"><span data-stu-id="995dc-110">Date</span></span>   |
| <span data-ttu-id="995dc-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="995dc-111">teamChatMessages</span></span>    | <span data-ttu-id="995dc-112">Int64</span><span class="sxs-lookup"><span data-stu-id="995dc-112">Int64</span></span>  |
| <span data-ttu-id="995dc-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="995dc-113">privateChatMessages</span></span> | <span data-ttu-id="995dc-114">Int64</span><span class="sxs-lookup"><span data-stu-id="995dc-114">Int64</span></span>  |
| <span data-ttu-id="995dc-115">呼び出し</span><span class="sxs-lookup"><span data-stu-id="995dc-115">calls</span></span>               | <span data-ttu-id="995dc-116">Int64</span><span class="sxs-lookup"><span data-stu-id="995dc-116">Int64</span></span>  |
| <span data-ttu-id="995dc-117">会議</span><span class="sxs-lookup"><span data-stu-id="995dc-117">meetings</span></span>            | <span data-ttu-id="995dc-118">Int64</span><span class="sxs-lookup"><span data-stu-id="995dc-118">Int64</span></span>  |
| <span data-ttu-id="995dc-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="995dc-119">reportPeriod</span></span>        | <span data-ttu-id="995dc-120">String</span><span class="sxs-lookup"><span data-stu-id="995dc-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="995dc-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="995dc-121">JSON representation</span></span>

<span data-ttu-id="995dc-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="995dc-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
