---
title: skypeforbusinessオーガナイザー eractivity計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 9f6c77e86f76ac2e34fb87cf8ca5b6bded35a2a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461160"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="a1b4d-103">skypeforbusinessオーガナイザー eractivity計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1b4d-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a1b4d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1b4d-104">Properties</span></span>

| <span data-ttu-id="a1b4d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1b4d-105">Property</span></span>           | <span data-ttu-id="a1b4d-106">型</span><span class="sxs-lookup"><span data-stu-id="a1b4d-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="a1b4d-107">im</span><span class="sxs-lookup"><span data-stu-id="a1b4d-107">im</span></span>                 | <span data-ttu-id="a1b4d-108">Int64</span><span class="sxs-lookup"><span data-stu-id="a1b4d-108">Int64</span></span>  |
| <span data-ttu-id="a1b4d-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="a1b4d-109">audioVideo</span></span>         | <span data-ttu-id="a1b4d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a1b4d-110">Int64</span></span>  |
| <span data-ttu-id="a1b4d-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="a1b4d-111">appSharing</span></span>         | <span data-ttu-id="a1b4d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a1b4d-112">Int64</span></span>  |
| <span data-ttu-id="a1b4d-113">web</span><span class="sxs-lookup"><span data-stu-id="a1b4d-113">web</span></span>                | <span data-ttu-id="a1b4d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a1b4d-114">Int64</span></span>  |
| <span data-ttu-id="a1b4d-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="a1b4d-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="a1b4d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a1b4d-116">Int64</span></span>  |
| <span data-ttu-id="a1b4d-117">ダイヤルアウト microsoft</span><span class="sxs-lookup"><span data-stu-id="a1b4d-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="a1b4d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a1b4d-118">Int64</span></span>  |
| <span data-ttu-id="a1b4d-119">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="a1b4d-119">reportRefreshDate</span></span>  | <span data-ttu-id="a1b4d-120">Date</span><span class="sxs-lookup"><span data-stu-id="a1b4d-120">Date</span></span>   |
| <span data-ttu-id="a1b4d-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="a1b4d-121">reportDate</span></span>         | <span data-ttu-id="a1b4d-122">Date</span><span class="sxs-lookup"><span data-stu-id="a1b4d-122">Date</span></span>   |
| <span data-ttu-id="a1b4d-123">reportperiod</span><span class="sxs-lookup"><span data-stu-id="a1b4d-123">reportPeriod</span></span>       | <span data-ttu-id="a1b4d-124">String</span><span class="sxs-lookup"><span data-stu-id="a1b4d-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1b4d-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1b4d-125">JSON representation</span></span>

<span data-ttu-id="a1b4d-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1b4d-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts"
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
