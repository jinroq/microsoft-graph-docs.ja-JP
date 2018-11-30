---
title: oneDriveUsageAccountDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 4b80ebc24aa45be0368dbb59d6d3e99e7adacc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071365"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="6d1b1-103">oneDriveUsageAccountDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6d1b1-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d1b1-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d1b1-104">Properties</span></span>

| <span data-ttu-id="6d1b1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d1b1-105">Property</span></span>                | <span data-ttu-id="6d1b1-106">型</span><span class="sxs-lookup"><span data-stu-id="6d1b1-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="6d1b1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d1b1-107">reportRefreshDate</span></span>       | <span data-ttu-id="6d1b1-108">Date</span><span class="sxs-lookup"><span data-stu-id="6d1b1-108">Date</span></span>    |
| <span data-ttu-id="6d1b1-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="6d1b1-109">siteUrl</span></span>                 | <span data-ttu-id="6d1b1-110">String</span><span class="sxs-lookup"><span data-stu-id="6d1b1-110">String</span></span>  |
| <span data-ttu-id="6d1b1-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="6d1b1-111">ownerDisplayName</span></span>        | <span data-ttu-id="6d1b1-112">String</span><span class="sxs-lookup"><span data-stu-id="6d1b1-112">String</span></span>  |
| <span data-ttu-id="6d1b1-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6d1b1-113">isDeleted</span></span>               | <span data-ttu-id="6d1b1-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="6d1b1-114">Boolean</span></span> |
| <span data-ttu-id="6d1b1-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6d1b1-115">lastActivityDate</span></span>        | <span data-ttu-id="6d1b1-116">Date</span><span class="sxs-lookup"><span data-stu-id="6d1b1-116">Date</span></span>    |
| <span data-ttu-id="6d1b1-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="6d1b1-117">fileCount</span></span>               | <span data-ttu-id="6d1b1-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6d1b1-118">Int64</span></span>   |
| <span data-ttu-id="6d1b1-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="6d1b1-119">activeFileCount</span></span>         | <span data-ttu-id="6d1b1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6d1b1-120">Int64</span></span>   |
| <span data-ttu-id="6d1b1-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="6d1b1-121">storageUsedInBytes</span></span>      | <span data-ttu-id="6d1b1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6d1b1-122">Int64</span></span>   |
| <span data-ttu-id="6d1b1-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="6d1b1-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="6d1b1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6d1b1-124">Int64</span></span>   |
| <span data-ttu-id="6d1b1-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d1b1-125">reportPeriod</span></span>            | <span data-ttu-id="6d1b1-126">String</span><span class="sxs-lookup"><span data-stu-id="6d1b1-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6d1b1-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6d1b1-127">JSON representation</span></span>

<span data-ttu-id="6d1b1-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d1b1-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
