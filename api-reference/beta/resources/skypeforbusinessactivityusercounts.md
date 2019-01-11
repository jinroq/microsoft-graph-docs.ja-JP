---
title: skypeForBusinessActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: e98133611d669a2a85bae65195fe70571d290442
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815485"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a><span data-ttu-id="43196-103">skypeForBusinessActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43196-103">skypeForBusinessActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="43196-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43196-104">Properties</span></span>

| <span data-ttu-id="43196-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43196-105">Property</span></span>          | <span data-ttu-id="43196-106">種類</span><span class="sxs-lookup"><span data-stu-id="43196-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="43196-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="43196-107">peerToPeer</span></span>        | <span data-ttu-id="43196-108">Int64</span><span class="sxs-lookup"><span data-stu-id="43196-108">Int64</span></span>  |
| <span data-ttu-id="43196-109">編成</span><span class="sxs-lookup"><span data-stu-id="43196-109">organized</span></span>         | <span data-ttu-id="43196-110">Int64</span><span class="sxs-lookup"><span data-stu-id="43196-110">Int64</span></span>  |
| <span data-ttu-id="43196-111">参加</span><span class="sxs-lookup"><span data-stu-id="43196-111">participated</span></span>      | <span data-ttu-id="43196-112">Int64</span><span class="sxs-lookup"><span data-stu-id="43196-112">Int64</span></span>  |
| <span data-ttu-id="43196-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="43196-113">reportRefreshDate</span></span> | <span data-ttu-id="43196-114">日付</span><span class="sxs-lookup"><span data-stu-id="43196-114">Date</span></span>   |
| <span data-ttu-id="43196-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="43196-115">reportDate</span></span>        | <span data-ttu-id="43196-116">日付</span><span class="sxs-lookup"><span data-stu-id="43196-116">Date</span></span>   |
| <span data-ttu-id="43196-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="43196-117">reportPeriod</span></span>      | <span data-ttu-id="43196-118">String</span><span class="sxs-lookup"><span data-stu-id="43196-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="43196-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43196-119">JSON representation</span></span>

<span data-ttu-id="43196-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="43196-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
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
