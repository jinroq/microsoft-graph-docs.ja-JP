---
title: emailAppUsageVersionsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 7b4a59a1e15ddf41f0e4204efc4d3e0c6549e587
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071873"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="f286e-103">emailAppUsageVersionsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f286e-103">emailAppUsageVersionsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f286e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f286e-104">Properties</span></span>

| <span data-ttu-id="f286e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f286e-105">Property</span></span>          | <span data-ttu-id="f286e-106">型</span><span class="sxs-lookup"><span data-stu-id="f286e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f286e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f286e-107">reportRefreshDate</span></span> | <span data-ttu-id="f286e-108">Date</span><span class="sxs-lookup"><span data-stu-id="f286e-108">Date</span></span>   |
| <span data-ttu-id="f286e-109">outlook2016</span><span class="sxs-lookup"><span data-stu-id="f286e-109">outlook2016</span></span>       | <span data-ttu-id="f286e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f286e-110">Int64</span></span>  |
| <span data-ttu-id="f286e-111">outlook2013</span><span class="sxs-lookup"><span data-stu-id="f286e-111">outlook2013</span></span>       | <span data-ttu-id="f286e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f286e-112">Int64</span></span>  |
| <span data-ttu-id="f286e-113">outlook2010</span><span class="sxs-lookup"><span data-stu-id="f286e-113">outlook2010</span></span>       | <span data-ttu-id="f286e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f286e-114">Int64</span></span>  |
| <span data-ttu-id="f286e-115">outlook2007</span><span class="sxs-lookup"><span data-stu-id="f286e-115">outlook2007</span></span>       | <span data-ttu-id="f286e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f286e-116">Int64</span></span>  |
| <span data-ttu-id="f286e-117">未決定の状態</span><span class="sxs-lookup"><span data-stu-id="f286e-117">undetermined</span></span>      | <span data-ttu-id="f286e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f286e-118">Int64</span></span>  |
| <span data-ttu-id="f286e-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f286e-119">reportPeriod</span></span>      | <span data-ttu-id="f286e-120">String</span><span class="sxs-lookup"><span data-stu-id="f286e-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f286e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f286e-121">JSON representation</span></span>

<span data-ttu-id="f286e-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f286e-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String"
}
```
