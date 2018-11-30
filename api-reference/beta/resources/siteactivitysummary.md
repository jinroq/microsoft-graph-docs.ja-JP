---
title: siteActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 354b329f592964249590b2f551d66681f45de485
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070212"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="cb7a7-103">siteActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb7a7-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cb7a7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb7a7-104">Properties</span></span>

| <span data-ttu-id="cb7a7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb7a7-105">Property</span></span>          | <span data-ttu-id="cb7a7-106">型</span><span class="sxs-lookup"><span data-stu-id="cb7a7-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="cb7a7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cb7a7-107">reportRefreshDate</span></span> | <span data-ttu-id="cb7a7-108">Date</span><span class="sxs-lookup"><span data-stu-id="cb7a7-108">Date</span></span>   |
| <span data-ttu-id="cb7a7-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="cb7a7-109">viewedOrEdited</span></span>    | <span data-ttu-id="cb7a7-110">Int64</span><span class="sxs-lookup"><span data-stu-id="cb7a7-110">Int64</span></span>  |
| <span data-ttu-id="cb7a7-111">同期</span><span class="sxs-lookup"><span data-stu-id="cb7a7-111">synced</span></span>            | <span data-ttu-id="cb7a7-112">Int64</span><span class="sxs-lookup"><span data-stu-id="cb7a7-112">Int64</span></span>  |
| <span data-ttu-id="cb7a7-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="cb7a7-113">sharedInternally</span></span>  | <span data-ttu-id="cb7a7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="cb7a7-114">Int64</span></span>  |
| <span data-ttu-id="cb7a7-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="cb7a7-115">sharedExternally</span></span>  | <span data-ttu-id="cb7a7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="cb7a7-116">Int64</span></span>  |
| <span data-ttu-id="cb7a7-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="cb7a7-117">reportDate</span></span>        | <span data-ttu-id="cb7a7-118">Date</span><span class="sxs-lookup"><span data-stu-id="cb7a7-118">Date</span></span>   |
| <span data-ttu-id="cb7a7-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cb7a7-119">reportPeriod</span></span>      | <span data-ttu-id="cb7a7-120">String</span><span class="sxs-lookup"><span data-stu-id="cb7a7-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb7a7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb7a7-121">JSON representation</span></span>

<span data-ttu-id="cb7a7-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb7a7-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
