---
title: skypeForBusinessOrganizerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: e2eba759ab8c22d8105267779bac46f909262bb8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342822"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a><span data-ttu-id="a2c49-103">skypeForBusinessOrganizerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2c49-103">skypeForBusinessOrganizerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a2c49-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2c49-104">Properties</span></span>

| <span data-ttu-id="a2c49-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2c49-105">Property</span></span>           | <span data-ttu-id="a2c49-106">型</span><span class="sxs-lookup"><span data-stu-id="a2c49-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="a2c49-107">audioVideo</span><span class="sxs-lookup"><span data-stu-id="a2c49-107">audioVideo</span></span>         | <span data-ttu-id="a2c49-108">Int64</span><span class="sxs-lookup"><span data-stu-id="a2c49-108">Int64</span></span>  |
| <span data-ttu-id="a2c49-109">dialInMicrosoft</span><span class="sxs-lookup"><span data-stu-id="a2c49-109">dialInMicrosoft</span></span>    | <span data-ttu-id="a2c49-110">Int64</span><span class="sxs-lookup"><span data-stu-id="a2c49-110">Int64</span></span>  |
| <span data-ttu-id="a2c49-111">ダイヤルアウト microsoft</span><span class="sxs-lookup"><span data-stu-id="a2c49-111">dialOutMicrosoft</span></span>   | <span data-ttu-id="a2c49-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a2c49-112">Int64</span></span>  |
| <span data-ttu-id="a2c49-113">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="a2c49-113">reportRefreshDate</span></span>  | <span data-ttu-id="a2c49-114">日付</span><span class="sxs-lookup"><span data-stu-id="a2c49-114">Date</span></span>   |
| <span data-ttu-id="a2c49-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="a2c49-115">reportDate</span></span>         | <span data-ttu-id="a2c49-116">日付</span><span class="sxs-lookup"><span data-stu-id="a2c49-116">Date</span></span>   |
| <span data-ttu-id="a2c49-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="a2c49-117">reportPeriod</span></span>       | <span data-ttu-id="a2c49-118">String</span><span class="sxs-lookup"><span data-stu-id="a2c49-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a2c49-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2c49-119">JSON representation</span></span>

<span data-ttu-id="a2c49-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a2c49-120">The following is a JSON representation of the resource.</span></span>

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
