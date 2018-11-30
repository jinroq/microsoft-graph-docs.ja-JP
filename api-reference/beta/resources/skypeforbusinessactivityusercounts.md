---
title: skypeForBusinessActivityUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: eee736958540f2a3fb42cf3c76a37da4ebe78afd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074498"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a><span data-ttu-id="da049-103">skypeForBusinessActivityUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="da049-103">skypeForBusinessActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="da049-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da049-104">Properties</span></span>

| <span data-ttu-id="da049-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da049-105">Property</span></span>          | <span data-ttu-id="da049-106">型</span><span class="sxs-lookup"><span data-stu-id="da049-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="da049-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="da049-107">peerToPeer</span></span>        | <span data-ttu-id="da049-108">Int64</span><span class="sxs-lookup"><span data-stu-id="da049-108">Int64</span></span>  |
| <span data-ttu-id="da049-109">編成</span><span class="sxs-lookup"><span data-stu-id="da049-109">organized</span></span>         | <span data-ttu-id="da049-110">Int64</span><span class="sxs-lookup"><span data-stu-id="da049-110">Int64</span></span>  |
| <span data-ttu-id="da049-111">参加</span><span class="sxs-lookup"><span data-stu-id="da049-111">participated</span></span>      | <span data-ttu-id="da049-112">Int64</span><span class="sxs-lookup"><span data-stu-id="da049-112">Int64</span></span>  |
| <span data-ttu-id="da049-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="da049-113">reportRefreshDate</span></span> | <span data-ttu-id="da049-114">Date</span><span class="sxs-lookup"><span data-stu-id="da049-114">Date</span></span>   |
| <span data-ttu-id="da049-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="da049-115">reportDate</span></span>        | <span data-ttu-id="da049-116">Date</span><span class="sxs-lookup"><span data-stu-id="da049-116">Date</span></span>   |
| <span data-ttu-id="da049-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="da049-117">reportPeriod</span></span>      | <span data-ttu-id="da049-118">String</span><span class="sxs-lookup"><span data-stu-id="da049-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da049-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="da049-119">JSON representation</span></span>

<span data-ttu-id="da049-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="da049-120">The following is a JSON representation of the resource.</span></span>

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
