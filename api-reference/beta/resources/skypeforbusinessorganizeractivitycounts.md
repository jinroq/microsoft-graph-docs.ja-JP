---
title: Skypeforbusinessオーガナイザー Eractivity計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a418d714effdc13f04c69e3371287d77cfe31c68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008139"
---
# <a name="skypeforbusinessorganizeractivitycounts-resource-type"></a><span data-ttu-id="2b7aa-103">Skypeforbusinessオーガナイザー Eractivity計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b7aa-103">skypeForBusinessOrganizerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2b7aa-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b7aa-104">Properties</span></span>

| <span data-ttu-id="2b7aa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b7aa-105">Property</span></span>           | <span data-ttu-id="2b7aa-106">型</span><span class="sxs-lookup"><span data-stu-id="2b7aa-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="2b7aa-107">im</span><span class="sxs-lookup"><span data-stu-id="2b7aa-107">im</span></span>                 | <span data-ttu-id="2b7aa-108">Int64</span><span class="sxs-lookup"><span data-stu-id="2b7aa-108">Int64</span></span>  |
| <span data-ttu-id="2b7aa-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="2b7aa-109">audioVideo</span></span>         | <span data-ttu-id="2b7aa-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2b7aa-110">Int64</span></span>  |
| <span data-ttu-id="2b7aa-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="2b7aa-111">appSharing</span></span>         | <span data-ttu-id="2b7aa-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2b7aa-112">Int64</span></span>  |
| <span data-ttu-id="2b7aa-113">Web</span><span class="sxs-lookup"><span data-stu-id="2b7aa-113">web</span></span>                | <span data-ttu-id="2b7aa-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2b7aa-114">Int64</span></span>  |
| <span data-ttu-id="2b7aa-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="2b7aa-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="2b7aa-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2b7aa-116">Int64</span></span>  |
| <span data-ttu-id="2b7aa-117">ダイヤルアウト Microsoft</span><span class="sxs-lookup"><span data-stu-id="2b7aa-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="2b7aa-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2b7aa-118">Int64</span></span>  |
| <span data-ttu-id="2b7aa-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2b7aa-119">reportRefreshDate</span></span>  | <span data-ttu-id="2b7aa-120">日付</span><span class="sxs-lookup"><span data-stu-id="2b7aa-120">Date</span></span>   |
| <span data-ttu-id="2b7aa-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="2b7aa-121">reportDate</span></span>         | <span data-ttu-id="2b7aa-122">日付</span><span class="sxs-lookup"><span data-stu-id="2b7aa-122">Date</span></span>   |
| <span data-ttu-id="2b7aa-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2b7aa-123">reportPeriod</span></span>       | <span data-ttu-id="2b7aa-124">String</span><span class="sxs-lookup"><span data-stu-id="2b7aa-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b7aa-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b7aa-125">JSON representation</span></span>

<span data-ttu-id="2b7aa-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2b7aa-126">The following is a JSON representation of the resource.</span></span>

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
