---
title: sharePointSiteUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1c88cd75e1b38da87042b7b67388ef869c15ec38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584013"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a><span data-ttu-id="35585-103">sharePointSiteUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35585-103">sharePointSiteUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="35585-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35585-104">Properties</span></span>

| <span data-ttu-id="35585-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35585-105">Property</span></span>          | <span data-ttu-id="35585-106">型</span><span class="sxs-lookup"><span data-stu-id="35585-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="35585-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="35585-107">reportRefreshDate</span></span> | <span data-ttu-id="35585-108">Date</span><span class="sxs-lookup"><span data-stu-id="35585-108">Date</span></span>   |
| <span data-ttu-id="35585-109">sitetype</span><span class="sxs-lookup"><span data-stu-id="35585-109">siteType</span></span>          | <span data-ttu-id="35585-110">String</span><span class="sxs-lookup"><span data-stu-id="35585-110">String</span></span> |
| <span data-ttu-id="35585-111">total</span><span class="sxs-lookup"><span data-stu-id="35585-111">total</span></span>             | <span data-ttu-id="35585-112">Int64</span><span class="sxs-lookup"><span data-stu-id="35585-112">Int64</span></span>  |
| <span data-ttu-id="35585-113">active</span><span class="sxs-lookup"><span data-stu-id="35585-113">active</span></span>            | <span data-ttu-id="35585-114">Int64</span><span class="sxs-lookup"><span data-stu-id="35585-114">Int64</span></span>  |
| <span data-ttu-id="35585-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="35585-115">reportDate</span></span>        | <span data-ttu-id="35585-116">Date</span><span class="sxs-lookup"><span data-stu-id="35585-116">Date</span></span>   |
| <span data-ttu-id="35585-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="35585-117">reportPeriod</span></span>      | <span data-ttu-id="35585-118">String</span><span class="sxs-lookup"><span data-stu-id="35585-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35585-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35585-119">JSON representation</span></span>

<span data-ttu-id="35585-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="35585-120">The following is a JSON representation of the resource.</span></span>

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
