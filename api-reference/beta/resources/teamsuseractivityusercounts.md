---
title: teamsUserActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f0b6d9d77518b6e40a5793c6715bfbae69600f3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964362"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="6d7fb-103">teamsUserActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d7fb-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d7fb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d7fb-104">Properties</span></span>

| <span data-ttu-id="6d7fb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d7fb-105">Property</span></span>            | <span data-ttu-id="6d7fb-106">型</span><span class="sxs-lookup"><span data-stu-id="6d7fb-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="6d7fb-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d7fb-107">reportRefreshDate</span></span>   | <span data-ttu-id="6d7fb-108">日付</span><span class="sxs-lookup"><span data-stu-id="6d7fb-108">Date</span></span>   |
| <span data-ttu-id="6d7fb-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="6d7fb-109">reportDate</span></span>          | <span data-ttu-id="6d7fb-110">日付</span><span class="sxs-lookup"><span data-stu-id="6d7fb-110">Date</span></span>   |
| <span data-ttu-id="6d7fb-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="6d7fb-111">teamChatMessages</span></span>    | <span data-ttu-id="6d7fb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6d7fb-112">Int64</span></span>  |
| <span data-ttu-id="6d7fb-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="6d7fb-113">privateChatMessages</span></span> | <span data-ttu-id="6d7fb-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6d7fb-114">Int64</span></span>  |
| <span data-ttu-id="6d7fb-115">calls</span><span class="sxs-lookup"><span data-stu-id="6d7fb-115">calls</span></span>               | <span data-ttu-id="6d7fb-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6d7fb-116">Int64</span></span>  |
| <span data-ttu-id="6d7fb-117">meetings</span><span class="sxs-lookup"><span data-stu-id="6d7fb-117">meetings</span></span>            | <span data-ttu-id="6d7fb-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6d7fb-118">Int64</span></span>  |
| <span data-ttu-id="6d7fb-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="6d7fb-119">otherActions</span></span>        | <span data-ttu-id="6d7fb-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6d7fb-120">Int64</span></span>  |
| <span data-ttu-id="6d7fb-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d7fb-121">reportPeriod</span></span>        | <span data-ttu-id="6d7fb-122">String</span><span class="sxs-lookup"><span data-stu-id="6d7fb-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6d7fb-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d7fb-123">JSON representation</span></span>

<span data-ttu-id="6d7fb-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d7fb-124">The following is a JSON representation of the resource.</span></span>

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
