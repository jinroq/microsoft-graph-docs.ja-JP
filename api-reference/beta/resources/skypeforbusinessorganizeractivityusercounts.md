---
title: skypeForBusinessOrganizerActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 0e0b6838b58b4a3fab9a62351446bf26fc50bfbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071480"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="699b3-103">skypeForBusinessOrganizerActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="699b3-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="699b3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="699b3-104">Properties</span></span>

| <span data-ttu-id="699b3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="699b3-105">Property</span></span>           | <span data-ttu-id="699b3-106">型</span><span class="sxs-lookup"><span data-stu-id="699b3-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="699b3-107">im</span><span class="sxs-lookup"><span data-stu-id="699b3-107">im</span></span>                 | <span data-ttu-id="699b3-108">Int64</span><span class="sxs-lookup"><span data-stu-id="699b3-108">Int64</span></span>  |
| <span data-ttu-id="699b3-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="699b3-109">audioVideo</span></span>         | <span data-ttu-id="699b3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="699b3-110">Int64</span></span>  |
| <span data-ttu-id="699b3-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="699b3-111">appSharing</span></span>         | <span data-ttu-id="699b3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="699b3-112">Int64</span></span>  |
| <span data-ttu-id="699b3-113">web</span><span class="sxs-lookup"><span data-stu-id="699b3-113">web</span></span>                | <span data-ttu-id="699b3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="699b3-114">Int64</span></span>  |
| <span data-ttu-id="699b3-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="699b3-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="699b3-116">Int64</span><span class="sxs-lookup"><span data-stu-id="699b3-116">Int64</span></span>  |
| <span data-ttu-id="699b3-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="699b3-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="699b3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="699b3-118">Int64</span></span>  |
| <span data-ttu-id="699b3-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="699b3-119">reportRefreshDate</span></span>  | <span data-ttu-id="699b3-120">Date</span><span class="sxs-lookup"><span data-stu-id="699b3-120">Date</span></span>   |
| <span data-ttu-id="699b3-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="699b3-121">reportDate</span></span>         | <span data-ttu-id="699b3-122">Date</span><span class="sxs-lookup"><span data-stu-id="699b3-122">Date</span></span>   |
| <span data-ttu-id="699b3-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="699b3-123">reportPeriod</span></span>       | <span data-ttu-id="699b3-124">String</span><span class="sxs-lookup"><span data-stu-id="699b3-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="699b3-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="699b3-125">JSON representation</span></span>

<span data-ttu-id="699b3-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="699b3-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
