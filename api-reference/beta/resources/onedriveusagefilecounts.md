---
title: oneDriveUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 98e387b97687a4aab55e8d94e72fdbfa585a0e84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067384"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="369f5-103">oneDriveUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="369f5-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="369f5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="369f5-104">Properties</span></span>

| <span data-ttu-id="369f5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="369f5-105">Property</span></span>          | <span data-ttu-id="369f5-106">型</span><span class="sxs-lookup"><span data-stu-id="369f5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="369f5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="369f5-107">reportRefreshDate</span></span> | <span data-ttu-id="369f5-108">Date</span><span class="sxs-lookup"><span data-stu-id="369f5-108">Date</span></span>   |
| <span data-ttu-id="369f5-109">ある</span><span class="sxs-lookup"><span data-stu-id="369f5-109">siteType</span></span>          | <span data-ttu-id="369f5-110">String</span><span class="sxs-lookup"><span data-stu-id="369f5-110">String</span></span> |
| <span data-ttu-id="369f5-111">total</span><span class="sxs-lookup"><span data-stu-id="369f5-111">total</span></span>             | <span data-ttu-id="369f5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="369f5-112">Int64</span></span>  |
| <span data-ttu-id="369f5-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="369f5-113">active</span></span>            | <span data-ttu-id="369f5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="369f5-114">Int64</span></span>  |
| <span data-ttu-id="369f5-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="369f5-115">reportDate</span></span>        | <span data-ttu-id="369f5-116">Date</span><span class="sxs-lookup"><span data-stu-id="369f5-116">Date</span></span>   |
| <span data-ttu-id="369f5-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="369f5-117">reportPeriod</span></span>      | <span data-ttu-id="369f5-118">String</span><span class="sxs-lookup"><span data-stu-id="369f5-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="369f5-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="369f5-119">JSON representation</span></span>

<span data-ttu-id="369f5-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="369f5-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
