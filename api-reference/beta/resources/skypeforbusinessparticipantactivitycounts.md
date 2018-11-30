---
title: skypeForBusinessParticipantActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 1e61526b281a87370835e8f6558ab3f0cb5707a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070210"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="c0302-103">skypeForBusinessParticipantActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0302-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c0302-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0302-104">Properties</span></span>

| <span data-ttu-id="c0302-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0302-105">Property</span></span>          | <span data-ttu-id="c0302-106">型</span><span class="sxs-lookup"><span data-stu-id="c0302-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c0302-107">im</span><span class="sxs-lookup"><span data-stu-id="c0302-107">im</span></span>                | <span data-ttu-id="c0302-108">Int64</span><span class="sxs-lookup"><span data-stu-id="c0302-108">Int64</span></span>  |
| <span data-ttu-id="c0302-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="c0302-109">audioVideo</span></span>        | <span data-ttu-id="c0302-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c0302-110">Int64</span></span>  |
| <span data-ttu-id="c0302-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="c0302-111">appSharing</span></span>        | <span data-ttu-id="c0302-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c0302-112">Int64</span></span>  |
| <span data-ttu-id="c0302-113">web</span><span class="sxs-lookup"><span data-stu-id="c0302-113">web</span></span>               | <span data-ttu-id="c0302-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c0302-114">Int64</span></span>  |
| <span data-ttu-id="c0302-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="c0302-115">dialInOut3rdParty</span></span> | <span data-ttu-id="c0302-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c0302-116">Int64</span></span>  |
| <span data-ttu-id="c0302-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c0302-117">reportRefreshDate</span></span> | <span data-ttu-id="c0302-118">Date</span><span class="sxs-lookup"><span data-stu-id="c0302-118">Date</span></span>   |
| <span data-ttu-id="c0302-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="c0302-119">reportDate</span></span>        | <span data-ttu-id="c0302-120">Date</span><span class="sxs-lookup"><span data-stu-id="c0302-120">Date</span></span>   |
| <span data-ttu-id="c0302-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c0302-121">reportPeriod</span></span>      | <span data-ttu-id="c0302-122">String</span><span class="sxs-lookup"><span data-stu-id="c0302-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c0302-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0302-123">JSON representation</span></span>

<span data-ttu-id="c0302-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0302-124">The following is a JSON representation of the resource.</span></span>

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
