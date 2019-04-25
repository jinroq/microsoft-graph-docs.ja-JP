---
title: sharePointActivityPages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: febca3bb97bc81d39838f168779d271a6e986bef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584041"
---
# <a name="sharepointactivitypages-resource-type"></a><span data-ttu-id="9a391-103">sharePointActivityPages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a391-103">sharePointActivityPages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9a391-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a391-104">Properties</span></span>

| <span data-ttu-id="9a391-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a391-105">Property</span></span>          | <span data-ttu-id="9a391-106">型</span><span class="sxs-lookup"><span data-stu-id="9a391-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="9a391-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="9a391-107">reportRefreshDate</span></span> | <span data-ttu-id="9a391-108">Date</span><span class="sxs-lookup"><span data-stu-id="9a391-108">Date</span></span>   |
| <span data-ttu-id="9a391-109">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="9a391-109">visitedPageCount</span></span>  | <span data-ttu-id="9a391-110">Int64</span><span class="sxs-lookup"><span data-stu-id="9a391-110">Int64</span></span>  |
| <span data-ttu-id="9a391-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="9a391-111">reportDate</span></span>        | <span data-ttu-id="9a391-112">Date</span><span class="sxs-lookup"><span data-stu-id="9a391-112">Date</span></span>   |
| <span data-ttu-id="9a391-113">reportperiod</span><span class="sxs-lookup"><span data-stu-id="9a391-113">reportPeriod</span></span>      | <span data-ttu-id="9a391-114">String</span><span class="sxs-lookup"><span data-stu-id="9a391-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a391-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a391-115">JSON representation</span></span>

<span data-ttu-id="9a391-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a391-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityPages"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPageCount": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
