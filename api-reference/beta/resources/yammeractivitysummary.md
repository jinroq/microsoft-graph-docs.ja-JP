---
title: yammerActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 974e234db31a7942b2b1dcbfff469288c32b6749
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974722"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="3373f-103">yammerActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3373f-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3373f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3373f-104">Properties</span></span>

| <span data-ttu-id="3373f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3373f-105">Property</span></span>          | <span data-ttu-id="3373f-106">種類</span><span class="sxs-lookup"><span data-stu-id="3373f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3373f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3373f-107">reportRefreshDate</span></span> | <span data-ttu-id="3373f-108">日付</span><span class="sxs-lookup"><span data-stu-id="3373f-108">Date</span></span>   |
| <span data-ttu-id="3373f-109">気に入られました</span><span class="sxs-lookup"><span data-stu-id="3373f-109">liked</span></span>             | <span data-ttu-id="3373f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="3373f-110">Int64</span></span>  |
| <span data-ttu-id="3373f-111">転記</span><span class="sxs-lookup"><span data-stu-id="3373f-111">posted</span></span>            | <span data-ttu-id="3373f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3373f-112">Int64</span></span>  |
| <span data-ttu-id="3373f-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="3373f-113">read</span></span>              | <span data-ttu-id="3373f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="3373f-114">Int64</span></span>  |
| <span data-ttu-id="3373f-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="3373f-115">reportDate</span></span>        | <span data-ttu-id="3373f-116">日付</span><span class="sxs-lookup"><span data-stu-id="3373f-116">Date</span></span>   |
| <span data-ttu-id="3373f-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3373f-117">reportPeriod</span></span>      | <span data-ttu-id="3373f-118">String</span><span class="sxs-lookup"><span data-stu-id="3373f-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3373f-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3373f-119">JSON representation</span></span>

<span data-ttu-id="3373f-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3373f-120">The following is a JSON representation of the resource.</span></span>

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
