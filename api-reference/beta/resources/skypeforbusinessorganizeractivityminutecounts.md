---
title: skypeForBusinessOrganizerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 6b3b38c61ebb7b294de9ea5fc2641a7527bf04f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823206"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a><span data-ttu-id="3465b-103">skypeForBusinessOrganizerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3465b-103">skypeForBusinessOrganizerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="3465b-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3465b-104">Properties</span></span>

| <span data-ttu-id="3465b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3465b-105">Property</span></span>           | <span data-ttu-id="3465b-106">種類</span><span class="sxs-lookup"><span data-stu-id="3465b-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="3465b-107">audioVideo</span><span class="sxs-lookup"><span data-stu-id="3465b-107">audioVideo</span></span>         | <span data-ttu-id="3465b-108">Int64</span><span class="sxs-lookup"><span data-stu-id="3465b-108">Int64</span></span>  |
| <span data-ttu-id="3465b-109">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="3465b-109">dialInOut3rdParty</span></span>  | <span data-ttu-id="3465b-110">Int64</span><span class="sxs-lookup"><span data-stu-id="3465b-110">Int64</span></span>  |
| <span data-ttu-id="3465b-111">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="3465b-111">dialInOutMicrosoft</span></span> | <span data-ttu-id="3465b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="3465b-112">Int64</span></span>  |
| <span data-ttu-id="3465b-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3465b-113">reportRefreshDate</span></span>  | <span data-ttu-id="3465b-114">日付</span><span class="sxs-lookup"><span data-stu-id="3465b-114">Date</span></span>   |
| <span data-ttu-id="3465b-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="3465b-115">reportDate</span></span>         | <span data-ttu-id="3465b-116">日付</span><span class="sxs-lookup"><span data-stu-id="3465b-116">Date</span></span>   |
| <span data-ttu-id="3465b-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3465b-117">reportPeriod</span></span>       | <span data-ttu-id="3465b-118">String</span><span class="sxs-lookup"><span data-stu-id="3465b-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3465b-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3465b-119">JSON representation</span></span>

<span data-ttu-id="3465b-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3465b-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts"
} -->

```json
{
  "audioVideo": 1024, 
  "dialInMicrosoft": 1024, 
  "dialOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
