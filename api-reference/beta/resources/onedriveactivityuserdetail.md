---
title: oneDriveActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 2f498c7c9507c4210f12f76d57f62729f84da578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820791"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="a56de-103">oneDriveActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a56de-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a56de-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a56de-104">Properties</span></span>

| <span data-ttu-id="a56de-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a56de-105">Property</span></span>                  | <span data-ttu-id="a56de-106">種類</span><span class="sxs-lookup"><span data-stu-id="a56de-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="a56de-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a56de-107">reportRefreshDate</span></span>         | <span data-ttu-id="a56de-108">日付</span><span class="sxs-lookup"><span data-stu-id="a56de-108">Date</span></span>              |
| <span data-ttu-id="a56de-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a56de-109">userPrincipalName</span></span>         | <span data-ttu-id="a56de-110">String</span><span class="sxs-lookup"><span data-stu-id="a56de-110">String</span></span>            |
| <span data-ttu-id="a56de-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a56de-111">isDeleted</span></span>                 | <span data-ttu-id="a56de-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="a56de-112">Boolean</span></span>           |
| <span data-ttu-id="a56de-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a56de-113">deletedDate</span></span>               | <span data-ttu-id="a56de-114">日付</span><span class="sxs-lookup"><span data-stu-id="a56de-114">Date</span></span>              |
| <span data-ttu-id="a56de-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a56de-115">lastActivityDate</span></span>          | <span data-ttu-id="a56de-116">日付</span><span class="sxs-lookup"><span data-stu-id="a56de-116">Date</span></span>              |
| <span data-ttu-id="a56de-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="a56de-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="a56de-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a56de-118">Int64</span></span>             |
| <span data-ttu-id="a56de-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="a56de-119">syncedFileCount</span></span>           | <span data-ttu-id="a56de-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a56de-120">Int64</span></span>             |
| <span data-ttu-id="a56de-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a56de-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="a56de-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a56de-122">Int64</span></span>             |
| <span data-ttu-id="a56de-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a56de-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="a56de-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a56de-124">Int64</span></span>             |
| <span data-ttu-id="a56de-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="a56de-125">assignedProducts</span></span>          | <span data-ttu-id="a56de-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a56de-126">String collection</span></span> |
| <span data-ttu-id="a56de-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a56de-127">reportPeriod</span></span>              | <span data-ttu-id="a56de-128">String</span><span class="sxs-lookup"><span data-stu-id="a56de-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a56de-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a56de-129">JSON representation</span></span>

<span data-ttu-id="a56de-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a56de-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
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
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
