---
title: skypeForBusinessOrganizerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 6b3b38c61ebb7b294de9ea5fc2641a7527bf04f7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461186"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a><span data-ttu-id="534b6-103">skypeForBusinessOrganizerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="534b6-103">skypeForBusinessOrganizerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="534b6-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="534b6-104">Properties</span></span>

| <span data-ttu-id="534b6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="534b6-105">Property</span></span>           | <span data-ttu-id="534b6-106">型</span><span class="sxs-lookup"><span data-stu-id="534b6-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="534b6-107">audioVideo</span><span class="sxs-lookup"><span data-stu-id="534b6-107">audioVideo</span></span>         | <span data-ttu-id="534b6-108">Int64</span><span class="sxs-lookup"><span data-stu-id="534b6-108">Int64</span></span>  |
| <span data-ttu-id="534b6-109">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="534b6-109">dialInOut3rdParty</span></span>  | <span data-ttu-id="534b6-110">Int64</span><span class="sxs-lookup"><span data-stu-id="534b6-110">Int64</span></span>  |
| <span data-ttu-id="534b6-111">ダイヤルアウト microsoft</span><span class="sxs-lookup"><span data-stu-id="534b6-111">dialInOutMicrosoft</span></span> | <span data-ttu-id="534b6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="534b6-112">Int64</span></span>  |
| <span data-ttu-id="534b6-113">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="534b6-113">reportRefreshDate</span></span>  | <span data-ttu-id="534b6-114">Date</span><span class="sxs-lookup"><span data-stu-id="534b6-114">Date</span></span>   |
| <span data-ttu-id="534b6-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="534b6-115">reportDate</span></span>         | <span data-ttu-id="534b6-116">Date</span><span class="sxs-lookup"><span data-stu-id="534b6-116">Date</span></span>   |
| <span data-ttu-id="534b6-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="534b6-117">reportPeriod</span></span>       | <span data-ttu-id="534b6-118">String</span><span class="sxs-lookup"><span data-stu-id="534b6-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="534b6-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="534b6-119">JSON representation</span></span>

<span data-ttu-id="534b6-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="534b6-120">The following is a JSON representation of the resource.</span></span>

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
