---
title: skypeForBusinessActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: e59bd33b1709780bac9726ee716ef9d81ef33c1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810130"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="55edb-103">skypeForBusinessActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55edb-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="55edb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55edb-104">Properties</span></span>

| <span data-ttu-id="55edb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55edb-105">Property</span></span>          | <span data-ttu-id="55edb-106">種類</span><span class="sxs-lookup"><span data-stu-id="55edb-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="55edb-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="55edb-107">peerToPeer</span></span>        | <span data-ttu-id="55edb-108">Int64</span><span class="sxs-lookup"><span data-stu-id="55edb-108">Int64</span></span>  |
| <span data-ttu-id="55edb-109">編成</span><span class="sxs-lookup"><span data-stu-id="55edb-109">organized</span></span>         | <span data-ttu-id="55edb-110">Int64</span><span class="sxs-lookup"><span data-stu-id="55edb-110">Int64</span></span>  |
| <span data-ttu-id="55edb-111">参加</span><span class="sxs-lookup"><span data-stu-id="55edb-111">participated</span></span>      | <span data-ttu-id="55edb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="55edb-112">Int64</span></span>  |
| <span data-ttu-id="55edb-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="55edb-113">reportRefreshDate</span></span> | <span data-ttu-id="55edb-114">日付</span><span class="sxs-lookup"><span data-stu-id="55edb-114">Date</span></span>   |
| <span data-ttu-id="55edb-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="55edb-115">reportDate</span></span>        | <span data-ttu-id="55edb-116">日付</span><span class="sxs-lookup"><span data-stu-id="55edb-116">Date</span></span>   |
| <span data-ttu-id="55edb-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="55edb-117">reportPeriod</span></span>      | <span data-ttu-id="55edb-118">String</span><span class="sxs-lookup"><span data-stu-id="55edb-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="55edb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55edb-119">JSON representation</span></span>

<span data-ttu-id="55edb-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55edb-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
