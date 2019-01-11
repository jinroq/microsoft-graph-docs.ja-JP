---
title: skypeForBusinessParticipantActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: de86c49da34c9af48478a912a6ab042a354a7bf5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808191"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="2aebb-103">skypeForBusinessParticipantActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2aebb-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2aebb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2aebb-104">Properties</span></span>

| <span data-ttu-id="2aebb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2aebb-105">Property</span></span>          | <span data-ttu-id="2aebb-106">種類</span><span class="sxs-lookup"><span data-stu-id="2aebb-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2aebb-107">im</span><span class="sxs-lookup"><span data-stu-id="2aebb-107">im</span></span>                | <span data-ttu-id="2aebb-108">Int64</span><span class="sxs-lookup"><span data-stu-id="2aebb-108">Int64</span></span>  |
| <span data-ttu-id="2aebb-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="2aebb-109">audioVideo</span></span>        | <span data-ttu-id="2aebb-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2aebb-110">Int64</span></span>  |
| <span data-ttu-id="2aebb-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="2aebb-111">appSharing</span></span>        | <span data-ttu-id="2aebb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2aebb-112">Int64</span></span>  |
| <span data-ttu-id="2aebb-113">web</span><span class="sxs-lookup"><span data-stu-id="2aebb-113">web</span></span>               | <span data-ttu-id="2aebb-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2aebb-114">Int64</span></span>  |
| <span data-ttu-id="2aebb-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="2aebb-115">dialInOut3rdParty</span></span> | <span data-ttu-id="2aebb-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2aebb-116">Int64</span></span>  |
| <span data-ttu-id="2aebb-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2aebb-117">reportRefreshDate</span></span> | <span data-ttu-id="2aebb-118">日付</span><span class="sxs-lookup"><span data-stu-id="2aebb-118">Date</span></span>   |
| <span data-ttu-id="2aebb-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="2aebb-119">reportDate</span></span>        | <span data-ttu-id="2aebb-120">日付</span><span class="sxs-lookup"><span data-stu-id="2aebb-120">Date</span></span>   |
| <span data-ttu-id="2aebb-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2aebb-121">reportPeriod</span></span>      | <span data-ttu-id="2aebb-122">String</span><span class="sxs-lookup"><span data-stu-id="2aebb-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2aebb-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2aebb-123">JSON representation</span></span>

<span data-ttu-id="2aebb-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2aebb-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
