---
title: sharePointActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 3d1c1f1b2bcf919769009bbb65a917c4b9cb84f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008433"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="fe494-103">sharePointActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe494-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fe494-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe494-104">Properties</span></span>

| <span data-ttu-id="fe494-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe494-105">Property</span></span>                  | <span data-ttu-id="fe494-106">型</span><span class="sxs-lookup"><span data-stu-id="fe494-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="fe494-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fe494-107">reportRefreshDate</span></span>         | <span data-ttu-id="fe494-108">日付</span><span class="sxs-lookup"><span data-stu-id="fe494-108">Date</span></span>              |
| <span data-ttu-id="fe494-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe494-109">userPrincipalName</span></span>         | <span data-ttu-id="fe494-110">String</span><span class="sxs-lookup"><span data-stu-id="fe494-110">String</span></span>            |
| <span data-ttu-id="fe494-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="fe494-111">isDeleted</span></span>                 | <span data-ttu-id="fe494-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe494-112">Boolean</span></span>           |
| <span data-ttu-id="fe494-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="fe494-113">deletedDate</span></span>               | <span data-ttu-id="fe494-114">日付</span><span class="sxs-lookup"><span data-stu-id="fe494-114">Date</span></span>              |
| <span data-ttu-id="fe494-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="fe494-115">lastActivityDate</span></span>          | <span data-ttu-id="fe494-116">日付</span><span class="sxs-lookup"><span data-stu-id="fe494-116">Date</span></span>              |
| <span data-ttu-id="fe494-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="fe494-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="fe494-118">Int64</span><span class="sxs-lookup"><span data-stu-id="fe494-118">Int64</span></span>             |
| <span data-ttu-id="fe494-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="fe494-119">syncedFileCount</span></span>           | <span data-ttu-id="fe494-120">Int64</span><span class="sxs-lookup"><span data-stu-id="fe494-120">Int64</span></span>             |
| <span data-ttu-id="fe494-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="fe494-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="fe494-122">Int64</span><span class="sxs-lookup"><span data-stu-id="fe494-122">Int64</span></span>             |
| <span data-ttu-id="fe494-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="fe494-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="fe494-124">Int64</span><span class="sxs-lookup"><span data-stu-id="fe494-124">Int64</span></span>             |
| <span data-ttu-id="fe494-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="fe494-125">visitedPageCount</span></span>          | <span data-ttu-id="fe494-126">Int64</span><span class="sxs-lookup"><span data-stu-id="fe494-126">Int64</span></span>             |
| <span data-ttu-id="fe494-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="fe494-127">assignedProducts</span></span>          | <span data-ttu-id="fe494-128">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="fe494-128">String collection</span></span> |
| <span data-ttu-id="fe494-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fe494-129">reportPeriod</span></span>              | <span data-ttu-id="fe494-130">String</span><span class="sxs-lookup"><span data-stu-id="fe494-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="fe494-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe494-131">JSON representation</span></span>

<span data-ttu-id="fe494-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fe494-132">The following is a JSON representation of the resource.</span></span>

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
