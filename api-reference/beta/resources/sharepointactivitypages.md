---
title: sharePointActivityPages リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: febca3bb97bc81d39838f168779d271a6e986bef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930965"
---
# <a name="sharepointactivitypages-resource-type"></a><span data-ttu-id="312b2-103">sharePointActivityPages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="312b2-103">sharePointActivityPages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="312b2-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="312b2-104">Properties</span></span>

| <span data-ttu-id="312b2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="312b2-105">Property</span></span>          | <span data-ttu-id="312b2-106">種類</span><span class="sxs-lookup"><span data-stu-id="312b2-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="312b2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="312b2-107">reportRefreshDate</span></span> | <span data-ttu-id="312b2-108">日付</span><span class="sxs-lookup"><span data-stu-id="312b2-108">Date</span></span>   |
| <span data-ttu-id="312b2-109">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="312b2-109">visitedPageCount</span></span>  | <span data-ttu-id="312b2-110">Int64</span><span class="sxs-lookup"><span data-stu-id="312b2-110">Int64</span></span>  |
| <span data-ttu-id="312b2-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="312b2-111">reportDate</span></span>        | <span data-ttu-id="312b2-112">日付</span><span class="sxs-lookup"><span data-stu-id="312b2-112">Date</span></span>   |
| <span data-ttu-id="312b2-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="312b2-113">reportPeriod</span></span>      | <span data-ttu-id="312b2-114">String</span><span class="sxs-lookup"><span data-stu-id="312b2-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="312b2-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="312b2-115">JSON representation</span></span>

<span data-ttu-id="312b2-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="312b2-116">The following is a JSON representation of the resource.</span></span>

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
