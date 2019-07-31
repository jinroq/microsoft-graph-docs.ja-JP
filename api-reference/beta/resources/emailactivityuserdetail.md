---
title: emailActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: cd78b80d97a6dfcaa4c7b97085e89daa4f8a8523
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972202"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="545f2-103">emailActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="545f2-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="545f2-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="545f2-104">Properties</span></span>

| <span data-ttu-id="545f2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="545f2-105">Property</span></span>          | <span data-ttu-id="545f2-106">型</span><span class="sxs-lookup"><span data-stu-id="545f2-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="545f2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="545f2-107">reportRefreshDate</span></span> | <span data-ttu-id="545f2-108">日付</span><span class="sxs-lookup"><span data-stu-id="545f2-108">Date</span></span>              |
| <span data-ttu-id="545f2-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="545f2-109">userPrincipalName</span></span> | <span data-ttu-id="545f2-110">String</span><span class="sxs-lookup"><span data-stu-id="545f2-110">String</span></span>            |
| <span data-ttu-id="545f2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="545f2-111">displayName</span></span>       | <span data-ttu-id="545f2-112">文字列</span><span class="sxs-lookup"><span data-stu-id="545f2-112">String</span></span>            |
| <span data-ttu-id="545f2-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="545f2-113">isDeleted</span></span>         | <span data-ttu-id="545f2-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="545f2-114">Boolean</span></span>           |
| <span data-ttu-id="545f2-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="545f2-115">deletedDate</span></span>       | <span data-ttu-id="545f2-116">日付</span><span class="sxs-lookup"><span data-stu-id="545f2-116">Date</span></span>              |
| <span data-ttu-id="545f2-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="545f2-117">lastActivityDate</span></span>  | <span data-ttu-id="545f2-118">日付</span><span class="sxs-lookup"><span data-stu-id="545f2-118">Date</span></span>              |
| <span data-ttu-id="545f2-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="545f2-119">sendCount</span></span>         | <span data-ttu-id="545f2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="545f2-120">Int64</span></span>             |
| <span data-ttu-id="545f2-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="545f2-121">receiveCount</span></span>      | <span data-ttu-id="545f2-122">Int64</span><span class="sxs-lookup"><span data-stu-id="545f2-122">Int64</span></span>             |
| <span data-ttu-id="545f2-123">readCount</span><span class="sxs-lookup"><span data-stu-id="545f2-123">readCount</span></span>         | <span data-ttu-id="545f2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="545f2-124">Int64</span></span>             |
| <span data-ttu-id="545f2-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="545f2-125">assignedProducts</span></span>  | <span data-ttu-id="545f2-126">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="545f2-126">String collection</span></span> |
| <span data-ttu-id="545f2-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="545f2-127">reportPeriod</span></span>      | <span data-ttu-id="545f2-128">String</span><span class="sxs-lookup"><span data-stu-id="545f2-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="545f2-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="545f2-129">JSON representation</span></span>

<span data-ttu-id="545f2-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="545f2-130">The following is a JSON representation of the resource.</span></span>

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
