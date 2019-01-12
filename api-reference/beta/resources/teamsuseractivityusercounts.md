---
title: teamsUserActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912821"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="b28d6-103">teamsUserActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b28d6-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b28d6-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b28d6-104">Properties</span></span>

| <span data-ttu-id="b28d6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b28d6-105">Property</span></span>            | <span data-ttu-id="b28d6-106">型</span><span class="sxs-lookup"><span data-stu-id="b28d6-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="b28d6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b28d6-107">reportRefreshDate</span></span>   | <span data-ttu-id="b28d6-108">日付</span><span class="sxs-lookup"><span data-stu-id="b28d6-108">Date</span></span>   |
| <span data-ttu-id="b28d6-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="b28d6-109">reportDate</span></span>          | <span data-ttu-id="b28d6-110">日付</span><span class="sxs-lookup"><span data-stu-id="b28d6-110">Date</span></span>   |
| <span data-ttu-id="b28d6-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="b28d6-111">teamChatMessages</span></span>    | <span data-ttu-id="b28d6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b28d6-112">Int64</span></span>  |
| <span data-ttu-id="b28d6-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="b28d6-113">privateChatMessages</span></span> | <span data-ttu-id="b28d6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b28d6-114">Int64</span></span>  |
| <span data-ttu-id="b28d6-115">呼び出し</span><span class="sxs-lookup"><span data-stu-id="b28d6-115">calls</span></span>               | <span data-ttu-id="b28d6-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b28d6-116">Int64</span></span>  |
| <span data-ttu-id="b28d6-117">会議</span><span class="sxs-lookup"><span data-stu-id="b28d6-117">meetings</span></span>            | <span data-ttu-id="b28d6-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b28d6-118">Int64</span></span>  |
| <span data-ttu-id="b28d6-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="b28d6-119">otherActions</span></span>        | <span data-ttu-id="b28d6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="b28d6-120">Int64</span></span>  |
| <span data-ttu-id="b28d6-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b28d6-121">reportPeriod</span></span>        | <span data-ttu-id="b28d6-122">String</span><span class="sxs-lookup"><span data-stu-id="b28d6-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b28d6-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b28d6-123">JSON representation</span></span>

<span data-ttu-id="b28d6-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b28d6-124">The following is a JSON representation of the resource.</span></span>

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
