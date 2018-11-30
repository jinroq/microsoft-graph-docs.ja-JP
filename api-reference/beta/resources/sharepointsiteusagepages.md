---
title: sharePointSiteUsagePages リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: c66a41393f1842a66c8e57c3d9ba77e6cf863cfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066511"
---
# <a name="sharepointsiteusagepages-resource-type"></a><span data-ttu-id="f2168-103">sharePointSiteUsagePages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2168-103">sharePointSiteUsagePages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f2168-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2168-104">Properties</span></span>

| <span data-ttu-id="f2168-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2168-105">Property</span></span>          | <span data-ttu-id="f2168-106">型</span><span class="sxs-lookup"><span data-stu-id="f2168-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f2168-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f2168-107">reportRefreshDate</span></span> | <span data-ttu-id="f2168-108">Date</span><span class="sxs-lookup"><span data-stu-id="f2168-108">Date</span></span>   |
| <span data-ttu-id="f2168-109">ある</span><span class="sxs-lookup"><span data-stu-id="f2168-109">siteType</span></span>          | <span data-ttu-id="f2168-110">String</span><span class="sxs-lookup"><span data-stu-id="f2168-110">String</span></span> |
| <span data-ttu-id="f2168-111">pageViewCount</span><span class="sxs-lookup"><span data-stu-id="f2168-111">pageViewCount</span></span>     | <span data-ttu-id="f2168-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f2168-112">Int64</span></span>  |
| <span data-ttu-id="f2168-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="f2168-113">reportDate</span></span>        | <span data-ttu-id="f2168-114">Date</span><span class="sxs-lookup"><span data-stu-id="f2168-114">Date</span></span>   |
| <span data-ttu-id="f2168-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f2168-115">reportPeriod</span></span>      | <span data-ttu-id="f2168-116">String</span><span class="sxs-lookup"><span data-stu-id="f2168-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2168-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2168-117">JSON representation</span></span>

<span data-ttu-id="f2168-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2168-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "pageViewCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
