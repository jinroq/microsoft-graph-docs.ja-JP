---
title: skypeforbusinessオーガナイザー eractivityuser計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 39ab5844adb9525b4e0f100892927d200609040c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534865"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="1061a-103">skypeforbusinessオーガナイザー eractivityuser計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1061a-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1061a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1061a-104">Properties</span></span>

| <span data-ttu-id="1061a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1061a-105">Property</span></span>           | <span data-ttu-id="1061a-106">型</span><span class="sxs-lookup"><span data-stu-id="1061a-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="1061a-107">im</span><span class="sxs-lookup"><span data-stu-id="1061a-107">im</span></span>                 | <span data-ttu-id="1061a-108">Int64</span><span class="sxs-lookup"><span data-stu-id="1061a-108">Int64</span></span>  |
| <span data-ttu-id="1061a-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="1061a-109">audioVideo</span></span>         | <span data-ttu-id="1061a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1061a-110">Int64</span></span>  |
| <span data-ttu-id="1061a-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="1061a-111">appSharing</span></span>         | <span data-ttu-id="1061a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1061a-112">Int64</span></span>  |
| <span data-ttu-id="1061a-113">web</span><span class="sxs-lookup"><span data-stu-id="1061a-113">web</span></span>                | <span data-ttu-id="1061a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1061a-114">Int64</span></span>  |
| <span data-ttu-id="1061a-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="1061a-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="1061a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1061a-116">Int64</span></span>  |
| <span data-ttu-id="1061a-117">ダイヤルアウト microsoft</span><span class="sxs-lookup"><span data-stu-id="1061a-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="1061a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1061a-118">Int64</span></span>  |
| <span data-ttu-id="1061a-119">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="1061a-119">reportRefreshDate</span></span>  | <span data-ttu-id="1061a-120">Date</span><span class="sxs-lookup"><span data-stu-id="1061a-120">Date</span></span>   |
| <span data-ttu-id="1061a-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="1061a-121">reportDate</span></span>         | <span data-ttu-id="1061a-122">Date</span><span class="sxs-lookup"><span data-stu-id="1061a-122">Date</span></span>   |
| <span data-ttu-id="1061a-123">reportperiod</span><span class="sxs-lookup"><span data-stu-id="1061a-123">reportPeriod</span></span>       | <span data-ttu-id="1061a-124">String</span><span class="sxs-lookup"><span data-stu-id="1061a-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1061a-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1061a-125">JSON representation</span></span>

<span data-ttu-id="1061a-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1061a-126">The following is a JSON representation of the resource.</span></span>

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
