---
title: siteActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 2eb5bdb89924338d1d352ea80bd516b8fb948250
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817767"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="a793c-103">siteActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a793c-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a793c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a793c-104">Properties</span></span>

| <span data-ttu-id="a793c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a793c-105">Property</span></span>          | <span data-ttu-id="a793c-106">種類</span><span class="sxs-lookup"><span data-stu-id="a793c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a793c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a793c-107">reportRefreshDate</span></span> | <span data-ttu-id="a793c-108">日付</span><span class="sxs-lookup"><span data-stu-id="a793c-108">Date</span></span>   |
| <span data-ttu-id="a793c-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="a793c-109">viewedOrEdited</span></span>    | <span data-ttu-id="a793c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a793c-110">Int64</span></span>  |
| <span data-ttu-id="a793c-111">同期</span><span class="sxs-lookup"><span data-stu-id="a793c-111">synced</span></span>            | <span data-ttu-id="a793c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a793c-112">Int64</span></span>  |
| <span data-ttu-id="a793c-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="a793c-113">sharedInternally</span></span>  | <span data-ttu-id="a793c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a793c-114">Int64</span></span>  |
| <span data-ttu-id="a793c-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="a793c-115">sharedExternally</span></span>  | <span data-ttu-id="a793c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a793c-116">Int64</span></span>  |
| <span data-ttu-id="a793c-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="a793c-117">reportDate</span></span>        | <span data-ttu-id="a793c-118">日付</span><span class="sxs-lookup"><span data-stu-id="a793c-118">Date</span></span>   |
| <span data-ttu-id="a793c-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a793c-119">reportPeriod</span></span>      | <span data-ttu-id="a793c-120">String</span><span class="sxs-lookup"><span data-stu-id="a793c-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a793c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a793c-121">JSON representation</span></span>

<span data-ttu-id="a793c-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a793c-122">The following is a JSON representation of the resource.</span></span>

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
