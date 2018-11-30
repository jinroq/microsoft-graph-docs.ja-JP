---
title: skypeForBusinessParticipantActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: d65d7fd9c2c3389e47a8b1f94538be158efd2642
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070216"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="d6f6a-103">skypeForBusinessParticipantActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6f6a-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d6f6a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6f6a-104">Properties</span></span>

| <span data-ttu-id="d6f6a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6f6a-105">Property</span></span>          | <span data-ttu-id="d6f6a-106">型</span><span class="sxs-lookup"><span data-stu-id="d6f6a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d6f6a-107">im</span><span class="sxs-lookup"><span data-stu-id="d6f6a-107">im</span></span>                | <span data-ttu-id="d6f6a-108">Int64</span><span class="sxs-lookup"><span data-stu-id="d6f6a-108">Int64</span></span>  |
| <span data-ttu-id="d6f6a-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="d6f6a-109">audioVideo</span></span>        | <span data-ttu-id="d6f6a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d6f6a-110">Int64</span></span>  |
| <span data-ttu-id="d6f6a-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="d6f6a-111">appSharing</span></span>        | <span data-ttu-id="d6f6a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d6f6a-112">Int64</span></span>  |
| <span data-ttu-id="d6f6a-113">web</span><span class="sxs-lookup"><span data-stu-id="d6f6a-113">web</span></span>               | <span data-ttu-id="d6f6a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d6f6a-114">Int64</span></span>  |
| <span data-ttu-id="d6f6a-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="d6f6a-115">dialInOut3rdParty</span></span> | <span data-ttu-id="d6f6a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d6f6a-116">Int64</span></span>  |
| <span data-ttu-id="d6f6a-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d6f6a-117">reportRefreshDate</span></span> | <span data-ttu-id="d6f6a-118">Date</span><span class="sxs-lookup"><span data-stu-id="d6f6a-118">Date</span></span>   |
| <span data-ttu-id="d6f6a-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="d6f6a-119">reportDate</span></span>        | <span data-ttu-id="d6f6a-120">Date</span><span class="sxs-lookup"><span data-stu-id="d6f6a-120">Date</span></span>   |
| <span data-ttu-id="d6f6a-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d6f6a-121">reportPeriod</span></span>      | <span data-ttu-id="d6f6a-122">String</span><span class="sxs-lookup"><span data-stu-id="d6f6a-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d6f6a-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6f6a-123">JSON representation</span></span>

<span data-ttu-id="d6f6a-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6f6a-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 196, 
  "appSharing": 196, 
  "web": 196, 
  "dialInOut3rdParty": 196, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
