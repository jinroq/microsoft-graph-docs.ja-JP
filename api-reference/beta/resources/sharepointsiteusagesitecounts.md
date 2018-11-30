---
title: sharePointSiteUsageSiteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 631e01a417e177e356b701ca8dc93ffa51b4f50f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068116"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="ebb89-103">sharePointSiteUsageSiteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebb89-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ebb89-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebb89-104">Properties</span></span>

| <span data-ttu-id="ebb89-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebb89-105">Property</span></span>          | <span data-ttu-id="ebb89-106">型</span><span class="sxs-lookup"><span data-stu-id="ebb89-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ebb89-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ebb89-107">reportRefreshDate</span></span> | <span data-ttu-id="ebb89-108">Date</span><span class="sxs-lookup"><span data-stu-id="ebb89-108">Date</span></span>   |
| <span data-ttu-id="ebb89-109">ある</span><span class="sxs-lookup"><span data-stu-id="ebb89-109">siteType</span></span>          | <span data-ttu-id="ebb89-110">String</span><span class="sxs-lookup"><span data-stu-id="ebb89-110">String</span></span> |
| <span data-ttu-id="ebb89-111">total</span><span class="sxs-lookup"><span data-stu-id="ebb89-111">total</span></span>             | <span data-ttu-id="ebb89-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ebb89-112">Int64</span></span>  |
| <span data-ttu-id="ebb89-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="ebb89-113">active</span></span>            | <span data-ttu-id="ebb89-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ebb89-114">Int64</span></span>  |
| <span data-ttu-id="ebb89-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="ebb89-115">reportDate</span></span>        | <span data-ttu-id="ebb89-116">Date</span><span class="sxs-lookup"><span data-stu-id="ebb89-116">Date</span></span>   |
| <span data-ttu-id="ebb89-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ebb89-117">reportPeriod</span></span>      | <span data-ttu-id="ebb89-118">String</span><span class="sxs-lookup"><span data-stu-id="ebb89-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ebb89-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ebb89-119">JSON representation</span></span>

<span data-ttu-id="ebb89-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ebb89-120">The following is a JSON representation of the resource.</span></span>

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
