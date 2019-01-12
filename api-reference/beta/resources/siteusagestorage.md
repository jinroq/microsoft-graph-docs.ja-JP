---
title: siteUsageStorage リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928102"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="1e238-103">siteUsageStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e238-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1e238-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e238-104">Properties</span></span>

| <span data-ttu-id="1e238-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e238-105">Property</span></span>           | <span data-ttu-id="1e238-106">種類</span><span class="sxs-lookup"><span data-stu-id="1e238-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="1e238-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1e238-107">reportRefreshDate</span></span>  | <span data-ttu-id="1e238-108">日付</span><span class="sxs-lookup"><span data-stu-id="1e238-108">Date</span></span>   |
| <span data-ttu-id="1e238-109">ある</span><span class="sxs-lookup"><span data-stu-id="1e238-109">siteType</span></span>           | <span data-ttu-id="1e238-110">String</span><span class="sxs-lookup"><span data-stu-id="1e238-110">String</span></span> |
| <span data-ttu-id="1e238-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="1e238-111">storageUsedInBytes</span></span> | <span data-ttu-id="1e238-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1e238-112">Int64</span></span>  |
| <span data-ttu-id="1e238-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="1e238-113">reportDate</span></span>         | <span data-ttu-id="1e238-114">日付</span><span class="sxs-lookup"><span data-stu-id="1e238-114">Date</span></span>   |
| <span data-ttu-id="1e238-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1e238-115">reportPeriod</span></span>       | <span data-ttu-id="1e238-116">String</span><span class="sxs-lookup"><span data-stu-id="1e238-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1e238-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e238-117">JSON representation</span></span>

<span data-ttu-id="1e238-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e238-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
