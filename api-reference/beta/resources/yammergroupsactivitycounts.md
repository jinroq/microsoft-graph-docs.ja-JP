---
title: yammerGroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: a308b6180eaf91614247b0b5f47064ae7e7de2b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073143"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="6e0cf-103">yammerGroupsActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e0cf-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6e0cf-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e0cf-104">Properties</span></span>

| <span data-ttu-id="6e0cf-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e0cf-105">Property</span></span>          | <span data-ttu-id="6e0cf-106">型</span><span class="sxs-lookup"><span data-stu-id="6e0cf-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6e0cf-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6e0cf-107">reportRefreshDate</span></span> | <span data-ttu-id="6e0cf-108">Date</span><span class="sxs-lookup"><span data-stu-id="6e0cf-108">Date</span></span>   |
| <span data-ttu-id="6e0cf-109">気に入られました</span><span class="sxs-lookup"><span data-stu-id="6e0cf-109">liked</span></span>             | <span data-ttu-id="6e0cf-110">Int64</span><span class="sxs-lookup"><span data-stu-id="6e0cf-110">Int64</span></span>  |
| <span data-ttu-id="6e0cf-111">転記</span><span class="sxs-lookup"><span data-stu-id="6e0cf-111">posted</span></span>            | <span data-ttu-id="6e0cf-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6e0cf-112">Int64</span></span>  |
| <span data-ttu-id="6e0cf-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="6e0cf-113">read</span></span>              | <span data-ttu-id="6e0cf-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6e0cf-114">Int64</span></span>  |
| <span data-ttu-id="6e0cf-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="6e0cf-115">reportDate</span></span>        | <span data-ttu-id="6e0cf-116">Date</span><span class="sxs-lookup"><span data-stu-id="6e0cf-116">Date</span></span>   |
| <span data-ttu-id="6e0cf-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6e0cf-117">reportPeriod</span></span>      | <span data-ttu-id="6e0cf-118">String</span><span class="sxs-lookup"><span data-stu-id="6e0cf-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e0cf-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e0cf-119">JSON representation</span></span>

<span data-ttu-id="6e0cf-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e0cf-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
