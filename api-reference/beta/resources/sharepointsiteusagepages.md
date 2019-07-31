---
title: Sharepointsiteの Pages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 7e3e1d463faddf823c49c58b4278f3812644cc9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008314"
---
# <a name="sharepointsiteusagepages-resource-type"></a><span data-ttu-id="11697-103">Sharepointsiteの Pages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="11697-103">sharePointSiteUsagePages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="11697-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11697-104">Properties</span></span>

| <span data-ttu-id="11697-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="11697-105">Property</span></span>          | <span data-ttu-id="11697-106">型</span><span class="sxs-lookup"><span data-stu-id="11697-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="11697-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="11697-107">reportRefreshDate</span></span> | <span data-ttu-id="11697-108">日付</span><span class="sxs-lookup"><span data-stu-id="11697-108">Date</span></span>   |
| <span data-ttu-id="11697-109">siteType</span><span class="sxs-lookup"><span data-stu-id="11697-109">siteType</span></span>          | <span data-ttu-id="11697-110">String</span><span class="sxs-lookup"><span data-stu-id="11697-110">String</span></span> |
| <span data-ttu-id="11697-111">pageViewCount</span><span class="sxs-lookup"><span data-stu-id="11697-111">pageViewCount</span></span>     | <span data-ttu-id="11697-112">Int64</span><span class="sxs-lookup"><span data-stu-id="11697-112">Int64</span></span>  |
| <span data-ttu-id="11697-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="11697-113">reportDate</span></span>        | <span data-ttu-id="11697-114">日付</span><span class="sxs-lookup"><span data-stu-id="11697-114">Date</span></span>   |
| <span data-ttu-id="11697-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="11697-115">reportPeriod</span></span>      | <span data-ttu-id="11697-116">String</span><span class="sxs-lookup"><span data-stu-id="11697-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="11697-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="11697-117">JSON representation</span></span>

<span data-ttu-id="11697-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="11697-118">The following is a JSON representation of the resource.</span></span>

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
