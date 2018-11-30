---
title: yammerActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 6ff2b347de77f91c96cb5f5be797eb70db0bbbee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067433"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="dd427-103">yammerActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dd427-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="dd427-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd427-104">Properties</span></span>

| <span data-ttu-id="dd427-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd427-105">Property</span></span>          | <span data-ttu-id="dd427-106">型</span><span class="sxs-lookup"><span data-stu-id="dd427-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="dd427-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="dd427-107">reportRefreshDate</span></span> | <span data-ttu-id="dd427-108">Date</span><span class="sxs-lookup"><span data-stu-id="dd427-108">Date</span></span>   |
| <span data-ttu-id="dd427-109">気に入られました</span><span class="sxs-lookup"><span data-stu-id="dd427-109">liked</span></span>             | <span data-ttu-id="dd427-110">Int64</span><span class="sxs-lookup"><span data-stu-id="dd427-110">Int64</span></span>  |
| <span data-ttu-id="dd427-111">転記</span><span class="sxs-lookup"><span data-stu-id="dd427-111">posted</span></span>            | <span data-ttu-id="dd427-112">Int64</span><span class="sxs-lookup"><span data-stu-id="dd427-112">Int64</span></span>  |
| <span data-ttu-id="dd427-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="dd427-113">read</span></span>              | <span data-ttu-id="dd427-114">Int64</span><span class="sxs-lookup"><span data-stu-id="dd427-114">Int64</span></span>  |
| <span data-ttu-id="dd427-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="dd427-115">reportDate</span></span>        | <span data-ttu-id="dd427-116">Date</span><span class="sxs-lookup"><span data-stu-id="dd427-116">Date</span></span>   |
| <span data-ttu-id="dd427-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="dd427-117">reportPeriod</span></span>      | <span data-ttu-id="dd427-118">String</span><span class="sxs-lookup"><span data-stu-id="dd427-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dd427-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd427-119">JSON representation</span></span>

<span data-ttu-id="dd427-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dd427-120">The following is a JSON representation of the resource.</span></span>

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
