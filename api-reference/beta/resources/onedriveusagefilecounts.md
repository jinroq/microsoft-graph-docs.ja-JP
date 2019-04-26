---
title: oneDriveUsageFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7e3a52d082d1acdd2e685008d60e6594615f57a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568104"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="856d5-103">oneDriveUsageFileCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="856d5-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="856d5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="856d5-104">Properties</span></span>

| <span data-ttu-id="856d5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="856d5-105">Property</span></span>          | <span data-ttu-id="856d5-106">型</span><span class="sxs-lookup"><span data-stu-id="856d5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="856d5-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="856d5-107">reportRefreshDate</span></span> | <span data-ttu-id="856d5-108">Date</span><span class="sxs-lookup"><span data-stu-id="856d5-108">Date</span></span>   |
| <span data-ttu-id="856d5-109">sitetype</span><span class="sxs-lookup"><span data-stu-id="856d5-109">siteType</span></span>          | <span data-ttu-id="856d5-110">String</span><span class="sxs-lookup"><span data-stu-id="856d5-110">String</span></span> |
| <span data-ttu-id="856d5-111">total</span><span class="sxs-lookup"><span data-stu-id="856d5-111">total</span></span>             | <span data-ttu-id="856d5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="856d5-112">Int64</span></span>  |
| <span data-ttu-id="856d5-113">active</span><span class="sxs-lookup"><span data-stu-id="856d5-113">active</span></span>            | <span data-ttu-id="856d5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="856d5-114">Int64</span></span>  |
| <span data-ttu-id="856d5-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="856d5-115">reportDate</span></span>        | <span data-ttu-id="856d5-116">Date</span><span class="sxs-lookup"><span data-stu-id="856d5-116">Date</span></span>   |
| <span data-ttu-id="856d5-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="856d5-117">reportPeriod</span></span>      | <span data-ttu-id="856d5-118">String</span><span class="sxs-lookup"><span data-stu-id="856d5-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="856d5-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="856d5-119">JSON representation</span></span>

<span data-ttu-id="856d5-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="856d5-120">The following is a JSON representation of the resource.</span></span>

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
