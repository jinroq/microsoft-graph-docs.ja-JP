---
title: teamsUserActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9e1a40d962ded7825b72d31675cefb9869750866
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007621"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="e71ca-103">teamsUserActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e71ca-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e71ca-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e71ca-104">Properties</span></span>

| <span data-ttu-id="e71ca-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e71ca-105">Property</span></span>            | <span data-ttu-id="e71ca-106">型</span><span class="sxs-lookup"><span data-stu-id="e71ca-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="e71ca-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e71ca-107">reportRefreshDate</span></span>   | <span data-ttu-id="e71ca-108">日付</span><span class="sxs-lookup"><span data-stu-id="e71ca-108">Date</span></span>   |
| <span data-ttu-id="e71ca-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="e71ca-109">reportDate</span></span>          | <span data-ttu-id="e71ca-110">日付</span><span class="sxs-lookup"><span data-stu-id="e71ca-110">Date</span></span>   |
| <span data-ttu-id="e71ca-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="e71ca-111">teamChatMessages</span></span>    | <span data-ttu-id="e71ca-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e71ca-112">Int64</span></span>  |
| <span data-ttu-id="e71ca-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="e71ca-113">privateChatMessages</span></span> | <span data-ttu-id="e71ca-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e71ca-114">Int64</span></span>  |
| <span data-ttu-id="e71ca-115">calls</span><span class="sxs-lookup"><span data-stu-id="e71ca-115">calls</span></span>               | <span data-ttu-id="e71ca-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e71ca-116">Int64</span></span>  |
| <span data-ttu-id="e71ca-117">meetings</span><span class="sxs-lookup"><span data-stu-id="e71ca-117">meetings</span></span>            | <span data-ttu-id="e71ca-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e71ca-118">Int64</span></span>  |
| <span data-ttu-id="e71ca-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e71ca-119">reportPeriod</span></span>        | <span data-ttu-id="e71ca-120">String</span><span class="sxs-lookup"><span data-stu-id="e71ca-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e71ca-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e71ca-121">JSON representation</span></span>

<span data-ttu-id="e71ca-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e71ca-122">The following is a JSON representation of the resource.</span></span>

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
