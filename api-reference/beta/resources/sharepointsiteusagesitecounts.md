---
title: sharePointSiteUsageSiteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d261bb6db255f9e901c7f86d0767b8dcf0121aba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970333"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a><span data-ttu-id="57e41-103">sharePointSiteUsageSiteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57e41-103">sharePointSiteUsageSiteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="57e41-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57e41-104">Properties</span></span>

| <span data-ttu-id="57e41-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57e41-105">Property</span></span>          | <span data-ttu-id="57e41-106">種類</span><span class="sxs-lookup"><span data-stu-id="57e41-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="57e41-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="57e41-107">reportRefreshDate</span></span> | <span data-ttu-id="57e41-108">日付</span><span class="sxs-lookup"><span data-stu-id="57e41-108">Date</span></span>   |
| <span data-ttu-id="57e41-109">ある</span><span class="sxs-lookup"><span data-stu-id="57e41-109">siteType</span></span>          | <span data-ttu-id="57e41-110">String</span><span class="sxs-lookup"><span data-stu-id="57e41-110">String</span></span> |
| <span data-ttu-id="57e41-111">total</span><span class="sxs-lookup"><span data-stu-id="57e41-111">total</span></span>             | <span data-ttu-id="57e41-112">Int64</span><span class="sxs-lookup"><span data-stu-id="57e41-112">Int64</span></span>  |
| <span data-ttu-id="57e41-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="57e41-113">active</span></span>            | <span data-ttu-id="57e41-114">Int64</span><span class="sxs-lookup"><span data-stu-id="57e41-114">Int64</span></span>  |
| <span data-ttu-id="57e41-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="57e41-115">reportDate</span></span>        | <span data-ttu-id="57e41-116">日付</span><span class="sxs-lookup"><span data-stu-id="57e41-116">Date</span></span>   |
| <span data-ttu-id="57e41-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="57e41-117">reportPeriod</span></span>      | <span data-ttu-id="57e41-118">String</span><span class="sxs-lookup"><span data-stu-id="57e41-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57e41-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57e41-119">JSON representation</span></span>

<span data-ttu-id="57e41-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="57e41-120">The following is a JSON representation of the resource.</span></span>

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
