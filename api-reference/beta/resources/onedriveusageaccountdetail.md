---
title: Onedrive のアカウント詳細リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bcf75fad8c39a543e69fc378546a2621f24eaeab
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344928"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="a1bb3-103">Onedrive のアカウント詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1bb3-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a1bb3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1bb3-104">Properties</span></span>

| <span data-ttu-id="a1bb3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1bb3-105">Property</span></span>                | <span data-ttu-id="a1bb3-106">型</span><span class="sxs-lookup"><span data-stu-id="a1bb3-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="a1bb3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a1bb3-107">reportRefreshDate</span></span>       | <span data-ttu-id="a1bb3-108">日付</span><span class="sxs-lookup"><span data-stu-id="a1bb3-108">Date</span></span>    |
| <span data-ttu-id="a1bb3-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="a1bb3-109">siteUrl</span></span>                 | <span data-ttu-id="a1bb3-110">String</span><span class="sxs-lookup"><span data-stu-id="a1bb3-110">String</span></span>  |
| <span data-ttu-id="a1bb3-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1bb3-111">ownerDisplayName</span></span>        | <span data-ttu-id="a1bb3-112">String</span><span class="sxs-lookup"><span data-stu-id="a1bb3-112">String</span></span>  |
| <span data-ttu-id="a1bb3-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a1bb3-113">ownerPrincipalName</span></span>      | <span data-ttu-id="a1bb3-114">String</span><span class="sxs-lookup"><span data-stu-id="a1bb3-114">String</span></span>  |
| <span data-ttu-id="a1bb3-115">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a1bb3-115">isDeleted</span></span>               | <span data-ttu-id="a1bb3-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1bb3-116">Boolean</span></span> |
| <span data-ttu-id="a1bb3-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a1bb3-117">lastActivityDate</span></span>        | <span data-ttu-id="a1bb3-118">日付</span><span class="sxs-lookup"><span data-stu-id="a1bb3-118">Date</span></span>    |
| <span data-ttu-id="a1bb3-119">fileCount</span><span class="sxs-lookup"><span data-stu-id="a1bb3-119">fileCount</span></span>               | <span data-ttu-id="a1bb3-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a1bb3-120">Int64</span></span>   |
| <span data-ttu-id="a1bb3-121">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="a1bb3-121">activeFileCount</span></span>         | <span data-ttu-id="a1bb3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a1bb3-122">Int64</span></span>   |
| <span data-ttu-id="a1bb3-123">Storageused Inbytes</span><span class="sxs-lookup"><span data-stu-id="a1bb3-123">storageUsedInBytes</span></span>      | <span data-ttu-id="a1bb3-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a1bb3-124">Int64</span></span>   |
| <span data-ttu-id="a1bb3-125">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="a1bb3-125">storageAllocatedInBytes</span></span> | <span data-ttu-id="a1bb3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a1bb3-126">Int64</span></span>   |
| <span data-ttu-id="a1bb3-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a1bb3-127">reportPeriod</span></span>            | <span data-ttu-id="a1bb3-128">String</span><span class="sxs-lookup"><span data-stu-id="a1bb3-128">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a1bb3-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1bb3-129">JSON representation</span></span>

<span data-ttu-id="a1bb3-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1bb3-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "ownerPrincipalName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
