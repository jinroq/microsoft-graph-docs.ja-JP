---
title: sharePointSiteUsageDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: b555132b2cd70d3a01e0c80fe95f0b14417c61fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861104"
---
# <a name="sharepointsiteusagedetail-resource-type"></a><span data-ttu-id="498bc-103">sharePointSiteUsageDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="498bc-103">sharePointSiteUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="498bc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="498bc-104">Properties</span></span>

| <span data-ttu-id="498bc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="498bc-105">Property</span></span>                | <span data-ttu-id="498bc-106">種類</span><span class="sxs-lookup"><span data-stu-id="498bc-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="498bc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="498bc-107">reportRefreshDate</span></span>       | <span data-ttu-id="498bc-108">日付</span><span class="sxs-lookup"><span data-stu-id="498bc-108">Date</span></span>    |
| <span data-ttu-id="498bc-109">siteId</span><span class="sxs-lookup"><span data-stu-id="498bc-109">siteId</span></span>                  | <span data-ttu-id="498bc-110">Guid</span><span class="sxs-lookup"><span data-stu-id="498bc-110">Guid</span></span>  |
| <span data-ttu-id="498bc-111">siteUrl</span><span class="sxs-lookup"><span data-stu-id="498bc-111">siteUrl</span></span>                 | <span data-ttu-id="498bc-112">String</span><span class="sxs-lookup"><span data-stu-id="498bc-112">String</span></span>  |
| <span data-ttu-id="498bc-113">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="498bc-113">ownerDisplayName</span></span>        | <span data-ttu-id="498bc-114">String</span><span class="sxs-lookup"><span data-stu-id="498bc-114">String</span></span>  |
| <span data-ttu-id="498bc-115">isDeleted</span><span class="sxs-lookup"><span data-stu-id="498bc-115">isDeleted</span></span>               | <span data-ttu-id="498bc-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="498bc-116">Boolean</span></span> |
| <span data-ttu-id="498bc-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="498bc-117">lastActivityDate</span></span>        | <span data-ttu-id="498bc-118">日付</span><span class="sxs-lookup"><span data-stu-id="498bc-118">Date</span></span>    |
| <span data-ttu-id="498bc-119">fileCount</span><span class="sxs-lookup"><span data-stu-id="498bc-119">fileCount</span></span>               | <span data-ttu-id="498bc-120">Int64</span><span class="sxs-lookup"><span data-stu-id="498bc-120">Int64</span></span>   |
| <span data-ttu-id="498bc-121">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="498bc-121">activeFileCount</span></span>         | <span data-ttu-id="498bc-122">Int64</span><span class="sxs-lookup"><span data-stu-id="498bc-122">Int64</span></span>   |
| <span data-ttu-id="498bc-123">pageViewCount</span><span class="sxs-lookup"><span data-stu-id="498bc-123">pageViewCount</span></span>           | <span data-ttu-id="498bc-124">Int64</span><span class="sxs-lookup"><span data-stu-id="498bc-124">Int64</span></span>   |
| <span data-ttu-id="498bc-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="498bc-125">visitedPageCount</span></span>        | <span data-ttu-id="498bc-126">Int64</span><span class="sxs-lookup"><span data-stu-id="498bc-126">Int64</span></span>   |
| <span data-ttu-id="498bc-127">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="498bc-127">storageUsedInBytes</span></span>      | <span data-ttu-id="498bc-128">Int64</span><span class="sxs-lookup"><span data-stu-id="498bc-128">Int64</span></span>   |
| <span data-ttu-id="498bc-129">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="498bc-129">storageAllocatedInBytes</span></span> | <span data-ttu-id="498bc-130">Int64</span><span class="sxs-lookup"><span data-stu-id="498bc-130">Int64</span></span>   |
| <span data-ttu-id="498bc-131">rootWebTemplate</span><span class="sxs-lookup"><span data-stu-id="498bc-131">rootWebTemplate</span></span>         | <span data-ttu-id="498bc-132">String</span><span class="sxs-lookup"><span data-stu-id="498bc-132">String</span></span>  |
| <span data-ttu-id="498bc-133">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="498bc-133">reportPeriod</span></span>            | <span data-ttu-id="498bc-134">String</span><span class="sxs-lookup"><span data-stu-id="498bc-134">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="498bc-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="498bc-135">JSON representation</span></span>

<span data-ttu-id="498bc-136">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="498bc-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteId": "Guid", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "pageViewCount": 1024, 
  "visitedPageCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "rootWebTemplate": "String", 
  "reportPeriod": "String"
}
```
