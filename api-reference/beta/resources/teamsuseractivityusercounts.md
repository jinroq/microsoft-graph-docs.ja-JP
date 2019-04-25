---
title: teamsuseractivityusercounts リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582914"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="f7a33-103">teamsuseractivityusercounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7a33-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f7a33-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7a33-104">Properties</span></span>

| <span data-ttu-id="f7a33-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7a33-105">Property</span></span>            | <span data-ttu-id="f7a33-106">型</span><span class="sxs-lookup"><span data-stu-id="f7a33-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="f7a33-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="f7a33-107">reportRefreshDate</span></span>   | <span data-ttu-id="f7a33-108">Date</span><span class="sxs-lookup"><span data-stu-id="f7a33-108">Date</span></span>   |
| <span data-ttu-id="f7a33-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="f7a33-109">reportDate</span></span>          | <span data-ttu-id="f7a33-110">Date</span><span class="sxs-lookup"><span data-stu-id="f7a33-110">Date</span></span>   |
| <span data-ttu-id="f7a33-111">teamchatmessages</span><span class="sxs-lookup"><span data-stu-id="f7a33-111">teamChatMessages</span></span>    | <span data-ttu-id="f7a33-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f7a33-112">Int64</span></span>  |
| <span data-ttu-id="f7a33-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="f7a33-113">privateChatMessages</span></span> | <span data-ttu-id="f7a33-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f7a33-114">Int64</span></span>  |
| <span data-ttu-id="f7a33-115">calls</span><span class="sxs-lookup"><span data-stu-id="f7a33-115">calls</span></span>               | <span data-ttu-id="f7a33-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f7a33-116">Int64</span></span>  |
| <span data-ttu-id="f7a33-117">meetings</span><span class="sxs-lookup"><span data-stu-id="f7a33-117">meetings</span></span>            | <span data-ttu-id="f7a33-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f7a33-118">Int64</span></span>  |
| <span data-ttu-id="f7a33-119">otheractions</span><span class="sxs-lookup"><span data-stu-id="f7a33-119">otherActions</span></span>        | <span data-ttu-id="f7a33-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f7a33-120">Int64</span></span>  |
| <span data-ttu-id="f7a33-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="f7a33-121">reportPeriod</span></span>        | <span data-ttu-id="f7a33-122">String</span><span class="sxs-lookup"><span data-stu-id="f7a33-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7a33-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7a33-123">JSON representation</span></span>

<span data-ttu-id="f7a33-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7a33-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
