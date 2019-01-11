---
title: yammerGroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: f8a205c2ecd74e8543a220508e7d4110a90317cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806791"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="93453-103">yammerGroupsActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93453-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="93453-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93453-104">Properties</span></span>

| <span data-ttu-id="93453-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93453-105">Property</span></span>          | <span data-ttu-id="93453-106">種類</span><span class="sxs-lookup"><span data-stu-id="93453-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="93453-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="93453-107">reportRefreshDate</span></span> | <span data-ttu-id="93453-108">日付</span><span class="sxs-lookup"><span data-stu-id="93453-108">Date</span></span>   |
| <span data-ttu-id="93453-109">気に入られました</span><span class="sxs-lookup"><span data-stu-id="93453-109">liked</span></span>             | <span data-ttu-id="93453-110">Int64</span><span class="sxs-lookup"><span data-stu-id="93453-110">Int64</span></span>  |
| <span data-ttu-id="93453-111">転記</span><span class="sxs-lookup"><span data-stu-id="93453-111">posted</span></span>            | <span data-ttu-id="93453-112">Int64</span><span class="sxs-lookup"><span data-stu-id="93453-112">Int64</span></span>  |
| <span data-ttu-id="93453-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="93453-113">read</span></span>              | <span data-ttu-id="93453-114">Int64</span><span class="sxs-lookup"><span data-stu-id="93453-114">Int64</span></span>  |
| <span data-ttu-id="93453-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="93453-115">reportDate</span></span>        | <span data-ttu-id="93453-116">日付</span><span class="sxs-lookup"><span data-stu-id="93453-116">Date</span></span>   |
| <span data-ttu-id="93453-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="93453-117">reportPeriod</span></span>      | <span data-ttu-id="93453-118">String</span><span class="sxs-lookup"><span data-stu-id="93453-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93453-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93453-119">JSON representation</span></span>

<span data-ttu-id="93453-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="93453-120">The following is a JSON representation of the resource.</span></span>

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
