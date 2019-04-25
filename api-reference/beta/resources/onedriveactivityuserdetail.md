---
title: onedrive activityuserdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582249"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="2421e-103">onedrive activityuserdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2421e-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2421e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2421e-104">Properties</span></span>

| <span data-ttu-id="2421e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2421e-105">Property</span></span>                  | <span data-ttu-id="2421e-106">型</span><span class="sxs-lookup"><span data-stu-id="2421e-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="2421e-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="2421e-107">reportRefreshDate</span></span>         | <span data-ttu-id="2421e-108">Date</span><span class="sxs-lookup"><span data-stu-id="2421e-108">Date</span></span>              |
| <span data-ttu-id="2421e-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2421e-109">userPrincipalName</span></span>         | <span data-ttu-id="2421e-110">String</span><span class="sxs-lookup"><span data-stu-id="2421e-110">String</span></span>            |
| <span data-ttu-id="2421e-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2421e-111">isDeleted</span></span>                 | <span data-ttu-id="2421e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2421e-112">Boolean</span></span>           |
| <span data-ttu-id="2421e-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="2421e-113">deletedDate</span></span>               | <span data-ttu-id="2421e-114">Date</span><span class="sxs-lookup"><span data-stu-id="2421e-114">Date</span></span>              |
| <span data-ttu-id="2421e-115">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="2421e-115">lastActivityDate</span></span>          | <span data-ttu-id="2421e-116">Date</span><span class="sxs-lookup"><span data-stu-id="2421e-116">Date</span></span>              |
| <span data-ttu-id="2421e-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="2421e-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="2421e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2421e-118">Int64</span></span>             |
| <span data-ttu-id="2421e-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="2421e-119">syncedFileCount</span></span>           | <span data-ttu-id="2421e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2421e-120">Int64</span></span>             |
| <span data-ttu-id="2421e-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="2421e-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="2421e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2421e-122">Int64</span></span>             |
| <span data-ttu-id="2421e-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="2421e-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="2421e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="2421e-124">Int64</span></span>             |
| <span data-ttu-id="2421e-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="2421e-125">assignedProducts</span></span>          | <span data-ttu-id="2421e-126">String collection</span><span class="sxs-lookup"><span data-stu-id="2421e-126">String collection</span></span> |
| <span data-ttu-id="2421e-127">reportperiod</span><span class="sxs-lookup"><span data-stu-id="2421e-127">reportPeriod</span></span>              | <span data-ttu-id="2421e-128">String</span><span class="sxs-lookup"><span data-stu-id="2421e-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="2421e-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2421e-129">JSON representation</span></span>

<span data-ttu-id="2421e-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2421e-130">The following is a JSON representation of the resource.</span></span>

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
