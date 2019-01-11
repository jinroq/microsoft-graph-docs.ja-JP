---
title: yammerActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: d7869869466dc785b92db23f8b574eb2e77dd786
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816402"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="8478c-103">yammerActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8478c-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8478c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8478c-104">Properties</span></span>

| <span data-ttu-id="8478c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8478c-105">Property</span></span>          | <span data-ttu-id="8478c-106">種類</span><span class="sxs-lookup"><span data-stu-id="8478c-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="8478c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8478c-107">reportRefreshDate</span></span> | <span data-ttu-id="8478c-108">日付</span><span class="sxs-lookup"><span data-stu-id="8478c-108">Date</span></span>              |
| <span data-ttu-id="8478c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8478c-109">userPrincipalName</span></span> | <span data-ttu-id="8478c-110">String</span><span class="sxs-lookup"><span data-stu-id="8478c-110">String</span></span>            |
| <span data-ttu-id="8478c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8478c-111">displayName</span></span>       | <span data-ttu-id="8478c-112">String</span><span class="sxs-lookup"><span data-stu-id="8478c-112">String</span></span>            |
| <span data-ttu-id="8478c-113">userState</span><span class="sxs-lookup"><span data-stu-id="8478c-113">userState</span></span>         | <span data-ttu-id="8478c-114">String</span><span class="sxs-lookup"><span data-stu-id="8478c-114">String</span></span>            |
| <span data-ttu-id="8478c-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="8478c-115">stateChangeDate</span></span>   | <span data-ttu-id="8478c-116">日付</span><span class="sxs-lookup"><span data-stu-id="8478c-116">Date</span></span>              |
| <span data-ttu-id="8478c-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8478c-117">lastActivityDate</span></span>  | <span data-ttu-id="8478c-118">日付</span><span class="sxs-lookup"><span data-stu-id="8478c-118">Date</span></span>              |
| <span data-ttu-id="8478c-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="8478c-119">postedCount</span></span>       | <span data-ttu-id="8478c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8478c-120">Int64</span></span>             |
| <span data-ttu-id="8478c-121">readCount</span><span class="sxs-lookup"><span data-stu-id="8478c-121">readCount</span></span>         | <span data-ttu-id="8478c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8478c-122">Int64</span></span>             |
| <span data-ttu-id="8478c-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="8478c-123">likedCount</span></span>        | <span data-ttu-id="8478c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8478c-124">Int64</span></span>             |
| <span data-ttu-id="8478c-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8478c-125">assignedProducts</span></span>  | <span data-ttu-id="8478c-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8478c-126">String collection</span></span> |
| <span data-ttu-id="8478c-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8478c-127">reportPeriod</span></span>      | <span data-ttu-id="8478c-128">String</span><span class="sxs-lookup"><span data-stu-id="8478c-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="8478c-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8478c-129">JSON representation</span></span>

<span data-ttu-id="8478c-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8478c-130">The following is a JSON representation of the resource.</span></span>

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
