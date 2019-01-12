---
title: teamsUserActivityUserDetail リソースの種類
description: リソースの JSON の representaion は、次のようにします。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913430"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="87b45-103">teamsUserActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="87b45-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="87b45-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87b45-104">Properties</span></span>

| <span data-ttu-id="87b45-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87b45-105">Property</span></span>                | <span data-ttu-id="87b45-106">種類</span><span class="sxs-lookup"><span data-stu-id="87b45-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="87b45-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="87b45-107">reportRefreshDate</span></span>       | <span data-ttu-id="87b45-108">日付</span><span class="sxs-lookup"><span data-stu-id="87b45-108">Date</span></span>              |
| <span data-ttu-id="87b45-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="87b45-109">userPrincipalName</span></span>       | <span data-ttu-id="87b45-110">String</span><span class="sxs-lookup"><span data-stu-id="87b45-110">String</span></span>            |
| <span data-ttu-id="87b45-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="87b45-111">lastActivityDate</span></span>        | <span data-ttu-id="87b45-112">日付</span><span class="sxs-lookup"><span data-stu-id="87b45-112">Date</span></span>              |
| <span data-ttu-id="87b45-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="87b45-113">isDeleted</span></span>               | <span data-ttu-id="87b45-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="87b45-114">Boolean</span></span>           |
| <span data-ttu-id="87b45-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="87b45-115">deletedDate</span></span>             | <span data-ttu-id="87b45-116">日付</span><span class="sxs-lookup"><span data-stu-id="87b45-116">Date</span></span>              |
| <span data-ttu-id="87b45-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="87b45-117">assignedProducts</span></span>        | <span data-ttu-id="87b45-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="87b45-118">String collection</span></span> |
| <span data-ttu-id="87b45-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="87b45-119">teamChatMessageCount</span></span>    | <span data-ttu-id="87b45-120">Int64</span><span class="sxs-lookup"><span data-stu-id="87b45-120">Int64</span></span>             |
| <span data-ttu-id="87b45-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="87b45-121">privateChatMessageCount</span></span> | <span data-ttu-id="87b45-122">Int64</span><span class="sxs-lookup"><span data-stu-id="87b45-122">Int64</span></span>             |
| <span data-ttu-id="87b45-123">callCount</span><span class="sxs-lookup"><span data-stu-id="87b45-123">callCount</span></span>               | <span data-ttu-id="87b45-124">Int64</span><span class="sxs-lookup"><span data-stu-id="87b45-124">Int64</span></span>             |
| <span data-ttu-id="87b45-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="87b45-125">meetingCount</span></span>            | <span data-ttu-id="87b45-126">Int64</span><span class="sxs-lookup"><span data-stu-id="87b45-126">Int64</span></span>             |
| <span data-ttu-id="87b45-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="87b45-127">hasOtherAction</span></span>          | <span data-ttu-id="87b45-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="87b45-128">Boolean</span></span>           |
| <span data-ttu-id="87b45-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="87b45-129">reportPeriod</span></span>            | <span data-ttu-id="87b45-130">String</span><span class="sxs-lookup"><span data-stu-id="87b45-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="87b45-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="87b45-131">JSON representation</span></span>

<span data-ttu-id="87b45-132">リソースの JSON の representaion は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="87b45-132">The following is a JSON representaion of the resource.</span></span>

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
