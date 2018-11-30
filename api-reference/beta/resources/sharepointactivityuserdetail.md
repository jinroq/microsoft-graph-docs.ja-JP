---
title: sharePointActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: a5b6de8a4a9b82d9e6d34a2ae289f0c7589798ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067143"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="a4315-103">sharePointActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4315-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a4315-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4315-104">Properties</span></span>

| <span data-ttu-id="a4315-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4315-105">Property</span></span>                  | <span data-ttu-id="a4315-106">型</span><span class="sxs-lookup"><span data-stu-id="a4315-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="a4315-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a4315-107">reportRefreshDate</span></span>         | <span data-ttu-id="a4315-108">Date</span><span class="sxs-lookup"><span data-stu-id="a4315-108">Date</span></span>              |
| <span data-ttu-id="a4315-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4315-109">userPrincipalName</span></span>         | <span data-ttu-id="a4315-110">String</span><span class="sxs-lookup"><span data-stu-id="a4315-110">String</span></span>            |
| <span data-ttu-id="a4315-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a4315-111">isDeleted</span></span>                 | <span data-ttu-id="a4315-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="a4315-112">Boolean</span></span>           |
| <span data-ttu-id="a4315-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a4315-113">deletedDate</span></span>               | <span data-ttu-id="a4315-114">Date</span><span class="sxs-lookup"><span data-stu-id="a4315-114">Date</span></span>              |
| <span data-ttu-id="a4315-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a4315-115">lastActivityDate</span></span>          | <span data-ttu-id="a4315-116">Date</span><span class="sxs-lookup"><span data-stu-id="a4315-116">Date</span></span>              |
| <span data-ttu-id="a4315-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="a4315-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="a4315-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a4315-118">Int64</span></span>             |
| <span data-ttu-id="a4315-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="a4315-119">syncedFileCount</span></span>           | <span data-ttu-id="a4315-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a4315-120">Int64</span></span>             |
| <span data-ttu-id="a4315-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a4315-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="a4315-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a4315-122">Int64</span></span>             |
| <span data-ttu-id="a4315-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a4315-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="a4315-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a4315-124">Int64</span></span>             |
| <span data-ttu-id="a4315-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="a4315-125">visitedPageCount</span></span>          | <span data-ttu-id="a4315-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a4315-126">Int64</span></span>             |
| <span data-ttu-id="a4315-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="a4315-127">assignedProducts</span></span>          | <span data-ttu-id="a4315-128">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a4315-128">String collection</span></span> |
| <span data-ttu-id="a4315-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a4315-129">reportPeriod</span></span>              | <span data-ttu-id="a4315-130">String</span><span class="sxs-lookup"><span data-stu-id="a4315-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a4315-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4315-131">JSON representation</span></span>

<span data-ttu-id="a4315-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4315-132">The following is a JSON representation of the resource.</span></span>

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
