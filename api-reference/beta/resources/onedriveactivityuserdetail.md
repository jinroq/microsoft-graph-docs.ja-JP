---
title: oneDriveActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 679ec9b8452d388fe311e67d88bcfffd6fe73d93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069188"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="8cc8a-103">oneDriveActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cc8a-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8cc8a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cc8a-104">Properties</span></span>

| <span data-ttu-id="8cc8a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cc8a-105">Property</span></span>                  | <span data-ttu-id="8cc8a-106">型</span><span class="sxs-lookup"><span data-stu-id="8cc8a-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="8cc8a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8cc8a-107">reportRefreshDate</span></span>         | <span data-ttu-id="8cc8a-108">Date</span><span class="sxs-lookup"><span data-stu-id="8cc8a-108">Date</span></span>              |
| <span data-ttu-id="8cc8a-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8cc8a-109">userPrincipalName</span></span>         | <span data-ttu-id="8cc8a-110">String</span><span class="sxs-lookup"><span data-stu-id="8cc8a-110">String</span></span>            |
| <span data-ttu-id="8cc8a-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8cc8a-111">isDeleted</span></span>                 | <span data-ttu-id="8cc8a-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="8cc8a-112">Boolean</span></span>           |
| <span data-ttu-id="8cc8a-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8cc8a-113">deletedDate</span></span>               | <span data-ttu-id="8cc8a-114">Date</span><span class="sxs-lookup"><span data-stu-id="8cc8a-114">Date</span></span>              |
| <span data-ttu-id="8cc8a-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8cc8a-115">lastActivityDate</span></span>          | <span data-ttu-id="8cc8a-116">Date</span><span class="sxs-lookup"><span data-stu-id="8cc8a-116">Date</span></span>              |
| <span data-ttu-id="8cc8a-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="8cc8a-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="8cc8a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="8cc8a-118">Int64</span></span>             |
| <span data-ttu-id="8cc8a-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="8cc8a-119">syncedFileCount</span></span>           | <span data-ttu-id="8cc8a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8cc8a-120">Int64</span></span>             |
| <span data-ttu-id="8cc8a-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="8cc8a-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="8cc8a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8cc8a-122">Int64</span></span>             |
| <span data-ttu-id="8cc8a-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="8cc8a-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="8cc8a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8cc8a-124">Int64</span></span>             |
| <span data-ttu-id="8cc8a-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8cc8a-125">assignedProducts</span></span>          | <span data-ttu-id="8cc8a-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8cc8a-126">String collection</span></span> |
| <span data-ttu-id="8cc8a-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8cc8a-127">reportPeriod</span></span>              | <span data-ttu-id="8cc8a-128">String</span><span class="sxs-lookup"><span data-stu-id="8cc8a-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="8cc8a-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cc8a-129">JSON representation</span></span>

<span data-ttu-id="8cc8a-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8cc8a-130">The following is a JSON representation of the resource.</span></span>

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
