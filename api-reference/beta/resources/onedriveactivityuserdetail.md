---
title: Onedrive Activityuserdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: c61db94678ed50e6cc93f123a506ce262616a1ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966483"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="ce2a5-103">Onedrive Activityuserdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce2a5-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ce2a5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce2a5-104">Properties</span></span>

| <span data-ttu-id="ce2a5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce2a5-105">Property</span></span>                  | <span data-ttu-id="ce2a5-106">型</span><span class="sxs-lookup"><span data-stu-id="ce2a5-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="ce2a5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ce2a5-107">reportRefreshDate</span></span>         | <span data-ttu-id="ce2a5-108">日付</span><span class="sxs-lookup"><span data-stu-id="ce2a5-108">Date</span></span>              |
| <span data-ttu-id="ce2a5-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ce2a5-109">userPrincipalName</span></span>         | <span data-ttu-id="ce2a5-110">String</span><span class="sxs-lookup"><span data-stu-id="ce2a5-110">String</span></span>            |
| <span data-ttu-id="ce2a5-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ce2a5-111">isDeleted</span></span>                 | <span data-ttu-id="ce2a5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce2a5-112">Boolean</span></span>           |
| <span data-ttu-id="ce2a5-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="ce2a5-113">deletedDate</span></span>               | <span data-ttu-id="ce2a5-114">日付</span><span class="sxs-lookup"><span data-stu-id="ce2a5-114">Date</span></span>              |
| <span data-ttu-id="ce2a5-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ce2a5-115">lastActivityDate</span></span>          | <span data-ttu-id="ce2a5-116">日付</span><span class="sxs-lookup"><span data-stu-id="ce2a5-116">Date</span></span>              |
| <span data-ttu-id="ce2a5-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="ce2a5-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="ce2a5-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ce2a5-118">Int64</span></span>             |
| <span data-ttu-id="ce2a5-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="ce2a5-119">syncedFileCount</span></span>           | <span data-ttu-id="ce2a5-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ce2a5-120">Int64</span></span>             |
| <span data-ttu-id="ce2a5-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="ce2a5-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="ce2a5-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ce2a5-122">Int64</span></span>             |
| <span data-ttu-id="ce2a5-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="ce2a5-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="ce2a5-124">Int64</span><span class="sxs-lookup"><span data-stu-id="ce2a5-124">Int64</span></span>             |
| <span data-ttu-id="ce2a5-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="ce2a5-125">assignedProducts</span></span>          | <span data-ttu-id="ce2a5-126">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="ce2a5-126">String collection</span></span> |
| <span data-ttu-id="ce2a5-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ce2a5-127">reportPeriod</span></span>              | <span data-ttu-id="ce2a5-128">String</span><span class="sxs-lookup"><span data-stu-id="ce2a5-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="ce2a5-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce2a5-129">JSON representation</span></span>

<span data-ttu-id="ce2a5-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce2a5-130">The following is a JSON representation of the resource.</span></span>

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
