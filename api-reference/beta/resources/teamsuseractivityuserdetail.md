---
title: teamsuseractivityuserdetail リソースの種類
description: 以下に、リソースの JSON 表記を示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582907"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="efd52-103">teamsuseractivityuserdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="efd52-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="efd52-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efd52-104">Properties</span></span>

| <span data-ttu-id="efd52-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="efd52-105">Property</span></span>                | <span data-ttu-id="efd52-106">型</span><span class="sxs-lookup"><span data-stu-id="efd52-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="efd52-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="efd52-107">reportRefreshDate</span></span>       | <span data-ttu-id="efd52-108">Date</span><span class="sxs-lookup"><span data-stu-id="efd52-108">Date</span></span>              |
| <span data-ttu-id="efd52-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="efd52-109">userPrincipalName</span></span>       | <span data-ttu-id="efd52-110">String</span><span class="sxs-lookup"><span data-stu-id="efd52-110">String</span></span>            |
| <span data-ttu-id="efd52-111">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="efd52-111">lastActivityDate</span></span>        | <span data-ttu-id="efd52-112">Date</span><span class="sxs-lookup"><span data-stu-id="efd52-112">Date</span></span>              |
| <span data-ttu-id="efd52-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="efd52-113">isDeleted</span></span>               | <span data-ttu-id="efd52-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="efd52-114">Boolean</span></span>           |
| <span data-ttu-id="efd52-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="efd52-115">deletedDate</span></span>             | <span data-ttu-id="efd52-116">Date</span><span class="sxs-lookup"><span data-stu-id="efd52-116">Date</span></span>              |
| <span data-ttu-id="efd52-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="efd52-117">assignedProducts</span></span>        | <span data-ttu-id="efd52-118">String collection</span><span class="sxs-lookup"><span data-stu-id="efd52-118">String collection</span></span> |
| <span data-ttu-id="efd52-119">teamchatmessagecount</span><span class="sxs-lookup"><span data-stu-id="efd52-119">teamChatMessageCount</span></span>    | <span data-ttu-id="efd52-120">Int64</span><span class="sxs-lookup"><span data-stu-id="efd52-120">Int64</span></span>             |
| <span data-ttu-id="efd52-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="efd52-121">privateChatMessageCount</span></span> | <span data-ttu-id="efd52-122">Int64</span><span class="sxs-lookup"><span data-stu-id="efd52-122">Int64</span></span>             |
| <span data-ttu-id="efd52-123">callcount</span><span class="sxs-lookup"><span data-stu-id="efd52-123">callCount</span></span>               | <span data-ttu-id="efd52-124">Int64</span><span class="sxs-lookup"><span data-stu-id="efd52-124">Int64</span></span>             |
| <span data-ttu-id="efd52-125">会議数</span><span class="sxs-lookup"><span data-stu-id="efd52-125">meetingCount</span></span>            | <span data-ttu-id="efd52-126">Int64</span><span class="sxs-lookup"><span data-stu-id="efd52-126">Int64</span></span>             |
| <span data-ttu-id="efd52-127">hasotheraction</span><span class="sxs-lookup"><span data-stu-id="efd52-127">hasOtherAction</span></span>          | <span data-ttu-id="efd52-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="efd52-128">Boolean</span></span>           |
| <span data-ttu-id="efd52-129">reportperiod</span><span class="sxs-lookup"><span data-stu-id="efd52-129">reportPeriod</span></span>            | <span data-ttu-id="efd52-130">String</span><span class="sxs-lookup"><span data-stu-id="efd52-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="efd52-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="efd52-131">JSON representation</span></span>

<span data-ttu-id="efd52-132">以下に、リソースの JSON 表記を示します。</span><span class="sxs-lookup"><span data-stu-id="efd52-132">The following is a JSON representaion of the resource.</span></span>

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
