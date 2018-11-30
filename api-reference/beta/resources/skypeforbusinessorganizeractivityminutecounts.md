---
title: skypeForBusinessOrganizerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: f11d303bd8737d9fb2870042ee93557343d44a2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072506"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a><span data-ttu-id="58fa0-103">skypeForBusinessOrganizerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58fa0-103">skypeForBusinessOrganizerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="58fa0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58fa0-104">Properties</span></span>

| <span data-ttu-id="58fa0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58fa0-105">Property</span></span>           | <span data-ttu-id="58fa0-106">型</span><span class="sxs-lookup"><span data-stu-id="58fa0-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="58fa0-107">audioVideo</span><span class="sxs-lookup"><span data-stu-id="58fa0-107">audioVideo</span></span>         | <span data-ttu-id="58fa0-108">Int64</span><span class="sxs-lookup"><span data-stu-id="58fa0-108">Int64</span></span>  |
| <span data-ttu-id="58fa0-109">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="58fa0-109">dialInOut3rdParty</span></span>  | <span data-ttu-id="58fa0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="58fa0-110">Int64</span></span>  |
| <span data-ttu-id="58fa0-111">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="58fa0-111">dialInOutMicrosoft</span></span> | <span data-ttu-id="58fa0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="58fa0-112">Int64</span></span>  |
| <span data-ttu-id="58fa0-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="58fa0-113">reportRefreshDate</span></span>  | <span data-ttu-id="58fa0-114">Date</span><span class="sxs-lookup"><span data-stu-id="58fa0-114">Date</span></span>   |
| <span data-ttu-id="58fa0-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="58fa0-115">reportDate</span></span>         | <span data-ttu-id="58fa0-116">Date</span><span class="sxs-lookup"><span data-stu-id="58fa0-116">Date</span></span>   |
| <span data-ttu-id="58fa0-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="58fa0-117">reportPeriod</span></span>       | <span data-ttu-id="58fa0-118">String</span><span class="sxs-lookup"><span data-stu-id="58fa0-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="58fa0-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58fa0-119">JSON representation</span></span>

<span data-ttu-id="58fa0-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58fa0-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024, 
  "dialInMicrosoft": 1024, 
  "dialOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
