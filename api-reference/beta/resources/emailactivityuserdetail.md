---
title: emailactivityuserdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542833"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="06660-103">emailactivityuserdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06660-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="06660-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06660-104">Properties</span></span>

| <span data-ttu-id="06660-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06660-105">Property</span></span>          | <span data-ttu-id="06660-106">型</span><span class="sxs-lookup"><span data-stu-id="06660-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="06660-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="06660-107">reportRefreshDate</span></span> | <span data-ttu-id="06660-108">Date</span><span class="sxs-lookup"><span data-stu-id="06660-108">Date</span></span>              |
| <span data-ttu-id="06660-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06660-109">userPrincipalName</span></span> | <span data-ttu-id="06660-110">String</span><span class="sxs-lookup"><span data-stu-id="06660-110">String</span></span>            |
| <span data-ttu-id="06660-111">displayName</span><span class="sxs-lookup"><span data-stu-id="06660-111">displayName</span></span>       | <span data-ttu-id="06660-112">String</span><span class="sxs-lookup"><span data-stu-id="06660-112">String</span></span>            |
| <span data-ttu-id="06660-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="06660-113">isDeleted</span></span>         | <span data-ttu-id="06660-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="06660-114">Boolean</span></span>           |
| <span data-ttu-id="06660-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="06660-115">deletedDate</span></span>       | <span data-ttu-id="06660-116">Date</span><span class="sxs-lookup"><span data-stu-id="06660-116">Date</span></span>              |
| <span data-ttu-id="06660-117">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="06660-117">lastActivityDate</span></span>  | <span data-ttu-id="06660-118">Date</span><span class="sxs-lookup"><span data-stu-id="06660-118">Date</span></span>              |
| <span data-ttu-id="06660-119">sendcount</span><span class="sxs-lookup"><span data-stu-id="06660-119">sendCount</span></span>         | <span data-ttu-id="06660-120">Int64</span><span class="sxs-lookup"><span data-stu-id="06660-120">Int64</span></span>             |
| <span data-ttu-id="06660-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="06660-121">receiveCount</span></span>      | <span data-ttu-id="06660-122">Int64</span><span class="sxs-lookup"><span data-stu-id="06660-122">Int64</span></span>             |
| <span data-ttu-id="06660-123">readcount</span><span class="sxs-lookup"><span data-stu-id="06660-123">readCount</span></span>         | <span data-ttu-id="06660-124">Int64</span><span class="sxs-lookup"><span data-stu-id="06660-124">Int64</span></span>             |
| <span data-ttu-id="06660-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="06660-125">assignedProducts</span></span>  | <span data-ttu-id="06660-126">String collection</span><span class="sxs-lookup"><span data-stu-id="06660-126">String collection</span></span> |
| <span data-ttu-id="06660-127">reportperiod</span><span class="sxs-lookup"><span data-stu-id="06660-127">reportPeriod</span></span>      | <span data-ttu-id="06660-128">String</span><span class="sxs-lookup"><span data-stu-id="06660-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="06660-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06660-129">JSON representation</span></span>

<span data-ttu-id="06660-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06660-130">The following is a JSON representation of the resource.</span></span>

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
