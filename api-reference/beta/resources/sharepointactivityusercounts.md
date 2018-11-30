---
title: sharePointActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 271ea6a70d56c55cf5a9561c2a1485c674a365f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069776"
---
# <a name="sharepointactivityusercounts-resource-type"></a><span data-ttu-id="45261-103">sharePointActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45261-103">sharePointActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="45261-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45261-104">Properties</span></span>

| <span data-ttu-id="45261-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45261-105">Property</span></span>          | <span data-ttu-id="45261-106">型</span><span class="sxs-lookup"><span data-stu-id="45261-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="45261-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="45261-107">reportRefreshDate</span></span> | <span data-ttu-id="45261-108">Date</span><span class="sxs-lookup"><span data-stu-id="45261-108">Date</span></span>   |
| <span data-ttu-id="45261-109">visitedPage</span><span class="sxs-lookup"><span data-stu-id="45261-109">visitedPage</span></span>       | <span data-ttu-id="45261-110">Int64</span><span class="sxs-lookup"><span data-stu-id="45261-110">Int64</span></span>  |
| <span data-ttu-id="45261-111">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="45261-111">viewedOrEdited</span></span>    | <span data-ttu-id="45261-112">Int64</span><span class="sxs-lookup"><span data-stu-id="45261-112">Int64</span></span>  |
| <span data-ttu-id="45261-113">同期</span><span class="sxs-lookup"><span data-stu-id="45261-113">synced</span></span>            | <span data-ttu-id="45261-114">Int64</span><span class="sxs-lookup"><span data-stu-id="45261-114">Int64</span></span>  |
| <span data-ttu-id="45261-115">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="45261-115">sharedInternally</span></span>  | <span data-ttu-id="45261-116">Int64</span><span class="sxs-lookup"><span data-stu-id="45261-116">Int64</span></span>  |
| <span data-ttu-id="45261-117">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="45261-117">sharedExternally</span></span>  | <span data-ttu-id="45261-118">Int64</span><span class="sxs-lookup"><span data-stu-id="45261-118">Int64</span></span>  |
| <span data-ttu-id="45261-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="45261-119">reportDate</span></span>        | <span data-ttu-id="45261-120">Date</span><span class="sxs-lookup"><span data-stu-id="45261-120">Date</span></span>   |
| <span data-ttu-id="45261-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="45261-121">reportPeriod</span></span>      | <span data-ttu-id="45261-122">String</span><span class="sxs-lookup"><span data-stu-id="45261-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45261-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45261-123">JSON representation</span></span>

<span data-ttu-id="45261-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="45261-124">The following is a JSON representation of the resource.</span></span>

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
