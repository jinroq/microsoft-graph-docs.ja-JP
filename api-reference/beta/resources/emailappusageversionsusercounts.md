---
title: emailAppUsageVersionsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 2aff22c0ae1d3042859f3457f398ef5d0a5ffbe7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884848"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="99b27-103">emailAppUsageVersionsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99b27-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="99b27-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99b27-104">Properties</span></span>

| <span data-ttu-id="99b27-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99b27-105">Property</span></span>          | <span data-ttu-id="99b27-106">種類</span><span class="sxs-lookup"><span data-stu-id="99b27-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="99b27-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="99b27-107">reportRefreshDate</span></span> | <span data-ttu-id="99b27-108">日付</span><span class="sxs-lookup"><span data-stu-id="99b27-108">Date</span></span>   |
| <span data-ttu-id="99b27-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="99b27-109">outlook2016</span></span>       | <span data-ttu-id="99b27-110">Int64</span><span class="sxs-lookup"><span data-stu-id="99b27-110">Int64</span></span>  |
| <span data-ttu-id="99b27-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="99b27-111">outlook2013</span></span>       | <span data-ttu-id="99b27-112">Int64</span><span class="sxs-lookup"><span data-stu-id="99b27-112">Int64</span></span>  |
| <span data-ttu-id="99b27-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="99b27-113">outlook2010</span></span>       | <span data-ttu-id="99b27-114">Int64</span><span class="sxs-lookup"><span data-stu-id="99b27-114">Int64</span></span>  |
| <span data-ttu-id="99b27-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="99b27-115">outlook2007</span></span>       | <span data-ttu-id="99b27-116">Int64</span><span class="sxs-lookup"><span data-stu-id="99b27-116">Int64</span></span>  |
| <span data-ttu-id="99b27-117">未決定の状態</span><span class="sxs-lookup"><span data-stu-id="99b27-117">undetermined</span></span>      | <span data-ttu-id="99b27-118">Int64</span><span class="sxs-lookup"><span data-stu-id="99b27-118">Int64</span></span>  |
| <span data-ttu-id="99b27-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="99b27-119">reportPeriod</span></span>      | <span data-ttu-id="99b27-120">String</span><span class="sxs-lookup"><span data-stu-id="99b27-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="99b27-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99b27-121">JSON representation</span></span>

<span data-ttu-id="99b27-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="99b27-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
