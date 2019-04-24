---
title: skypeforbusinessactivityusercounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: e98133611d669a2a85bae65195fe70571d290442
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521979"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a><span data-ttu-id="d12c3-103">skypeforbusinessactivityusercounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d12c3-103">skypeForBusinessActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d12c3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d12c3-104">Properties</span></span>

| <span data-ttu-id="d12c3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d12c3-105">Property</span></span>          | <span data-ttu-id="d12c3-106">型</span><span class="sxs-lookup"><span data-stu-id="d12c3-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d12c3-107">peertopeer</span><span class="sxs-lookup"><span data-stu-id="d12c3-107">peerToPeer</span></span>        | <span data-ttu-id="d12c3-108">Int64</span><span class="sxs-lookup"><span data-stu-id="d12c3-108">Int64</span></span>  |
| <span data-ttu-id="d12c3-109">別</span><span class="sxs-lookup"><span data-stu-id="d12c3-109">organized</span></span>         | <span data-ttu-id="d12c3-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d12c3-110">Int64</span></span>  |
| <span data-ttu-id="d12c3-111">参加した</span><span class="sxs-lookup"><span data-stu-id="d12c3-111">participated</span></span>      | <span data-ttu-id="d12c3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d12c3-112">Int64</span></span>  |
| <span data-ttu-id="d12c3-113">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="d12c3-113">reportRefreshDate</span></span> | <span data-ttu-id="d12c3-114">Date</span><span class="sxs-lookup"><span data-stu-id="d12c3-114">Date</span></span>   |
| <span data-ttu-id="d12c3-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="d12c3-115">reportDate</span></span>        | <span data-ttu-id="d12c3-116">Date</span><span class="sxs-lookup"><span data-stu-id="d12c3-116">Date</span></span>   |
| <span data-ttu-id="d12c3-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="d12c3-117">reportPeriod</span></span>      | <span data-ttu-id="d12c3-118">String</span><span class="sxs-lookup"><span data-stu-id="d12c3-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d12c3-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d12c3-119">JSON representation</span></span>

<span data-ttu-id="d12c3-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d12c3-120">The following is a JSON representation of the resource.</span></span>

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
