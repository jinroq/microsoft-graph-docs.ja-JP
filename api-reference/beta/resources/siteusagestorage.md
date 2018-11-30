---
title: siteUsageStorage リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 1fdfa6cb2690d6dbacf5e534792061b6e64025d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067720"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="14614-103">siteUsageStorage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14614-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="14614-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14614-104">Properties</span></span>

| <span data-ttu-id="14614-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14614-105">Property</span></span>           | <span data-ttu-id="14614-106">型</span><span class="sxs-lookup"><span data-stu-id="14614-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="14614-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="14614-107">reportRefreshDate</span></span>  | <span data-ttu-id="14614-108">Date</span><span class="sxs-lookup"><span data-stu-id="14614-108">Date</span></span>   |
| <span data-ttu-id="14614-109">ある</span><span class="sxs-lookup"><span data-stu-id="14614-109">siteType</span></span>           | <span data-ttu-id="14614-110">String</span><span class="sxs-lookup"><span data-stu-id="14614-110">String</span></span> |
| <span data-ttu-id="14614-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="14614-111">storageUsedInBytes</span></span> | <span data-ttu-id="14614-112">Int64</span><span class="sxs-lookup"><span data-stu-id="14614-112">Int64</span></span>  |
| <span data-ttu-id="14614-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="14614-113">reportDate</span></span>         | <span data-ttu-id="14614-114">Date</span><span class="sxs-lookup"><span data-stu-id="14614-114">Date</span></span>   |
| <span data-ttu-id="14614-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="14614-115">reportPeriod</span></span>       | <span data-ttu-id="14614-116">String</span><span class="sxs-lookup"><span data-stu-id="14614-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="14614-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14614-117">JSON representation</span></span>

<span data-ttu-id="14614-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14614-118">The following is a JSON representation of the resource.</span></span>

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
