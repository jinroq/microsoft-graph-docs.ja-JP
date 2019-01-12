---
title: oneDriveActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948248"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="8f760-103">oneDriveActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f760-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8f760-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f760-104">Properties</span></span>

| <span data-ttu-id="8f760-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f760-105">Property</span></span>                  | <span data-ttu-id="8f760-106">種類</span><span class="sxs-lookup"><span data-stu-id="8f760-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="8f760-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8f760-107">reportRefreshDate</span></span>         | <span data-ttu-id="8f760-108">日付</span><span class="sxs-lookup"><span data-stu-id="8f760-108">Date</span></span>              |
| <span data-ttu-id="8f760-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8f760-109">userPrincipalName</span></span>         | <span data-ttu-id="8f760-110">String</span><span class="sxs-lookup"><span data-stu-id="8f760-110">String</span></span>            |
| <span data-ttu-id="8f760-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8f760-111">isDeleted</span></span>                 | <span data-ttu-id="8f760-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="8f760-112">Boolean</span></span>           |
| <span data-ttu-id="8f760-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8f760-113">deletedDate</span></span>               | <span data-ttu-id="8f760-114">日付</span><span class="sxs-lookup"><span data-stu-id="8f760-114">Date</span></span>              |
| <span data-ttu-id="8f760-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8f760-115">lastActivityDate</span></span>          | <span data-ttu-id="8f760-116">日付</span><span class="sxs-lookup"><span data-stu-id="8f760-116">Date</span></span>              |
| <span data-ttu-id="8f760-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="8f760-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="8f760-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8f760-118">Int64</span></span>             |
| <span data-ttu-id="8f760-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="8f760-119">syncedFileCount</span></span>           | <span data-ttu-id="8f760-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8f760-120">Int64</span></span>             |
| <span data-ttu-id="8f760-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="8f760-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="8f760-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8f760-122">Int64</span></span>             |
| <span data-ttu-id="8f760-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="8f760-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="8f760-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8f760-124">Int64</span></span>             |
| <span data-ttu-id="8f760-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8f760-125">assignedProducts</span></span>          | <span data-ttu-id="8f760-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8f760-126">String collection</span></span> |
| <span data-ttu-id="8f760-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8f760-127">reportPeriod</span></span>              | <span data-ttu-id="8f760-128">String</span><span class="sxs-lookup"><span data-stu-id="8f760-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="8f760-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f760-129">JSON representation</span></span>

<span data-ttu-id="8f760-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8f760-130">The following is a JSON representation of the resource.</span></span>

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
