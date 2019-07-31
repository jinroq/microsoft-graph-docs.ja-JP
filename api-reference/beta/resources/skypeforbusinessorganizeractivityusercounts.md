---
title: Skypeforbusinessオーガナイザー Eractivityuser計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b6fcb2114e78bd9aabb170795b49d80bb58e6844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964873"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="f6b87-103">Skypeforbusinessオーガナイザー Eractivityuser計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f6b87-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f6b87-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6b87-104">Properties</span></span>

| <span data-ttu-id="f6b87-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6b87-105">Property</span></span>           | <span data-ttu-id="f6b87-106">型</span><span class="sxs-lookup"><span data-stu-id="f6b87-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="f6b87-107">im</span><span class="sxs-lookup"><span data-stu-id="f6b87-107">im</span></span>                 | <span data-ttu-id="f6b87-108">Int64</span><span class="sxs-lookup"><span data-stu-id="f6b87-108">Int64</span></span>  |
| <span data-ttu-id="f6b87-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="f6b87-109">audioVideo</span></span>         | <span data-ttu-id="f6b87-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f6b87-110">Int64</span></span>  |
| <span data-ttu-id="f6b87-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="f6b87-111">appSharing</span></span>         | <span data-ttu-id="f6b87-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f6b87-112">Int64</span></span>  |
| <span data-ttu-id="f6b87-113">Web</span><span class="sxs-lookup"><span data-stu-id="f6b87-113">web</span></span>                | <span data-ttu-id="f6b87-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f6b87-114">Int64</span></span>  |
| <span data-ttu-id="f6b87-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="f6b87-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="f6b87-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f6b87-116">Int64</span></span>  |
| <span data-ttu-id="f6b87-117">ダイヤルアウト Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6b87-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="f6b87-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f6b87-118">Int64</span></span>  |
| <span data-ttu-id="f6b87-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f6b87-119">reportRefreshDate</span></span>  | <span data-ttu-id="f6b87-120">日付</span><span class="sxs-lookup"><span data-stu-id="f6b87-120">Date</span></span>   |
| <span data-ttu-id="f6b87-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="f6b87-121">reportDate</span></span>         | <span data-ttu-id="f6b87-122">日付</span><span class="sxs-lookup"><span data-stu-id="f6b87-122">Date</span></span>   |
| <span data-ttu-id="f6b87-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f6b87-123">reportPeriod</span></span>       | <span data-ttu-id="f6b87-124">String</span><span class="sxs-lookup"><span data-stu-id="f6b87-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f6b87-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f6b87-125">JSON representation</span></span>

<span data-ttu-id="f6b87-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6b87-126">The following is a JSON representation of the resource.</span></span>

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
