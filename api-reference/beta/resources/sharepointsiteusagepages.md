---
title: sharePointSiteUsagePages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 625dc6ff15a7a9efb8a2b2b545fcc78a4e7e9407
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865640"
---
# <a name="sharepointsiteusagepages-resource-type"></a><span data-ttu-id="f1224-103">sharePointSiteUsagePages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1224-103">sharePointSiteUsagePages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f1224-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1224-104">Properties</span></span>

| <span data-ttu-id="f1224-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1224-105">Property</span></span>          | <span data-ttu-id="f1224-106">種類</span><span class="sxs-lookup"><span data-stu-id="f1224-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f1224-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f1224-107">reportRefreshDate</span></span> | <span data-ttu-id="f1224-108">日付</span><span class="sxs-lookup"><span data-stu-id="f1224-108">Date</span></span>   |
| <span data-ttu-id="f1224-109">ある</span><span class="sxs-lookup"><span data-stu-id="f1224-109">siteType</span></span>          | <span data-ttu-id="f1224-110">String</span><span class="sxs-lookup"><span data-stu-id="f1224-110">String</span></span> |
| <span data-ttu-id="f1224-111">pageViewCount</span><span class="sxs-lookup"><span data-stu-id="f1224-111">pageViewCount</span></span>     | <span data-ttu-id="f1224-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f1224-112">Int64</span></span>  |
| <span data-ttu-id="f1224-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="f1224-113">reportDate</span></span>        | <span data-ttu-id="f1224-114">日付</span><span class="sxs-lookup"><span data-stu-id="f1224-114">Date</span></span>   |
| <span data-ttu-id="f1224-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f1224-115">reportPeriod</span></span>      | <span data-ttu-id="f1224-116">String</span><span class="sxs-lookup"><span data-stu-id="f1224-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1224-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1224-117">JSON representation</span></span>

<span data-ttu-id="f1224-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1224-118">The following is a JSON representation of the resource.</span></span>

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
