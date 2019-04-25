---
title: skypeForBusinessParticipantActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: de86c49da34c9af48478a912a6ab042a354a7bf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568090"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="61738-103">skypeForBusinessParticipantActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61738-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="61738-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61738-104">Properties</span></span>

| <span data-ttu-id="61738-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61738-105">Property</span></span>          | <span data-ttu-id="61738-106">型</span><span class="sxs-lookup"><span data-stu-id="61738-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="61738-107">im</span><span class="sxs-lookup"><span data-stu-id="61738-107">im</span></span>                | <span data-ttu-id="61738-108">Int64</span><span class="sxs-lookup"><span data-stu-id="61738-108">Int64</span></span>  |
| <span data-ttu-id="61738-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="61738-109">audioVideo</span></span>        | <span data-ttu-id="61738-110">Int64</span><span class="sxs-lookup"><span data-stu-id="61738-110">Int64</span></span>  |
| <span data-ttu-id="61738-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="61738-111">appSharing</span></span>        | <span data-ttu-id="61738-112">Int64</span><span class="sxs-lookup"><span data-stu-id="61738-112">Int64</span></span>  |
| <span data-ttu-id="61738-113">web</span><span class="sxs-lookup"><span data-stu-id="61738-113">web</span></span>               | <span data-ttu-id="61738-114">Int64</span><span class="sxs-lookup"><span data-stu-id="61738-114">Int64</span></span>  |
| <span data-ttu-id="61738-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="61738-115">dialInOut3rdParty</span></span> | <span data-ttu-id="61738-116">Int64</span><span class="sxs-lookup"><span data-stu-id="61738-116">Int64</span></span>  |
| <span data-ttu-id="61738-117">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="61738-117">reportRefreshDate</span></span> | <span data-ttu-id="61738-118">Date</span><span class="sxs-lookup"><span data-stu-id="61738-118">Date</span></span>   |
| <span data-ttu-id="61738-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="61738-119">reportDate</span></span>        | <span data-ttu-id="61738-120">Date</span><span class="sxs-lookup"><span data-stu-id="61738-120">Date</span></span>   |
| <span data-ttu-id="61738-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="61738-121">reportPeriod</span></span>      | <span data-ttu-id="61738-122">String</span><span class="sxs-lookup"><span data-stu-id="61738-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61738-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61738-123">JSON representation</span></span>

<span data-ttu-id="61738-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61738-124">The following is a JSON representation of the resource.</span></span>

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
