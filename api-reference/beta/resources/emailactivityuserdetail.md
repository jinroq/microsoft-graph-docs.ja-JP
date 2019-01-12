---
title: emailActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938308"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="03964-103">emailActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03964-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="03964-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03964-104">Properties</span></span>

| <span data-ttu-id="03964-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03964-105">Property</span></span>          | <span data-ttu-id="03964-106">種類</span><span class="sxs-lookup"><span data-stu-id="03964-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="03964-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="03964-107">reportRefreshDate</span></span> | <span data-ttu-id="03964-108">日付</span><span class="sxs-lookup"><span data-stu-id="03964-108">Date</span></span>              |
| <span data-ttu-id="03964-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03964-109">userPrincipalName</span></span> | <span data-ttu-id="03964-110">String</span><span class="sxs-lookup"><span data-stu-id="03964-110">String</span></span>            |
| <span data-ttu-id="03964-111">displayName</span><span class="sxs-lookup"><span data-stu-id="03964-111">displayName</span></span>       | <span data-ttu-id="03964-112">String</span><span class="sxs-lookup"><span data-stu-id="03964-112">String</span></span>            |
| <span data-ttu-id="03964-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="03964-113">isDeleted</span></span>         | <span data-ttu-id="03964-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="03964-114">Boolean</span></span>           |
| <span data-ttu-id="03964-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="03964-115">deletedDate</span></span>       | <span data-ttu-id="03964-116">日付</span><span class="sxs-lookup"><span data-stu-id="03964-116">Date</span></span>              |
| <span data-ttu-id="03964-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="03964-117">lastActivityDate</span></span>  | <span data-ttu-id="03964-118">日付</span><span class="sxs-lookup"><span data-stu-id="03964-118">Date</span></span>              |
| <span data-ttu-id="03964-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="03964-119">sendCount</span></span>         | <span data-ttu-id="03964-120">Int64</span><span class="sxs-lookup"><span data-stu-id="03964-120">Int64</span></span>             |
| <span data-ttu-id="03964-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="03964-121">receiveCount</span></span>      | <span data-ttu-id="03964-122">Int64</span><span class="sxs-lookup"><span data-stu-id="03964-122">Int64</span></span>             |
| <span data-ttu-id="03964-123">readCount</span><span class="sxs-lookup"><span data-stu-id="03964-123">readCount</span></span>         | <span data-ttu-id="03964-124">Int64</span><span class="sxs-lookup"><span data-stu-id="03964-124">Int64</span></span>             |
| <span data-ttu-id="03964-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="03964-125">assignedProducts</span></span>  | <span data-ttu-id="03964-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="03964-126">String collection</span></span> |
| <span data-ttu-id="03964-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="03964-127">reportPeriod</span></span>      | <span data-ttu-id="03964-128">String</span><span class="sxs-lookup"><span data-stu-id="03964-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="03964-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03964-129">JSON representation</span></span>

<span data-ttu-id="03964-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="03964-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
