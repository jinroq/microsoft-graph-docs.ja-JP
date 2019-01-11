---
title: sharePointActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 4503739a7b2e13cade72951ae56ab410f22608b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880697"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="c9ce5-103">sharePointActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9ce5-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c9ce5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9ce5-104">Properties</span></span>

| <span data-ttu-id="c9ce5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9ce5-105">Property</span></span>                  | <span data-ttu-id="c9ce5-106">種類</span><span class="sxs-lookup"><span data-stu-id="c9ce5-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="c9ce5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c9ce5-107">reportRefreshDate</span></span>         | <span data-ttu-id="c9ce5-108">日付</span><span class="sxs-lookup"><span data-stu-id="c9ce5-108">Date</span></span>              |
| <span data-ttu-id="c9ce5-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c9ce5-109">userPrincipalName</span></span>         | <span data-ttu-id="c9ce5-110">String</span><span class="sxs-lookup"><span data-stu-id="c9ce5-110">String</span></span>            |
| <span data-ttu-id="c9ce5-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c9ce5-111">isDeleted</span></span>                 | <span data-ttu-id="c9ce5-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="c9ce5-112">Boolean</span></span>           |
| <span data-ttu-id="c9ce5-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="c9ce5-113">deletedDate</span></span>               | <span data-ttu-id="c9ce5-114">日付</span><span class="sxs-lookup"><span data-stu-id="c9ce5-114">Date</span></span>              |
| <span data-ttu-id="c9ce5-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c9ce5-115">lastActivityDate</span></span>          | <span data-ttu-id="c9ce5-116">日付</span><span class="sxs-lookup"><span data-stu-id="c9ce5-116">Date</span></span>              |
| <span data-ttu-id="c9ce5-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="c9ce5-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="c9ce5-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c9ce5-118">Int64</span></span>             |
| <span data-ttu-id="c9ce5-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="c9ce5-119">syncedFileCount</span></span>           | <span data-ttu-id="c9ce5-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c9ce5-120">Int64</span></span>             |
| <span data-ttu-id="c9ce5-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="c9ce5-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="c9ce5-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c9ce5-122">Int64</span></span>             |
| <span data-ttu-id="c9ce5-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="c9ce5-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="c9ce5-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c9ce5-124">Int64</span></span>             |
| <span data-ttu-id="c9ce5-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="c9ce5-125">visitedPageCount</span></span>          | <span data-ttu-id="c9ce5-126">Int64</span><span class="sxs-lookup"><span data-stu-id="c9ce5-126">Int64</span></span>             |
| <span data-ttu-id="c9ce5-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="c9ce5-127">assignedProducts</span></span>          | <span data-ttu-id="c9ce5-128">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c9ce5-128">String collection</span></span> |
| <span data-ttu-id="c9ce5-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c9ce5-129">reportPeriod</span></span>              | <span data-ttu-id="c9ce5-130">String</span><span class="sxs-lookup"><span data-stu-id="c9ce5-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c9ce5-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9ce5-131">JSON representation</span></span>

<span data-ttu-id="c9ce5-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9ce5-132">The following is a JSON representation of the resource.</span></span>

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
