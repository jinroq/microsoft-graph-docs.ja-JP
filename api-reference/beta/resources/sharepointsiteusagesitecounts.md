---
title: sharePointSiteUsageSiteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 96bb3c9835ea6490893c41595a89a08601e9e88c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965104"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="6317f-103">sharePointSiteUsageSiteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6317f-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6317f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6317f-104">Properties</span></span>

| <span data-ttu-id="6317f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6317f-105">Property</span></span>          | <span data-ttu-id="6317f-106">型</span><span class="sxs-lookup"><span data-stu-id="6317f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6317f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6317f-107">reportRefreshDate</span></span> | <span data-ttu-id="6317f-108">日付</span><span class="sxs-lookup"><span data-stu-id="6317f-108">Date</span></span>   |
| <span data-ttu-id="6317f-109">siteType</span><span class="sxs-lookup"><span data-stu-id="6317f-109">siteType</span></span>          | <span data-ttu-id="6317f-110">String</span><span class="sxs-lookup"><span data-stu-id="6317f-110">String</span></span> |
| <span data-ttu-id="6317f-111">total</span><span class="sxs-lookup"><span data-stu-id="6317f-111">total</span></span>             | <span data-ttu-id="6317f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6317f-112">Int64</span></span>  |
| <span data-ttu-id="6317f-113">active</span><span class="sxs-lookup"><span data-stu-id="6317f-113">active</span></span>            | <span data-ttu-id="6317f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6317f-114">Int64</span></span>  |
| <span data-ttu-id="6317f-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="6317f-115">reportDate</span></span>        | <span data-ttu-id="6317f-116">日付</span><span class="sxs-lookup"><span data-stu-id="6317f-116">Date</span></span>   |
| <span data-ttu-id="6317f-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6317f-117">reportPeriod</span></span>      | <span data-ttu-id="6317f-118">String</span><span class="sxs-lookup"><span data-stu-id="6317f-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6317f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6317f-119">JSON representation</span></span>

<span data-ttu-id="6317f-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6317f-120">The following is a JSON representation of the resource.</span></span>

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
