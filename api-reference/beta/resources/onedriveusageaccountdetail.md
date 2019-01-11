---
title: oneDriveUsageAccountDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 92695f509302ede4b3ce64320e8f4ed42418f7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842610"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="a8826-103">oneDriveUsageAccountDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8826-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a8826-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8826-104">Properties</span></span>

| <span data-ttu-id="a8826-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8826-105">Property</span></span>                | <span data-ttu-id="a8826-106">種類</span><span class="sxs-lookup"><span data-stu-id="a8826-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="a8826-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a8826-107">reportRefreshDate</span></span>       | <span data-ttu-id="a8826-108">日付</span><span class="sxs-lookup"><span data-stu-id="a8826-108">Date</span></span>    |
| <span data-ttu-id="a8826-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="a8826-109">siteUrl</span></span>                 | <span data-ttu-id="a8826-110">String</span><span class="sxs-lookup"><span data-stu-id="a8826-110">String</span></span>  |
| <span data-ttu-id="a8826-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="a8826-111">ownerDisplayName</span></span>        | <span data-ttu-id="a8826-112">String</span><span class="sxs-lookup"><span data-stu-id="a8826-112">String</span></span>  |
| <span data-ttu-id="a8826-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a8826-113">isDeleted</span></span>               | <span data-ttu-id="a8826-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="a8826-114">Boolean</span></span> |
| <span data-ttu-id="a8826-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a8826-115">lastActivityDate</span></span>        | <span data-ttu-id="a8826-116">日付</span><span class="sxs-lookup"><span data-stu-id="a8826-116">Date</span></span>    |
| <span data-ttu-id="a8826-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="a8826-117">fileCount</span></span>               | <span data-ttu-id="a8826-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a8826-118">Int64</span></span>   |
| <span data-ttu-id="a8826-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="a8826-119">activeFileCount</span></span>         | <span data-ttu-id="a8826-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a8826-120">Int64</span></span>   |
| <span data-ttu-id="a8826-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="a8826-121">storageUsedInBytes</span></span>      | <span data-ttu-id="a8826-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a8826-122">Int64</span></span>   |
| <span data-ttu-id="a8826-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="a8826-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="a8826-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a8826-124">Int64</span></span>   |
| <span data-ttu-id="a8826-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a8826-125">reportPeriod</span></span>            | <span data-ttu-id="a8826-126">String</span><span class="sxs-lookup"><span data-stu-id="a8826-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a8826-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8826-127">JSON representation</span></span>

<span data-ttu-id="a8826-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a8826-128">The following is a JSON representation of the resource.</span></span>

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
