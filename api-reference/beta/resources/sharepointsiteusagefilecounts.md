---
title: sharePointSiteUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: ade81efa7494983a7f4b3c565c0ff4f7de532f67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067145"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a><span data-ttu-id="27cf7-103">sharePointSiteUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27cf7-103">sharePointSiteUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="27cf7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27cf7-104">Properties</span></span>

| <span data-ttu-id="27cf7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27cf7-105">Property</span></span>          | <span data-ttu-id="27cf7-106">型</span><span class="sxs-lookup"><span data-stu-id="27cf7-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="27cf7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="27cf7-107">reportRefreshDate</span></span> | <span data-ttu-id="27cf7-108">Date</span><span class="sxs-lookup"><span data-stu-id="27cf7-108">Date</span></span>   |
| <span data-ttu-id="27cf7-109">ある</span><span class="sxs-lookup"><span data-stu-id="27cf7-109">siteType</span></span>          | <span data-ttu-id="27cf7-110">String</span><span class="sxs-lookup"><span data-stu-id="27cf7-110">String</span></span> |
| <span data-ttu-id="27cf7-111">total</span><span class="sxs-lookup"><span data-stu-id="27cf7-111">total</span></span>             | <span data-ttu-id="27cf7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="27cf7-112">Int64</span></span>  |
| <span data-ttu-id="27cf7-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="27cf7-113">active</span></span>            | <span data-ttu-id="27cf7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="27cf7-114">Int64</span></span>  |
| <span data-ttu-id="27cf7-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="27cf7-115">reportDate</span></span>        | <span data-ttu-id="27cf7-116">Date</span><span class="sxs-lookup"><span data-stu-id="27cf7-116">Date</span></span>   |
| <span data-ttu-id="27cf7-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="27cf7-117">reportPeriod</span></span>      | <span data-ttu-id="27cf7-118">String</span><span class="sxs-lookup"><span data-stu-id="27cf7-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="27cf7-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27cf7-119">JSON representation</span></span>

<span data-ttu-id="27cf7-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="27cf7-120">The following is a JSON representation of the resource.</span></span>

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
