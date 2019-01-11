---
title: emailActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 82fbdc2621b9c8746ed3028fe44414edeb7e56db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871345"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="c7af4-103">emailActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7af4-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c7af4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7af4-104">Properties</span></span>

| <span data-ttu-id="c7af4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7af4-105">Property</span></span>          | <span data-ttu-id="c7af4-106">種類</span><span class="sxs-lookup"><span data-stu-id="c7af4-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c7af4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c7af4-107">reportRefreshDate</span></span> | <span data-ttu-id="c7af4-108">日付</span><span class="sxs-lookup"><span data-stu-id="c7af4-108">Date</span></span>   |
| <span data-ttu-id="c7af4-109">送信</span><span class="sxs-lookup"><span data-stu-id="c7af4-109">send</span></span>              | <span data-ttu-id="c7af4-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c7af4-110">Int64</span></span>  |
| <span data-ttu-id="c7af4-111">表示されます。</span><span class="sxs-lookup"><span data-stu-id="c7af4-111">receive</span></span>           | <span data-ttu-id="c7af4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c7af4-112">Int64</span></span>  |
| <span data-ttu-id="c7af4-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="c7af4-113">read</span></span>              | <span data-ttu-id="c7af4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c7af4-114">Int64</span></span>  |
| <span data-ttu-id="c7af4-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="c7af4-115">reportDate</span></span>        | <span data-ttu-id="c7af4-116">日付</span><span class="sxs-lookup"><span data-stu-id="c7af4-116">Date</span></span>   |
| <span data-ttu-id="c7af4-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c7af4-117">reportPeriod</span></span>      | <span data-ttu-id="c7af4-118">String</span><span class="sxs-lookup"><span data-stu-id="c7af4-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7af4-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7af4-119">JSON representation</span></span>

<span data-ttu-id="c7af4-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c7af4-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
