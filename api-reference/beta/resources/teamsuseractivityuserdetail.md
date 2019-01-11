---
title: teamsUserActivityUserDetail リソースの種類
description: リソースの JSON の representaion は、次のようにします。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2e3f64c7065343712f6a9d9c6a114bf95f24c171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823654"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="42f17-103">teamsUserActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42f17-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="42f17-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42f17-104">Properties</span></span>

| <span data-ttu-id="42f17-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42f17-105">Property</span></span>                | <span data-ttu-id="42f17-106">種類</span><span class="sxs-lookup"><span data-stu-id="42f17-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="42f17-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="42f17-107">reportRefreshDate</span></span>       | <span data-ttu-id="42f17-108">日付</span><span class="sxs-lookup"><span data-stu-id="42f17-108">Date</span></span>              |
| <span data-ttu-id="42f17-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42f17-109">userPrincipalName</span></span>       | <span data-ttu-id="42f17-110">String</span><span class="sxs-lookup"><span data-stu-id="42f17-110">String</span></span>            |
| <span data-ttu-id="42f17-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="42f17-111">lastActivityDate</span></span>        | <span data-ttu-id="42f17-112">日付</span><span class="sxs-lookup"><span data-stu-id="42f17-112">Date</span></span>              |
| <span data-ttu-id="42f17-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="42f17-113">isDeleted</span></span>               | <span data-ttu-id="42f17-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="42f17-114">Boolean</span></span>           |
| <span data-ttu-id="42f17-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="42f17-115">deletedDate</span></span>             | <span data-ttu-id="42f17-116">日付</span><span class="sxs-lookup"><span data-stu-id="42f17-116">Date</span></span>              |
| <span data-ttu-id="42f17-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="42f17-117">assignedProducts</span></span>        | <span data-ttu-id="42f17-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="42f17-118">String collection</span></span> |
| <span data-ttu-id="42f17-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="42f17-119">teamChatMessageCount</span></span>    | <span data-ttu-id="42f17-120">Int64</span><span class="sxs-lookup"><span data-stu-id="42f17-120">Int64</span></span>             |
| <span data-ttu-id="42f17-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="42f17-121">privateChatMessageCount</span></span> | <span data-ttu-id="42f17-122">Int64</span><span class="sxs-lookup"><span data-stu-id="42f17-122">Int64</span></span>             |
| <span data-ttu-id="42f17-123">callCount</span><span class="sxs-lookup"><span data-stu-id="42f17-123">callCount</span></span>               | <span data-ttu-id="42f17-124">Int64</span><span class="sxs-lookup"><span data-stu-id="42f17-124">Int64</span></span>             |
| <span data-ttu-id="42f17-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="42f17-125">meetingCount</span></span>            | <span data-ttu-id="42f17-126">Int64</span><span class="sxs-lookup"><span data-stu-id="42f17-126">Int64</span></span>             |
| <span data-ttu-id="42f17-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="42f17-127">hasOtherAction</span></span>          | <span data-ttu-id="42f17-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="42f17-128">Boolean</span></span>           |
| <span data-ttu-id="42f17-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="42f17-129">reportPeriod</span></span>            | <span data-ttu-id="42f17-130">String</span><span class="sxs-lookup"><span data-stu-id="42f17-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="42f17-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42f17-131">JSON representation</span></span>

<span data-ttu-id="42f17-132">リソースの JSON の representaion は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="42f17-132">The following is a JSON representaion of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
