---
title: skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 695c2fc57ab9d105b2576a9228ccc58d74b0094d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851619"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="30eee-103">skypeForBusinessPeerToPeerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30eee-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="30eee-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30eee-104">Properties</span></span>

| <span data-ttu-id="30eee-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30eee-105">Property</span></span>          | <span data-ttu-id="30eee-106">種類</span><span class="sxs-lookup"><span data-stu-id="30eee-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="30eee-107">audio</span><span class="sxs-lookup"><span data-stu-id="30eee-107">audio</span></span>             | <span data-ttu-id="30eee-108">Int64</span><span class="sxs-lookup"><span data-stu-id="30eee-108">Int64</span></span>  |
| <span data-ttu-id="30eee-109">video</span><span class="sxs-lookup"><span data-stu-id="30eee-109">video</span></span>             | <span data-ttu-id="30eee-110">Int64</span><span class="sxs-lookup"><span data-stu-id="30eee-110">Int64</span></span>  |
| <span data-ttu-id="30eee-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="30eee-111">reportRefreshDate</span></span> | <span data-ttu-id="30eee-112">日付</span><span class="sxs-lookup"><span data-stu-id="30eee-112">Date</span></span>   |
| <span data-ttu-id="30eee-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="30eee-113">reportDate</span></span>        | <span data-ttu-id="30eee-114">日付</span><span class="sxs-lookup"><span data-stu-id="30eee-114">Date</span></span>   |
| <span data-ttu-id="30eee-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="30eee-115">reportPeriod</span></span>      | <span data-ttu-id="30eee-116">String</span><span class="sxs-lookup"><span data-stu-id="30eee-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30eee-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30eee-117">JSON representation</span></span>

<span data-ttu-id="30eee-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="30eee-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024, 
  "video": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
