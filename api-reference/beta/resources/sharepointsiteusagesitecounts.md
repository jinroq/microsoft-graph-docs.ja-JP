---
title: sharePointSiteUsageSiteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 913f9de5972d857b859b713298a0413d615b8991
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828127"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="55b26-103">sharePointSiteUsageSiteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55b26-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="55b26-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55b26-104">Properties</span></span>

| <span data-ttu-id="55b26-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55b26-105">Property</span></span>          | <span data-ttu-id="55b26-106">種類</span><span class="sxs-lookup"><span data-stu-id="55b26-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="55b26-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="55b26-107">reportRefreshDate</span></span> | <span data-ttu-id="55b26-108">日付</span><span class="sxs-lookup"><span data-stu-id="55b26-108">Date</span></span>   |
| <span data-ttu-id="55b26-109">ある</span><span class="sxs-lookup"><span data-stu-id="55b26-109">siteType</span></span>          | <span data-ttu-id="55b26-110">String</span><span class="sxs-lookup"><span data-stu-id="55b26-110">String</span></span> |
| <span data-ttu-id="55b26-111">total</span><span class="sxs-lookup"><span data-stu-id="55b26-111">total</span></span>             | <span data-ttu-id="55b26-112">Int64</span><span class="sxs-lookup"><span data-stu-id="55b26-112">Int64</span></span>  |
| <span data-ttu-id="55b26-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="55b26-113">active</span></span>            | <span data-ttu-id="55b26-114">Int64</span><span class="sxs-lookup"><span data-stu-id="55b26-114">Int64</span></span>  |
| <span data-ttu-id="55b26-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="55b26-115">reportDate</span></span>        | <span data-ttu-id="55b26-116">日付</span><span class="sxs-lookup"><span data-stu-id="55b26-116">Date</span></span>   |
| <span data-ttu-id="55b26-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="55b26-117">reportPeriod</span></span>      | <span data-ttu-id="55b26-118">String</span><span class="sxs-lookup"><span data-stu-id="55b26-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="55b26-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55b26-119">JSON representation</span></span>

<span data-ttu-id="55b26-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55b26-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
