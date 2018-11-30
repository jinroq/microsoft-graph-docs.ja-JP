---
title: teamsUserActivityUserDetail リソースの種類
description: リソースの JSON の representaion は、次のようにします。
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073145"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="93937-103">teamsUserActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93937-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="93937-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93937-104">Properties</span></span>

| <span data-ttu-id="93937-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93937-105">Property</span></span>                | <span data-ttu-id="93937-106">型</span><span class="sxs-lookup"><span data-stu-id="93937-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="93937-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="93937-107">reportRefreshDate</span></span>       | <span data-ttu-id="93937-108">Date</span><span class="sxs-lookup"><span data-stu-id="93937-108">Date</span></span>              |
| <span data-ttu-id="93937-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="93937-109">userPrincipalName</span></span>       | <span data-ttu-id="93937-110">String</span><span class="sxs-lookup"><span data-stu-id="93937-110">String</span></span>            |
| <span data-ttu-id="93937-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="93937-111">lastActivityDate</span></span>        | <span data-ttu-id="93937-112">Date</span><span class="sxs-lookup"><span data-stu-id="93937-112">Date</span></span>              |
| <span data-ttu-id="93937-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="93937-113">isDeleted</span></span>               | <span data-ttu-id="93937-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="93937-114">Boolean</span></span>           |
| <span data-ttu-id="93937-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="93937-115">deletedDate</span></span>             | <span data-ttu-id="93937-116">Date</span><span class="sxs-lookup"><span data-stu-id="93937-116">Date</span></span>              |
| <span data-ttu-id="93937-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="93937-117">assignedProducts</span></span>        | <span data-ttu-id="93937-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="93937-118">String collection</span></span> |
| <span data-ttu-id="93937-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="93937-119">teamChatMessageCount</span></span>    | <span data-ttu-id="93937-120">Int64</span><span class="sxs-lookup"><span data-stu-id="93937-120">Int64</span></span>             |
| <span data-ttu-id="93937-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="93937-121">privateChatMessageCount</span></span> | <span data-ttu-id="93937-122">Int64</span><span class="sxs-lookup"><span data-stu-id="93937-122">Int64</span></span>             |
| <span data-ttu-id="93937-123">callCount</span><span class="sxs-lookup"><span data-stu-id="93937-123">callCount</span></span>               | <span data-ttu-id="93937-124">Int64</span><span class="sxs-lookup"><span data-stu-id="93937-124">Int64</span></span>             |
| <span data-ttu-id="93937-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="93937-125">meetingCount</span></span>            | <span data-ttu-id="93937-126">Int64</span><span class="sxs-lookup"><span data-stu-id="93937-126">Int64</span></span>             |
| <span data-ttu-id="93937-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="93937-127">hasOtherAction</span></span>          | <span data-ttu-id="93937-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="93937-128">Boolean</span></span>           |
| <span data-ttu-id="93937-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="93937-129">reportPeriod</span></span>            | <span data-ttu-id="93937-130">String</span><span class="sxs-lookup"><span data-stu-id="93937-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="93937-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93937-131">JSON representation</span></span>

<span data-ttu-id="93937-132">リソースの JSON の representaion は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="93937-132">The following is a JSON representaion of the resource.</span></span>

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
