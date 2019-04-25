---
title: yammerActivityUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541186"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="86e11-103">yammerActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86e11-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="86e11-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86e11-104">Properties</span></span>

| <span data-ttu-id="86e11-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86e11-105">Property</span></span>          | <span data-ttu-id="86e11-106">型</span><span class="sxs-lookup"><span data-stu-id="86e11-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="86e11-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="86e11-107">reportRefreshDate</span></span> | <span data-ttu-id="86e11-108">Date</span><span class="sxs-lookup"><span data-stu-id="86e11-108">Date</span></span>              |
| <span data-ttu-id="86e11-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86e11-109">userPrincipalName</span></span> | <span data-ttu-id="86e11-110">String</span><span class="sxs-lookup"><span data-stu-id="86e11-110">String</span></span>            |
| <span data-ttu-id="86e11-111">displayName</span><span class="sxs-lookup"><span data-stu-id="86e11-111">displayName</span></span>       | <span data-ttu-id="86e11-112">String</span><span class="sxs-lookup"><span data-stu-id="86e11-112">String</span></span>            |
| <span data-ttu-id="86e11-113">userState</span><span class="sxs-lookup"><span data-stu-id="86e11-113">userState</span></span>         | <span data-ttu-id="86e11-114">String</span><span class="sxs-lookup"><span data-stu-id="86e11-114">String</span></span>            |
| <span data-ttu-id="86e11-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="86e11-115">stateChangeDate</span></span>   | <span data-ttu-id="86e11-116">Date</span><span class="sxs-lookup"><span data-stu-id="86e11-116">Date</span></span>              |
| <span data-ttu-id="86e11-117">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="86e11-117">lastActivityDate</span></span>  | <span data-ttu-id="86e11-118">Date</span><span class="sxs-lookup"><span data-stu-id="86e11-118">Date</span></span>              |
| <span data-ttu-id="86e11-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="86e11-119">postedCount</span></span>       | <span data-ttu-id="86e11-120">Int64</span><span class="sxs-lookup"><span data-stu-id="86e11-120">Int64</span></span>             |
| <span data-ttu-id="86e11-121">readcount</span><span class="sxs-lookup"><span data-stu-id="86e11-121">readCount</span></span>         | <span data-ttu-id="86e11-122">Int64</span><span class="sxs-lookup"><span data-stu-id="86e11-122">Int64</span></span>             |
| <span data-ttu-id="86e11-123">dcount</span><span class="sxs-lookup"><span data-stu-id="86e11-123">likedCount</span></span>        | <span data-ttu-id="86e11-124">Int64</span><span class="sxs-lookup"><span data-stu-id="86e11-124">Int64</span></span>             |
| <span data-ttu-id="86e11-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="86e11-125">assignedProducts</span></span>  | <span data-ttu-id="86e11-126">String collection</span><span class="sxs-lookup"><span data-stu-id="86e11-126">String collection</span></span> |
| <span data-ttu-id="86e11-127">reportperiod</span><span class="sxs-lookup"><span data-stu-id="86e11-127">reportPeriod</span></span>      | <span data-ttu-id="86e11-128">String</span><span class="sxs-lookup"><span data-stu-id="86e11-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="86e11-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86e11-129">JSON representation</span></span>

<span data-ttu-id="86e11-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="86e11-130">The following is a JSON representation of the resource.</span></span>

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
