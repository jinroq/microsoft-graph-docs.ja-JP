---
title: oneDriveUsageAccountDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957397"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="f4a98-103">oneDriveUsageAccountDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4a98-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f4a98-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4a98-104">Properties</span></span>

| <span data-ttu-id="f4a98-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4a98-105">Property</span></span>                | <span data-ttu-id="f4a98-106">種類</span><span class="sxs-lookup"><span data-stu-id="f4a98-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="f4a98-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f4a98-107">reportRefreshDate</span></span>       | <span data-ttu-id="f4a98-108">日付</span><span class="sxs-lookup"><span data-stu-id="f4a98-108">Date</span></span>    |
| <span data-ttu-id="f4a98-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="f4a98-109">siteUrl</span></span>                 | <span data-ttu-id="f4a98-110">String</span><span class="sxs-lookup"><span data-stu-id="f4a98-110">String</span></span>  |
| <span data-ttu-id="f4a98-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4a98-111">ownerDisplayName</span></span>        | <span data-ttu-id="f4a98-112">String</span><span class="sxs-lookup"><span data-stu-id="f4a98-112">String</span></span>  |
| <span data-ttu-id="f4a98-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f4a98-113">isDeleted</span></span>               | <span data-ttu-id="f4a98-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="f4a98-114">Boolean</span></span> |
| <span data-ttu-id="f4a98-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f4a98-115">lastActivityDate</span></span>        | <span data-ttu-id="f4a98-116">日付</span><span class="sxs-lookup"><span data-stu-id="f4a98-116">Date</span></span>    |
| <span data-ttu-id="f4a98-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="f4a98-117">fileCount</span></span>               | <span data-ttu-id="f4a98-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f4a98-118">Int64</span></span>   |
| <span data-ttu-id="f4a98-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="f4a98-119">activeFileCount</span></span>         | <span data-ttu-id="f4a98-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f4a98-120">Int64</span></span>   |
| <span data-ttu-id="f4a98-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="f4a98-121">storageUsedInBytes</span></span>      | <span data-ttu-id="f4a98-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f4a98-122">Int64</span></span>   |
| <span data-ttu-id="f4a98-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="f4a98-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="f4a98-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f4a98-124">Int64</span></span>   |
| <span data-ttu-id="f4a98-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f4a98-125">reportPeriod</span></span>            | <span data-ttu-id="f4a98-126">String</span><span class="sxs-lookup"><span data-stu-id="f4a98-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f4a98-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4a98-127">JSON representation</span></span>

<span data-ttu-id="f4a98-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4a98-128">The following is a JSON representation of the resource.</span></span>

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
