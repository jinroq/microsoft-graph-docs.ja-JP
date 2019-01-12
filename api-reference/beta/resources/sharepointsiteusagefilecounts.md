---
title: sharePointSiteUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1c88cd75e1b38da87042b7b67388ef869c15ec38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950432"
---
# <a name="sharepointsiteusagefilecounts-resource-type"></a><span data-ttu-id="1a45e-103">sharePointSiteUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a45e-103">sharePointSiteUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1a45e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a45e-104">Properties</span></span>

| <span data-ttu-id="1a45e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a45e-105">Property</span></span>          | <span data-ttu-id="1a45e-106">種類</span><span class="sxs-lookup"><span data-stu-id="1a45e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1a45e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1a45e-107">reportRefreshDate</span></span> | <span data-ttu-id="1a45e-108">日付</span><span class="sxs-lookup"><span data-stu-id="1a45e-108">Date</span></span>   |
| <span data-ttu-id="1a45e-109">ある</span><span class="sxs-lookup"><span data-stu-id="1a45e-109">siteType</span></span>          | <span data-ttu-id="1a45e-110">String</span><span class="sxs-lookup"><span data-stu-id="1a45e-110">String</span></span> |
| <span data-ttu-id="1a45e-111">total</span><span class="sxs-lookup"><span data-stu-id="1a45e-111">total</span></span>             | <span data-ttu-id="1a45e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1a45e-112">Int64</span></span>  |
| <span data-ttu-id="1a45e-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="1a45e-113">active</span></span>            | <span data-ttu-id="1a45e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1a45e-114">Int64</span></span>  |
| <span data-ttu-id="1a45e-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="1a45e-115">reportDate</span></span>        | <span data-ttu-id="1a45e-116">日付</span><span class="sxs-lookup"><span data-stu-id="1a45e-116">Date</span></span>   |
| <span data-ttu-id="1a45e-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1a45e-117">reportPeriod</span></span>      | <span data-ttu-id="1a45e-118">String</span><span class="sxs-lookup"><span data-stu-id="1a45e-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1a45e-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a45e-119">JSON representation</span></span>

<span data-ttu-id="1a45e-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1a45e-120">The following is a JSON representation of the resource.</span></span>

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
