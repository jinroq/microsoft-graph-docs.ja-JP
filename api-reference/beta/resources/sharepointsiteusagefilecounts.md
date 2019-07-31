---
title: sharePointSiteUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 7d1c47b5149bcee4b5a77945b927bfd5d4786dda
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008363"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a><span data-ttu-id="6673a-103">sharePointSiteUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6673a-103">sharePointSiteUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6673a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6673a-104">Properties</span></span>

| <span data-ttu-id="6673a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6673a-105">Property</span></span>          | <span data-ttu-id="6673a-106">型</span><span class="sxs-lookup"><span data-stu-id="6673a-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="6673a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6673a-107">reportRefreshDate</span></span> | <span data-ttu-id="6673a-108">日付</span><span class="sxs-lookup"><span data-stu-id="6673a-108">Date</span></span>   |
| <span data-ttu-id="6673a-109">siteType</span><span class="sxs-lookup"><span data-stu-id="6673a-109">siteType</span></span>          | <span data-ttu-id="6673a-110">String</span><span class="sxs-lookup"><span data-stu-id="6673a-110">String</span></span> |
| <span data-ttu-id="6673a-111">total</span><span class="sxs-lookup"><span data-stu-id="6673a-111">total</span></span>             | <span data-ttu-id="6673a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6673a-112">Int64</span></span>  |
| <span data-ttu-id="6673a-113">active</span><span class="sxs-lookup"><span data-stu-id="6673a-113">active</span></span>            | <span data-ttu-id="6673a-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6673a-114">Int64</span></span>  |
| <span data-ttu-id="6673a-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="6673a-115">reportDate</span></span>        | <span data-ttu-id="6673a-116">日付</span><span class="sxs-lookup"><span data-stu-id="6673a-116">Date</span></span>   |
| <span data-ttu-id="6673a-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6673a-117">reportPeriod</span></span>      | <span data-ttu-id="6673a-118">String</span><span class="sxs-lookup"><span data-stu-id="6673a-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6673a-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6673a-119">JSON representation</span></span>

<span data-ttu-id="6673a-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6673a-120">The following is a JSON representation of the resource.</span></span>

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
