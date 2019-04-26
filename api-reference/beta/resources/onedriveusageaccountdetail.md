---
title: onedrive のアカウント詳細リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563547"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="6f739-103">onedrive のアカウント詳細リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f739-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6f739-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f739-104">Properties</span></span>

| <span data-ttu-id="6f739-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f739-105">Property</span></span>                | <span data-ttu-id="6f739-106">型</span><span class="sxs-lookup"><span data-stu-id="6f739-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="6f739-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="6f739-107">reportRefreshDate</span></span>       | <span data-ttu-id="6f739-108">Date</span><span class="sxs-lookup"><span data-stu-id="6f739-108">Date</span></span>    |
| <span data-ttu-id="6f739-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="6f739-109">siteUrl</span></span>                 | <span data-ttu-id="6f739-110">String</span><span class="sxs-lookup"><span data-stu-id="6f739-110">String</span></span>  |
| <span data-ttu-id="6f739-111">ownerdisplayname</span><span class="sxs-lookup"><span data-stu-id="6f739-111">ownerDisplayName</span></span>        | <span data-ttu-id="6f739-112">String</span><span class="sxs-lookup"><span data-stu-id="6f739-112">String</span></span>  |
| <span data-ttu-id="6f739-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6f739-113">isDeleted</span></span>               | <span data-ttu-id="6f739-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f739-114">Boolean</span></span> |
| <span data-ttu-id="6f739-115">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="6f739-115">lastActivityDate</span></span>        | <span data-ttu-id="6f739-116">Date</span><span class="sxs-lookup"><span data-stu-id="6f739-116">Date</span></span>    |
| <span data-ttu-id="6f739-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="6f739-117">fileCount</span></span>               | <span data-ttu-id="6f739-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6f739-118">Int64</span></span>   |
| <span data-ttu-id="6f739-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="6f739-119">activeFileCount</span></span>         | <span data-ttu-id="6f739-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6f739-120">Int64</span></span>   |
| <span data-ttu-id="6f739-121">storageused inbytes</span><span class="sxs-lookup"><span data-stu-id="6f739-121">storageUsedInBytes</span></span>      | <span data-ttu-id="6f739-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6f739-122">Int64</span></span>   |
| <span data-ttu-id="6f739-123">storageallocatedinbytes</span><span class="sxs-lookup"><span data-stu-id="6f739-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="6f739-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6f739-124">Int64</span></span>   |
| <span data-ttu-id="6f739-125">reportperiod</span><span class="sxs-lookup"><span data-stu-id="6f739-125">reportPeriod</span></span>            | <span data-ttu-id="6f739-126">String</span><span class="sxs-lookup"><span data-stu-id="6f739-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6f739-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f739-127">JSON representation</span></span>

<span data-ttu-id="6f739-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6f739-128">The following is a JSON representation of the resource.</span></span>

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
