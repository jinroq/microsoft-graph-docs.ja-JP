---
title: sharePointActivityPages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 758dcfd2e1c48b0bf8d0d85f06a68f26bfbbef99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811845"
---
# <a name="sharepointactivitypages-resource-type"></a><span data-ttu-id="4c6fc-103">sharePointActivityPages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c6fc-103">sharePointActivityPages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4c6fc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c6fc-104">Properties</span></span>

| <span data-ttu-id="4c6fc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c6fc-105">Property</span></span>          | <span data-ttu-id="4c6fc-106">種類</span><span class="sxs-lookup"><span data-stu-id="4c6fc-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4c6fc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4c6fc-107">reportRefreshDate</span></span> | <span data-ttu-id="4c6fc-108">日付</span><span class="sxs-lookup"><span data-stu-id="4c6fc-108">Date</span></span>   |
| <span data-ttu-id="4c6fc-109">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="4c6fc-109">visitedPageCount</span></span>  | <span data-ttu-id="4c6fc-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4c6fc-110">Int64</span></span>  |
| <span data-ttu-id="4c6fc-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="4c6fc-111">reportDate</span></span>        | <span data-ttu-id="4c6fc-112">日付</span><span class="sxs-lookup"><span data-stu-id="4c6fc-112">Date</span></span>   |
| <span data-ttu-id="4c6fc-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4c6fc-113">reportPeriod</span></span>      | <span data-ttu-id="4c6fc-114">String</span><span class="sxs-lookup"><span data-stu-id="4c6fc-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c6fc-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c6fc-115">JSON representation</span></span>

<span data-ttu-id="4c6fc-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4c6fc-116">The following is a JSON representation of the resource.</span></span>

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
