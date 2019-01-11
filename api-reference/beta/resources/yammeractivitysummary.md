---
title: yammerActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 438cb55f4682d533876ef9a01561a3d69c4f1ea2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836653"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="dca75-103">yammerActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dca75-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dca75-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dca75-104">Properties</span></span>

| <span data-ttu-id="dca75-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dca75-105">Property</span></span>          | <span data-ttu-id="dca75-106">種類</span><span class="sxs-lookup"><span data-stu-id="dca75-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="dca75-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dca75-107">reportRefreshDate</span></span> | <span data-ttu-id="dca75-108">日付</span><span class="sxs-lookup"><span data-stu-id="dca75-108">Date</span></span>   |
| <span data-ttu-id="dca75-109">気に入られました</span><span class="sxs-lookup"><span data-stu-id="dca75-109">liked</span></span>             | <span data-ttu-id="dca75-110">Int64</span><span class="sxs-lookup"><span data-stu-id="dca75-110">Int64</span></span>  |
| <span data-ttu-id="dca75-111">転記</span><span class="sxs-lookup"><span data-stu-id="dca75-111">posted</span></span>            | <span data-ttu-id="dca75-112">Int64</span><span class="sxs-lookup"><span data-stu-id="dca75-112">Int64</span></span>  |
| <span data-ttu-id="dca75-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="dca75-113">read</span></span>              | <span data-ttu-id="dca75-114">Int64</span><span class="sxs-lookup"><span data-stu-id="dca75-114">Int64</span></span>  |
| <span data-ttu-id="dca75-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="dca75-115">reportDate</span></span>        | <span data-ttu-id="dca75-116">日付</span><span class="sxs-lookup"><span data-stu-id="dca75-116">Date</span></span>   |
| <span data-ttu-id="dca75-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="dca75-117">reportPeriod</span></span>      | <span data-ttu-id="dca75-118">String</span><span class="sxs-lookup"><span data-stu-id="dca75-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dca75-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dca75-119">JSON representation</span></span>

<span data-ttu-id="dca75-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dca75-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
