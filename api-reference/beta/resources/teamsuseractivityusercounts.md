---
title: teamsUserActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
ms.openlocfilehash: f4e10f1e34d4c6bdbed83279b98632c504630bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330458"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="6d45b-103">teamsUserActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d45b-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d45b-104">Properties</span><span class="sxs-lookup"><span data-stu-id="6d45b-104">Properties</span></span>

| <span data-ttu-id="6d45b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d45b-105">Property</span></span>            | <span data-ttu-id="6d45b-106">種類</span><span class="sxs-lookup"><span data-stu-id="6d45b-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="6d45b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d45b-107">reportRefreshDate</span></span>   | <span data-ttu-id="6d45b-108">日付</span><span class="sxs-lookup"><span data-stu-id="6d45b-108">Date</span></span>   |
| <span data-ttu-id="6d45b-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="6d45b-109">reportDate</span></span>          | <span data-ttu-id="6d45b-110">日付</span><span class="sxs-lookup"><span data-stu-id="6d45b-110">Date</span></span>   |
| <span data-ttu-id="6d45b-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="6d45b-111">teamChatMessages</span></span>    | <span data-ttu-id="6d45b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6d45b-112">Int64</span></span>  |
| <span data-ttu-id="6d45b-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="6d45b-113">privateChatMessages</span></span> | <span data-ttu-id="6d45b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6d45b-114">Int64</span></span>  |
| <span data-ttu-id="6d45b-115">呼び出し</span><span class="sxs-lookup"><span data-stu-id="6d45b-115">calls</span></span>               | <span data-ttu-id="6d45b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6d45b-116">Int64</span></span>  |
| <span data-ttu-id="6d45b-117">会議</span><span class="sxs-lookup"><span data-stu-id="6d45b-117">meetings</span></span>            | <span data-ttu-id="6d45b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6d45b-118">Int64</span></span>  |
| <span data-ttu-id="6d45b-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="6d45b-119">otherActions</span></span>        | <span data-ttu-id="6d45b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6d45b-120">Int64</span></span>  |
| <span data-ttu-id="6d45b-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d45b-121">reportPeriod</span></span>        | <span data-ttu-id="6d45b-122">String</span><span class="sxs-lookup"><span data-stu-id="6d45b-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d45b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d45b-123">JSON representation</span></span>

<span data-ttu-id="6d45b-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d45b-124">The following is a JSON representation of the resource.</span></span>

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
