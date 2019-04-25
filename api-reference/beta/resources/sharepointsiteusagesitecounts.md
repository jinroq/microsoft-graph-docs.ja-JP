---
title: sharepointsiteusagesitecounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d261bb6db255f9e901c7f86d0767b8dcf0121aba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584020"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="1a3a3-103">sharepointsiteusagesitecounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a3a3-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1a3a3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a3a3-104">Properties</span></span>

| <span data-ttu-id="1a3a3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a3a3-105">Property</span></span>          | <span data-ttu-id="1a3a3-106">型</span><span class="sxs-lookup"><span data-stu-id="1a3a3-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1a3a3-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="1a3a3-107">reportRefreshDate</span></span> | <span data-ttu-id="1a3a3-108">Date</span><span class="sxs-lookup"><span data-stu-id="1a3a3-108">Date</span></span>   |
| <span data-ttu-id="1a3a3-109">sitetype</span><span class="sxs-lookup"><span data-stu-id="1a3a3-109">siteType</span></span>          | <span data-ttu-id="1a3a3-110">String</span><span class="sxs-lookup"><span data-stu-id="1a3a3-110">String</span></span> |
| <span data-ttu-id="1a3a3-111">total</span><span class="sxs-lookup"><span data-stu-id="1a3a3-111">total</span></span>             | <span data-ttu-id="1a3a3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1a3a3-112">Int64</span></span>  |
| <span data-ttu-id="1a3a3-113">active</span><span class="sxs-lookup"><span data-stu-id="1a3a3-113">active</span></span>            | <span data-ttu-id="1a3a3-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1a3a3-114">Int64</span></span>  |
| <span data-ttu-id="1a3a3-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="1a3a3-115">reportDate</span></span>        | <span data-ttu-id="1a3a3-116">Date</span><span class="sxs-lookup"><span data-stu-id="1a3a3-116">Date</span></span>   |
| <span data-ttu-id="1a3a3-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="1a3a3-117">reportPeriod</span></span>      | <span data-ttu-id="1a3a3-118">String</span><span class="sxs-lookup"><span data-stu-id="1a3a3-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1a3a3-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a3a3-119">JSON representation</span></span>

<span data-ttu-id="1a3a3-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a3a3-120">The following is a JSON representation of the resource.</span></span>

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
