---
title: sharePointSiteUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: b304a5bb519f8ffb2a23087b2ea38fd12fde6fab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836128"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a><span data-ttu-id="f26bb-103">sharePointSiteUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f26bb-103">sharePointSiteUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f26bb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f26bb-104">Properties</span></span>

| <span data-ttu-id="f26bb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f26bb-105">Property</span></span>          | <span data-ttu-id="f26bb-106">種類</span><span class="sxs-lookup"><span data-stu-id="f26bb-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f26bb-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f26bb-107">reportRefreshDate</span></span> | <span data-ttu-id="f26bb-108">日付</span><span class="sxs-lookup"><span data-stu-id="f26bb-108">Date</span></span>   |
| <span data-ttu-id="f26bb-109">ある</span><span class="sxs-lookup"><span data-stu-id="f26bb-109">siteType</span></span>          | <span data-ttu-id="f26bb-110">String</span><span class="sxs-lookup"><span data-stu-id="f26bb-110">String</span></span> |
| <span data-ttu-id="f26bb-111">total</span><span class="sxs-lookup"><span data-stu-id="f26bb-111">total</span></span>             | <span data-ttu-id="f26bb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f26bb-112">Int64</span></span>  |
| <span data-ttu-id="f26bb-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="f26bb-113">active</span></span>            | <span data-ttu-id="f26bb-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f26bb-114">Int64</span></span>  |
| <span data-ttu-id="f26bb-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="f26bb-115">reportDate</span></span>        | <span data-ttu-id="f26bb-116">日付</span><span class="sxs-lookup"><span data-stu-id="f26bb-116">Date</span></span>   |
| <span data-ttu-id="f26bb-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f26bb-117">reportPeriod</span></span>      | <span data-ttu-id="f26bb-118">String</span><span class="sxs-lookup"><span data-stu-id="f26bb-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f26bb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f26bb-119">JSON representation</span></span>

<span data-ttu-id="f26bb-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f26bb-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
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
