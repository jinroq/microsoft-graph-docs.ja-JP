---
title: sharepointactivityusercounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9656b39572eac5b6474dd7884eb7d1d2edb17310
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583950"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="b4de9-103">sharepointactivityusercounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4de9-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b4de9-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4de9-104">Properties</span></span>

| <span data-ttu-id="b4de9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4de9-105">Property</span></span>          | <span data-ttu-id="b4de9-106">型</span><span class="sxs-lookup"><span data-stu-id="b4de9-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b4de9-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="b4de9-107">reportRefreshDate</span></span> | <span data-ttu-id="b4de9-108">Date</span><span class="sxs-lookup"><span data-stu-id="b4de9-108">Date</span></span>   |
| <span data-ttu-id="b4de9-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="b4de9-109">visitedPage</span></span>       | <span data-ttu-id="b4de9-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b4de9-110">Int64</span></span>  |
| <span data-ttu-id="b4de9-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="b4de9-111">viewedOrEdited</span></span>    | <span data-ttu-id="b4de9-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b4de9-112">Int64</span></span>  |
| <span data-ttu-id="b4de9-113">同期</span><span class="sxs-lookup"><span data-stu-id="b4de9-113">synced</span></span>            | <span data-ttu-id="b4de9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b4de9-114">Int64</span></span>  |
| <span data-ttu-id="b4de9-115">sharedinternally</span><span class="sxs-lookup"><span data-stu-id="b4de9-115">sharedInternally</span></span>  | <span data-ttu-id="b4de9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b4de9-116">Int64</span></span>  |
| <span data-ttu-id="b4de9-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="b4de9-117">sharedExternally</span></span>  | <span data-ttu-id="b4de9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b4de9-118">Int64</span></span>  |
| <span data-ttu-id="b4de9-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="b4de9-119">reportDate</span></span>        | <span data-ttu-id="b4de9-120">Date</span><span class="sxs-lookup"><span data-stu-id="b4de9-120">Date</span></span>   |
| <span data-ttu-id="b4de9-121">reportperiod</span><span class="sxs-lookup"><span data-stu-id="b4de9-121">reportPeriod</span></span>      | <span data-ttu-id="b4de9-122">String</span><span class="sxs-lookup"><span data-stu-id="b4de9-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b4de9-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4de9-123">JSON representation</span></span>

<span data-ttu-id="b4de9-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b4de9-124">The following is a JSON representation of the resource.</span></span>

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
