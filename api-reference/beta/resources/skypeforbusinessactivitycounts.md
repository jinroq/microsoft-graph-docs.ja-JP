---
title: skypeForBusinessActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 00c55df3a0a6201bd731938675880b9cbbe9cee6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072512"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="b827e-103">skypeForBusinessActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b827e-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b827e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b827e-104">Properties</span></span>

| <span data-ttu-id="b827e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b827e-105">Property</span></span>          | <span data-ttu-id="b827e-106">型</span><span class="sxs-lookup"><span data-stu-id="b827e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b827e-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="b827e-107">peerToPeer</span></span>        | <span data-ttu-id="b827e-108">Int64</span><span class="sxs-lookup"><span data-stu-id="b827e-108">Int64</span></span>  |
| <span data-ttu-id="b827e-109">編成</span><span class="sxs-lookup"><span data-stu-id="b827e-109">organized</span></span>         | <span data-ttu-id="b827e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b827e-110">Int64</span></span>  |
| <span data-ttu-id="b827e-111">参加</span><span class="sxs-lookup"><span data-stu-id="b827e-111">participated</span></span>      | <span data-ttu-id="b827e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b827e-112">Int64</span></span>  |
| <span data-ttu-id="b827e-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b827e-113">reportRefreshDate</span></span> | <span data-ttu-id="b827e-114">Date</span><span class="sxs-lookup"><span data-stu-id="b827e-114">Date</span></span>   |
| <span data-ttu-id="b827e-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="b827e-115">reportDate</span></span>        | <span data-ttu-id="b827e-116">Date</span><span class="sxs-lookup"><span data-stu-id="b827e-116">Date</span></span>   |
| <span data-ttu-id="b827e-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b827e-117">reportPeriod</span></span>      | <span data-ttu-id="b827e-118">String</span><span class="sxs-lookup"><span data-stu-id="b827e-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b827e-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b827e-119">JSON representation</span></span>

<span data-ttu-id="b827e-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b827e-120">The following is a JSON representation of the resource.</span></span>

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
