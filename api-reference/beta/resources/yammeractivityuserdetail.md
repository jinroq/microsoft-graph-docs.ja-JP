---
title: yammerActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: a1ca33efe8327b1c1e52de25714df9c0bd45ee05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072466"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="d6150-103">yammerActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6150-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d6150-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6150-104">Properties</span></span>

| <span data-ttu-id="d6150-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6150-105">Property</span></span>          | <span data-ttu-id="d6150-106">型</span><span class="sxs-lookup"><span data-stu-id="d6150-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="d6150-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d6150-107">reportRefreshDate</span></span> | <span data-ttu-id="d6150-108">Date</span><span class="sxs-lookup"><span data-stu-id="d6150-108">Date</span></span>              |
| <span data-ttu-id="d6150-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6150-109">userPrincipalName</span></span> | <span data-ttu-id="d6150-110">String</span><span class="sxs-lookup"><span data-stu-id="d6150-110">String</span></span>            |
| <span data-ttu-id="d6150-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d6150-111">displayName</span></span>       | <span data-ttu-id="d6150-112">String</span><span class="sxs-lookup"><span data-stu-id="d6150-112">String</span></span>            |
| <span data-ttu-id="d6150-113">userState</span><span class="sxs-lookup"><span data-stu-id="d6150-113">userState</span></span>         | <span data-ttu-id="d6150-114">String</span><span class="sxs-lookup"><span data-stu-id="d6150-114">String</span></span>            |
| <span data-ttu-id="d6150-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="d6150-115">stateChangeDate</span></span>   | <span data-ttu-id="d6150-116">Date</span><span class="sxs-lookup"><span data-stu-id="d6150-116">Date</span></span>              |
| <span data-ttu-id="d6150-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d6150-117">lastActivityDate</span></span>  | <span data-ttu-id="d6150-118">Date</span><span class="sxs-lookup"><span data-stu-id="d6150-118">Date</span></span>              |
| <span data-ttu-id="d6150-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="d6150-119">postedCount</span></span>       | <span data-ttu-id="d6150-120">Int64</span><span class="sxs-lookup"><span data-stu-id="d6150-120">Int64</span></span>             |
| <span data-ttu-id="d6150-121">readCount</span><span class="sxs-lookup"><span data-stu-id="d6150-121">readCount</span></span>         | <span data-ttu-id="d6150-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d6150-122">Int64</span></span>             |
| <span data-ttu-id="d6150-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="d6150-123">likedCount</span></span>        | <span data-ttu-id="d6150-124">Int64</span><span class="sxs-lookup"><span data-stu-id="d6150-124">Int64</span></span>             |
| <span data-ttu-id="d6150-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="d6150-125">assignedProducts</span></span>  | <span data-ttu-id="d6150-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d6150-126">String collection</span></span> |
| <span data-ttu-id="d6150-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d6150-127">reportPeriod</span></span>      | <span data-ttu-id="d6150-128">String</span><span class="sxs-lookup"><span data-stu-id="d6150-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="d6150-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6150-129">JSON representation</span></span>

<span data-ttu-id="d6150-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6150-130">The following is a JSON representation of the resource.</span></span>

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
