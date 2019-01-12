---
title: emailAppUsageVersionsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 371352c42e870f45224999b7a618d1bb694ea512
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965286"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="ddd34-103">emailAppUsageVersionsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ddd34-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ddd34-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddd34-104">Properties</span></span>

| <span data-ttu-id="ddd34-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ddd34-105">Property</span></span>          | <span data-ttu-id="ddd34-106">種類</span><span class="sxs-lookup"><span data-stu-id="ddd34-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ddd34-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ddd34-107">reportRefreshDate</span></span> | <span data-ttu-id="ddd34-108">日付</span><span class="sxs-lookup"><span data-stu-id="ddd34-108">Date</span></span>   |
| <span data-ttu-id="ddd34-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="ddd34-109">outlook2016</span></span>       | <span data-ttu-id="ddd34-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ddd34-110">Int64</span></span>  |
| <span data-ttu-id="ddd34-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="ddd34-111">outlook2013</span></span>       | <span data-ttu-id="ddd34-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ddd34-112">Int64</span></span>  |
| <span data-ttu-id="ddd34-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="ddd34-113">outlook2010</span></span>       | <span data-ttu-id="ddd34-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ddd34-114">Int64</span></span>  |
| <span data-ttu-id="ddd34-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="ddd34-115">outlook2007</span></span>       | <span data-ttu-id="ddd34-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ddd34-116">Int64</span></span>  |
| <span data-ttu-id="ddd34-117">未決定の状態</span><span class="sxs-lookup"><span data-stu-id="ddd34-117">undetermined</span></span>      | <span data-ttu-id="ddd34-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ddd34-118">Int64</span></span>  |
| <span data-ttu-id="ddd34-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ddd34-119">reportPeriod</span></span>      | <span data-ttu-id="ddd34-120">String</span><span class="sxs-lookup"><span data-stu-id="ddd34-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ddd34-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ddd34-121">JSON representation</span></span>

<span data-ttu-id="ddd34-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ddd34-122">The following is a JSON representation of the resource.</span></span>

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
