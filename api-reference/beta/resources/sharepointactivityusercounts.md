---
title: sharePointActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9656b39572eac5b6474dd7884eb7d1d2edb17310
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984725"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="46e90-103">sharePointActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46e90-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="46e90-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46e90-104">Properties</span></span>

| <span data-ttu-id="46e90-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46e90-105">Property</span></span>          | <span data-ttu-id="46e90-106">種類</span><span class="sxs-lookup"><span data-stu-id="46e90-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="46e90-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="46e90-107">reportRefreshDate</span></span> | <span data-ttu-id="46e90-108">日付</span><span class="sxs-lookup"><span data-stu-id="46e90-108">Date</span></span>   |
| <span data-ttu-id="46e90-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="46e90-109">visitedPage</span></span>       | <span data-ttu-id="46e90-110">Int64</span><span class="sxs-lookup"><span data-stu-id="46e90-110">Int64</span></span>  |
| <span data-ttu-id="46e90-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="46e90-111">viewedOrEdited</span></span>    | <span data-ttu-id="46e90-112">Int64</span><span class="sxs-lookup"><span data-stu-id="46e90-112">Int64</span></span>  |
| <span data-ttu-id="46e90-113">同期</span><span class="sxs-lookup"><span data-stu-id="46e90-113">synced</span></span>            | <span data-ttu-id="46e90-114">Int64</span><span class="sxs-lookup"><span data-stu-id="46e90-114">Int64</span></span>  |
| <span data-ttu-id="46e90-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="46e90-115">sharedInternally</span></span>  | <span data-ttu-id="46e90-116">Int64</span><span class="sxs-lookup"><span data-stu-id="46e90-116">Int64</span></span>  |
| <span data-ttu-id="46e90-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="46e90-117">sharedExternally</span></span>  | <span data-ttu-id="46e90-118">Int64</span><span class="sxs-lookup"><span data-stu-id="46e90-118">Int64</span></span>  |
| <span data-ttu-id="46e90-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="46e90-119">reportDate</span></span>        | <span data-ttu-id="46e90-120">日付</span><span class="sxs-lookup"><span data-stu-id="46e90-120">Date</span></span>   |
| <span data-ttu-id="46e90-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="46e90-121">reportPeriod</span></span>      | <span data-ttu-id="46e90-122">String</span><span class="sxs-lookup"><span data-stu-id="46e90-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="46e90-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46e90-123">JSON representation</span></span>

<span data-ttu-id="46e90-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="46e90-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPage": 1024, 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
