---
title: teamsUserActivityUserDetail リソースの種類
description: リソースの JSON の representaion は、次のようにします。
author: nkramer
ms.openlocfilehash: a1f47bc52c2a0a613598ce663f16023dce208c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331942"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="831a0-103">teamsUserActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="831a0-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="831a0-104">Properties</span><span class="sxs-lookup"><span data-stu-id="831a0-104">Properties</span></span>

| <span data-ttu-id="831a0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="831a0-105">Property</span></span>                | <span data-ttu-id="831a0-106">種類</span><span class="sxs-lookup"><span data-stu-id="831a0-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="831a0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="831a0-107">reportRefreshDate</span></span>       | <span data-ttu-id="831a0-108">日付</span><span class="sxs-lookup"><span data-stu-id="831a0-108">Date</span></span>              |
| <span data-ttu-id="831a0-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="831a0-109">userPrincipalName</span></span>       | <span data-ttu-id="831a0-110">String</span><span class="sxs-lookup"><span data-stu-id="831a0-110">String</span></span>            |
| <span data-ttu-id="831a0-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="831a0-111">lastActivityDate</span></span>        | <span data-ttu-id="831a0-112">日付</span><span class="sxs-lookup"><span data-stu-id="831a0-112">Date</span></span>              |
| <span data-ttu-id="831a0-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="831a0-113">isDeleted</span></span>               | <span data-ttu-id="831a0-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="831a0-114">Boolean</span></span>           |
| <span data-ttu-id="831a0-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="831a0-115">deletedDate</span></span>             | <span data-ttu-id="831a0-116">日付</span><span class="sxs-lookup"><span data-stu-id="831a0-116">Date</span></span>              |
| <span data-ttu-id="831a0-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="831a0-117">assignedProducts</span></span>        | <span data-ttu-id="831a0-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="831a0-118">String collection</span></span> |
| <span data-ttu-id="831a0-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="831a0-119">teamChatMessageCount</span></span>    | <span data-ttu-id="831a0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="831a0-120">Int64</span></span>             |
| <span data-ttu-id="831a0-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="831a0-121">privateChatMessageCount</span></span> | <span data-ttu-id="831a0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="831a0-122">Int64</span></span>             |
| <span data-ttu-id="831a0-123">callCount</span><span class="sxs-lookup"><span data-stu-id="831a0-123">callCount</span></span>               | <span data-ttu-id="831a0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="831a0-124">Int64</span></span>             |
| <span data-ttu-id="831a0-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="831a0-125">meetingCount</span></span>            | <span data-ttu-id="831a0-126">Int64</span><span class="sxs-lookup"><span data-stu-id="831a0-126">Int64</span></span>             |
| <span data-ttu-id="831a0-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="831a0-127">hasOtherAction</span></span>          | <span data-ttu-id="831a0-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="831a0-128">Boolean</span></span>           |
| <span data-ttu-id="831a0-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="831a0-129">reportPeriod</span></span>            | <span data-ttu-id="831a0-130">String</span><span class="sxs-lookup"><span data-stu-id="831a0-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="831a0-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="831a0-131">JSON representation</span></span>

<span data-ttu-id="831a0-132">リソースの JSON の representaion は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="831a0-132">The following is a JSON representaion of the resource.</span></span>

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
