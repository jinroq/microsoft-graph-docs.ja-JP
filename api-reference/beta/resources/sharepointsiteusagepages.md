---
title: sharePointSiteUsagePages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1a82c0a1174559db6d90e64f1fd1ed1403caa048
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950446"
---
# <a name="sharepointsiteusagepages-resource-type"></a><span data-ttu-id="f588b-103">sharePointSiteUsagePages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f588b-103">sharePointSiteUsagePages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f588b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f588b-104">Properties</span></span>

| <span data-ttu-id="f588b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f588b-105">Property</span></span>          | <span data-ttu-id="f588b-106">種類</span><span class="sxs-lookup"><span data-stu-id="f588b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f588b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f588b-107">reportRefreshDate</span></span> | <span data-ttu-id="f588b-108">日付</span><span class="sxs-lookup"><span data-stu-id="f588b-108">Date</span></span>   |
| <span data-ttu-id="f588b-109">ある</span><span class="sxs-lookup"><span data-stu-id="f588b-109">siteType</span></span>          | <span data-ttu-id="f588b-110">String</span><span class="sxs-lookup"><span data-stu-id="f588b-110">String</span></span> |
| <span data-ttu-id="f588b-111">pageViewCount</span><span class="sxs-lookup"><span data-stu-id="f588b-111">pageViewCount</span></span>     | <span data-ttu-id="f588b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f588b-112">Int64</span></span>  |
| <span data-ttu-id="f588b-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="f588b-113">reportDate</span></span>        | <span data-ttu-id="f588b-114">日付</span><span class="sxs-lookup"><span data-stu-id="f588b-114">Date</span></span>   |
| <span data-ttu-id="f588b-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f588b-115">reportPeriod</span></span>      | <span data-ttu-id="f588b-116">String</span><span class="sxs-lookup"><span data-stu-id="f588b-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f588b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f588b-117">JSON representation</span></span>

<span data-ttu-id="f588b-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f588b-118">The following is a JSON representation of the resource.</span></span>

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
