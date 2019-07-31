---
title: skypeForBusinessOrganizerActivityMinuteCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c06f2f266cf86d0eae9166b5520a4519d045f948
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964894"
---
# <a name="skypeforbusinessorganizeractivityminutecounts-resource-type"></a><span data-ttu-id="aa537-103">skypeForBusinessOrganizerActivityMinuteCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa537-103">skypeForBusinessOrganizerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="aa537-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa537-104">Properties</span></span>

| <span data-ttu-id="aa537-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa537-105">Property</span></span>           | <span data-ttu-id="aa537-106">型</span><span class="sxs-lookup"><span data-stu-id="aa537-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="aa537-107">audioVideo</span><span class="sxs-lookup"><span data-stu-id="aa537-107">audioVideo</span></span>         | <span data-ttu-id="aa537-108">Int64</span><span class="sxs-lookup"><span data-stu-id="aa537-108">Int64</span></span>  |
| <span data-ttu-id="aa537-109">dialInMicrosoft</span><span class="sxs-lookup"><span data-stu-id="aa537-109">dialInMicrosoft</span></span>    | <span data-ttu-id="aa537-110">Int64</span><span class="sxs-lookup"><span data-stu-id="aa537-110">Int64</span></span>  |
| <span data-ttu-id="aa537-111">ダイヤルアウト Microsoft</span><span class="sxs-lookup"><span data-stu-id="aa537-111">dialOutMicrosoft</span></span>   | <span data-ttu-id="aa537-112">Int64</span><span class="sxs-lookup"><span data-stu-id="aa537-112">Int64</span></span>  |
| <span data-ttu-id="aa537-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="aa537-113">reportRefreshDate</span></span>  | <span data-ttu-id="aa537-114">日付</span><span class="sxs-lookup"><span data-stu-id="aa537-114">Date</span></span>   |
| <span data-ttu-id="aa537-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="aa537-115">reportDate</span></span>         | <span data-ttu-id="aa537-116">日付</span><span class="sxs-lookup"><span data-stu-id="aa537-116">Date</span></span>   |
| <span data-ttu-id="aa537-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="aa537-117">reportPeriod</span></span>       | <span data-ttu-id="aa537-118">String</span><span class="sxs-lookup"><span data-stu-id="aa537-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa537-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa537-119">JSON representation</span></span>

<span data-ttu-id="aa537-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aa537-120">The following is a JSON representation of the resource.</span></span>

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
