---
title: sharepointactivityuserdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7dc324d821dca26ff1083f1e48c258e1955d72f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583978"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="52d66-103">sharepointactivityuserdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52d66-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="52d66-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52d66-104">Properties</span></span>

| <span data-ttu-id="52d66-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52d66-105">Property</span></span>                  | <span data-ttu-id="52d66-106">型</span><span class="sxs-lookup"><span data-stu-id="52d66-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="52d66-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="52d66-107">reportRefreshDate</span></span>         | <span data-ttu-id="52d66-108">Date</span><span class="sxs-lookup"><span data-stu-id="52d66-108">Date</span></span>              |
| <span data-ttu-id="52d66-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="52d66-109">userPrincipalName</span></span>         | <span data-ttu-id="52d66-110">String</span><span class="sxs-lookup"><span data-stu-id="52d66-110">String</span></span>            |
| <span data-ttu-id="52d66-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="52d66-111">isDeleted</span></span>                 | <span data-ttu-id="52d66-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="52d66-112">Boolean</span></span>           |
| <span data-ttu-id="52d66-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="52d66-113">deletedDate</span></span>               | <span data-ttu-id="52d66-114">Date</span><span class="sxs-lookup"><span data-stu-id="52d66-114">Date</span></span>              |
| <span data-ttu-id="52d66-115">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="52d66-115">lastActivityDate</span></span>          | <span data-ttu-id="52d66-116">Date</span><span class="sxs-lookup"><span data-stu-id="52d66-116">Date</span></span>              |
| <span data-ttu-id="52d66-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="52d66-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="52d66-118">Int64</span><span class="sxs-lookup"><span data-stu-id="52d66-118">Int64</span></span>             |
| <span data-ttu-id="52d66-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="52d66-119">syncedFileCount</span></span>           | <span data-ttu-id="52d66-120">Int64</span><span class="sxs-lookup"><span data-stu-id="52d66-120">Int64</span></span>             |
| <span data-ttu-id="52d66-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="52d66-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="52d66-122">Int64</span><span class="sxs-lookup"><span data-stu-id="52d66-122">Int64</span></span>             |
| <span data-ttu-id="52d66-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="52d66-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="52d66-124">Int64</span><span class="sxs-lookup"><span data-stu-id="52d66-124">Int64</span></span>             |
| <span data-ttu-id="52d66-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="52d66-125">visitedPageCount</span></span>          | <span data-ttu-id="52d66-126">Int64</span><span class="sxs-lookup"><span data-stu-id="52d66-126">Int64</span></span>             |
| <span data-ttu-id="52d66-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="52d66-127">assignedProducts</span></span>          | <span data-ttu-id="52d66-128">String collection</span><span class="sxs-lookup"><span data-stu-id="52d66-128">String collection</span></span> |
| <span data-ttu-id="52d66-129">reportperiod</span><span class="sxs-lookup"><span data-stu-id="52d66-129">reportPeriod</span></span>              | <span data-ttu-id="52d66-130">String</span><span class="sxs-lookup"><span data-stu-id="52d66-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="52d66-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52d66-131">JSON representation</span></span>

<span data-ttu-id="52d66-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52d66-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "visitedPageCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
