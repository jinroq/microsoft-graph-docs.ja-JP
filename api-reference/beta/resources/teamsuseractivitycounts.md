---
title: teamsUserActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987525"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="786d2-103">teamsUserActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="786d2-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="786d2-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="786d2-104">Properties</span></span>

| <span data-ttu-id="786d2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="786d2-105">Property</span></span>            | <span data-ttu-id="786d2-106">種類</span><span class="sxs-lookup"><span data-stu-id="786d2-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="786d2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="786d2-107">reportRefreshDate</span></span>   | <span data-ttu-id="786d2-108">日付</span><span class="sxs-lookup"><span data-stu-id="786d2-108">Date</span></span>   |
| <span data-ttu-id="786d2-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="786d2-109">reportDate</span></span>          | <span data-ttu-id="786d2-110">日付</span><span class="sxs-lookup"><span data-stu-id="786d2-110">Date</span></span>   |
| <span data-ttu-id="786d2-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="786d2-111">teamChatMessages</span></span>    | <span data-ttu-id="786d2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="786d2-112">Int64</span></span>  |
| <span data-ttu-id="786d2-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="786d2-113">privateChatMessages</span></span> | <span data-ttu-id="786d2-114">Int64</span><span class="sxs-lookup"><span data-stu-id="786d2-114">Int64</span></span>  |
| <span data-ttu-id="786d2-115">呼び出し</span><span class="sxs-lookup"><span data-stu-id="786d2-115">calls</span></span>               | <span data-ttu-id="786d2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="786d2-116">Int64</span></span>  |
| <span data-ttu-id="786d2-117">会議</span><span class="sxs-lookup"><span data-stu-id="786d2-117">meetings</span></span>            | <span data-ttu-id="786d2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="786d2-118">Int64</span></span>  |
| <span data-ttu-id="786d2-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="786d2-119">reportPeriod</span></span>        | <span data-ttu-id="786d2-120">String</span><span class="sxs-lookup"><span data-stu-id="786d2-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="786d2-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="786d2-121">JSON representation</span></span>

<span data-ttu-id="786d2-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="786d2-122">The following is a JSON representation of the resource.</span></span>

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
