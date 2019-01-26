---
title: yammerActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575829"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="0acc6-103">yammerActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0acc6-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0acc6-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0acc6-104">Properties</span></span>

| <span data-ttu-id="0acc6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0acc6-105">Property</span></span>          | <span data-ttu-id="0acc6-106">型</span><span class="sxs-lookup"><span data-stu-id="0acc6-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="0acc6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0acc6-107">reportRefreshDate</span></span> | <span data-ttu-id="0acc6-108">日付</span><span class="sxs-lookup"><span data-stu-id="0acc6-108">Date</span></span>              |
| <span data-ttu-id="0acc6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0acc6-109">userPrincipalName</span></span> | <span data-ttu-id="0acc6-110">String</span><span class="sxs-lookup"><span data-stu-id="0acc6-110">String</span></span>            |
| <span data-ttu-id="0acc6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0acc6-111">displayName</span></span>       | <span data-ttu-id="0acc6-112">String</span><span class="sxs-lookup"><span data-stu-id="0acc6-112">String</span></span>            |
| <span data-ttu-id="0acc6-113">userState</span><span class="sxs-lookup"><span data-stu-id="0acc6-113">userState</span></span>         | <span data-ttu-id="0acc6-114">String</span><span class="sxs-lookup"><span data-stu-id="0acc6-114">String</span></span>            |
| <span data-ttu-id="0acc6-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="0acc6-115">stateChangeDate</span></span>   | <span data-ttu-id="0acc6-116">日付</span><span class="sxs-lookup"><span data-stu-id="0acc6-116">Date</span></span>              |
| <span data-ttu-id="0acc6-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="0acc6-117">lastActivityDate</span></span>  | <span data-ttu-id="0acc6-118">日付</span><span class="sxs-lookup"><span data-stu-id="0acc6-118">Date</span></span>              |
| <span data-ttu-id="0acc6-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="0acc6-119">postedCount</span></span>       | <span data-ttu-id="0acc6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="0acc6-120">Int64</span></span>             |
| <span data-ttu-id="0acc6-121">readCount</span><span class="sxs-lookup"><span data-stu-id="0acc6-121">readCount</span></span>         | <span data-ttu-id="0acc6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0acc6-122">Int64</span></span>             |
| <span data-ttu-id="0acc6-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="0acc6-123">likedCount</span></span>        | <span data-ttu-id="0acc6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0acc6-124">Int64</span></span>             |
| <span data-ttu-id="0acc6-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="0acc6-125">assignedProducts</span></span>  | <span data-ttu-id="0acc6-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0acc6-126">String collection</span></span> |
| <span data-ttu-id="0acc6-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0acc6-127">reportPeriod</span></span>      | <span data-ttu-id="0acc6-128">String</span><span class="sxs-lookup"><span data-stu-id="0acc6-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="0acc6-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0acc6-129">JSON representation</span></span>

<span data-ttu-id="0acc6-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0acc6-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
