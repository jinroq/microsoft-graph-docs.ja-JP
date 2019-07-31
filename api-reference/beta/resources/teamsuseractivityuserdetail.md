---
title: teamsUserActivityUserDetail リソースの種類
description: 以下に、リソースの JSON 表記を示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbe6297388907f28f8841e0a1dcb2ec3ae788844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964355"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="8a61c-103">teamsUserActivityUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a61c-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8a61c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a61c-104">Properties</span></span>

| <span data-ttu-id="8a61c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a61c-105">Property</span></span>                | <span data-ttu-id="8a61c-106">型</span><span class="sxs-lookup"><span data-stu-id="8a61c-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="8a61c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8a61c-107">reportRefreshDate</span></span>       | <span data-ttu-id="8a61c-108">日付</span><span class="sxs-lookup"><span data-stu-id="8a61c-108">Date</span></span>              |
| <span data-ttu-id="8a61c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8a61c-109">userPrincipalName</span></span>       | <span data-ttu-id="8a61c-110">String</span><span class="sxs-lookup"><span data-stu-id="8a61c-110">String</span></span>            |
| <span data-ttu-id="8a61c-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8a61c-111">lastActivityDate</span></span>        | <span data-ttu-id="8a61c-112">日付</span><span class="sxs-lookup"><span data-stu-id="8a61c-112">Date</span></span>              |
| <span data-ttu-id="8a61c-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8a61c-113">isDeleted</span></span>               | <span data-ttu-id="8a61c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a61c-114">Boolean</span></span>           |
| <span data-ttu-id="8a61c-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="8a61c-115">deletedDate</span></span>             | <span data-ttu-id="8a61c-116">日付</span><span class="sxs-lookup"><span data-stu-id="8a61c-116">Date</span></span>              |
| <span data-ttu-id="8a61c-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="8a61c-117">assignedProducts</span></span>        | <span data-ttu-id="8a61c-118">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="8a61c-118">String collection</span></span> |
| <span data-ttu-id="8a61c-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="8a61c-119">teamChatMessageCount</span></span>    | <span data-ttu-id="8a61c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="8a61c-120">Int64</span></span>             |
| <span data-ttu-id="8a61c-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="8a61c-121">privateChatMessageCount</span></span> | <span data-ttu-id="8a61c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8a61c-122">Int64</span></span>             |
| <span data-ttu-id="8a61c-123">callCount</span><span class="sxs-lookup"><span data-stu-id="8a61c-123">callCount</span></span>               | <span data-ttu-id="8a61c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="8a61c-124">Int64</span></span>             |
| <span data-ttu-id="8a61c-125">会議数</span><span class="sxs-lookup"><span data-stu-id="8a61c-125">meetingCount</span></span>            | <span data-ttu-id="8a61c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="8a61c-126">Int64</span></span>             |
| <span data-ttu-id="8a61c-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="8a61c-127">hasOtherAction</span></span>          | <span data-ttu-id="8a61c-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a61c-128">Boolean</span></span>           |
| <span data-ttu-id="8a61c-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8a61c-129">reportPeriod</span></span>            | <span data-ttu-id="8a61c-130">String</span><span class="sxs-lookup"><span data-stu-id="8a61c-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="8a61c-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a61c-131">JSON representation</span></span>

<span data-ttu-id="8a61c-132">以下に、リソースの JSON 表記を示します。</span><span class="sxs-lookup"><span data-stu-id="8a61c-132">The following is a JSON representaion of the resource.</span></span>

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
