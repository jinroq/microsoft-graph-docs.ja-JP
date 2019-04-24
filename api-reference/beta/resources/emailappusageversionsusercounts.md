---
title: emailAppUsageVersionsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 371352c42e870f45224999b7a618d1bb694ea512
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506679"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="7863d-103">emailAppUsageVersionsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7863d-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7863d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7863d-104">Properties</span></span>

| <span data-ttu-id="7863d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7863d-105">Property</span></span>          | <span data-ttu-id="7863d-106">型</span><span class="sxs-lookup"><span data-stu-id="7863d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7863d-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="7863d-107">reportRefreshDate</span></span> | <span data-ttu-id="7863d-108">Date</span><span class="sxs-lookup"><span data-stu-id="7863d-108">Date</span></span>   |
| <span data-ttu-id="7863d-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="7863d-109">outlook2016</span></span>       | <span data-ttu-id="7863d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7863d-110">Int64</span></span>  |
| <span data-ttu-id="7863d-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="7863d-111">outlook2013</span></span>       | <span data-ttu-id="7863d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7863d-112">Int64</span></span>  |
| <span data-ttu-id="7863d-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="7863d-113">outlook2010</span></span>       | <span data-ttu-id="7863d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7863d-114">Int64</span></span>  |
| <span data-ttu-id="7863d-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="7863d-115">outlook2007</span></span>       | <span data-ttu-id="7863d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="7863d-116">Int64</span></span>  |
| <span data-ttu-id="7863d-117">変換</span><span class="sxs-lookup"><span data-stu-id="7863d-117">undetermined</span></span>      | <span data-ttu-id="7863d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7863d-118">Int64</span></span>  |
| <span data-ttu-id="7863d-119">reportperiod</span><span class="sxs-lookup"><span data-stu-id="7863d-119">reportPeriod</span></span>      | <span data-ttu-id="7863d-120">String</span><span class="sxs-lookup"><span data-stu-id="7863d-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7863d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7863d-121">JSON representation</span></span>

<span data-ttu-id="7863d-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7863d-122">The following is a JSON representation of the resource.</span></span>

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
