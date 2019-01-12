---
title: emailActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 84958874af09b31aafed694c1a62d080a5c798ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990090"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="59686-103">emailActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59686-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="59686-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59686-104">Properties</span></span>

| <span data-ttu-id="59686-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59686-105">Property</span></span>          | <span data-ttu-id="59686-106">種類</span><span class="sxs-lookup"><span data-stu-id="59686-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="59686-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="59686-107">reportRefreshDate</span></span> | <span data-ttu-id="59686-108">日付</span><span class="sxs-lookup"><span data-stu-id="59686-108">Date</span></span>   |
| <span data-ttu-id="59686-109">送信</span><span class="sxs-lookup"><span data-stu-id="59686-109">send</span></span>              | <span data-ttu-id="59686-110">Int64</span><span class="sxs-lookup"><span data-stu-id="59686-110">Int64</span></span>  |
| <span data-ttu-id="59686-111">表示されます。</span><span class="sxs-lookup"><span data-stu-id="59686-111">receive</span></span>           | <span data-ttu-id="59686-112">Int64</span><span class="sxs-lookup"><span data-stu-id="59686-112">Int64</span></span>  |
| <span data-ttu-id="59686-113">読み取り</span><span class="sxs-lookup"><span data-stu-id="59686-113">read</span></span>              | <span data-ttu-id="59686-114">Int64</span><span class="sxs-lookup"><span data-stu-id="59686-114">Int64</span></span>  |
| <span data-ttu-id="59686-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="59686-115">reportDate</span></span>        | <span data-ttu-id="59686-116">日付</span><span class="sxs-lookup"><span data-stu-id="59686-116">Date</span></span>   |
| <span data-ttu-id="59686-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="59686-117">reportPeriod</span></span>      | <span data-ttu-id="59686-118">String</span><span class="sxs-lookup"><span data-stu-id="59686-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="59686-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59686-119">JSON representation</span></span>

<span data-ttu-id="59686-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59686-120">The following is a JSON representation of the resource.</span></span>

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
