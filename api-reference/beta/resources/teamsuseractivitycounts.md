---
title: teamsUserActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 39e90b4c9dc6b9929959139ba67ddb090d143e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073133"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="20a4a-103">teamsUserActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20a4a-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="20a4a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20a4a-104">Properties</span></span>

| <span data-ttu-id="20a4a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20a4a-105">Property</span></span>            | <span data-ttu-id="20a4a-106">型</span><span class="sxs-lookup"><span data-stu-id="20a4a-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="20a4a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="20a4a-107">reportRefreshDate</span></span>   | <span data-ttu-id="20a4a-108">Date</span><span class="sxs-lookup"><span data-stu-id="20a4a-108">Date</span></span>   |
| <span data-ttu-id="20a4a-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="20a4a-109">reportDate</span></span>          | <span data-ttu-id="20a4a-110">Date</span><span class="sxs-lookup"><span data-stu-id="20a4a-110">Date</span></span>   |
| <span data-ttu-id="20a4a-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="20a4a-111">teamChatMessages</span></span>    | <span data-ttu-id="20a4a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="20a4a-112">Int64</span></span>  |
| <span data-ttu-id="20a4a-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="20a4a-113">privateChatMessages</span></span> | <span data-ttu-id="20a4a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="20a4a-114">Int64</span></span>  |
| <span data-ttu-id="20a4a-115">呼び出し</span><span class="sxs-lookup"><span data-stu-id="20a4a-115">calls</span></span>               | <span data-ttu-id="20a4a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="20a4a-116">Int64</span></span>  |
| <span data-ttu-id="20a4a-117">会議</span><span class="sxs-lookup"><span data-stu-id="20a4a-117">meetings</span></span>            | <span data-ttu-id="20a4a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="20a4a-118">Int64</span></span>  |
| <span data-ttu-id="20a4a-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="20a4a-119">reportPeriod</span></span>        | <span data-ttu-id="20a4a-120">String</span><span class="sxs-lookup"><span data-stu-id="20a4a-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="20a4a-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20a4a-121">JSON representation</span></span>

<span data-ttu-id="20a4a-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="20a4a-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
