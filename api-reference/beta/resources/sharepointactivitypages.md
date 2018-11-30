---
title: sharePointActivityPages リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 9111457d5cb9e710f0b07a43ea06c137af0db0f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066512"
---
# <a name="sharepointactivitypages-resource-type"></a><span data-ttu-id="eacd0-103">sharePointActivityPages リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eacd0-103">sharePointActivityPages resource type</span></span>

## <a name="properties"></a><span data-ttu-id="eacd0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eacd0-104">Properties</span></span>

| <span data-ttu-id="eacd0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eacd0-105">Property</span></span>          | <span data-ttu-id="eacd0-106">型</span><span class="sxs-lookup"><span data-stu-id="eacd0-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="eacd0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="eacd0-107">reportRefreshDate</span></span> | <span data-ttu-id="eacd0-108">Date</span><span class="sxs-lookup"><span data-stu-id="eacd0-108">Date</span></span>   |
| <span data-ttu-id="eacd0-109">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="eacd0-109">visitedPageCount</span></span>  | <span data-ttu-id="eacd0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="eacd0-110">Int64</span></span>  |
| <span data-ttu-id="eacd0-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="eacd0-111">reportDate</span></span>        | <span data-ttu-id="eacd0-112">Date</span><span class="sxs-lookup"><span data-stu-id="eacd0-112">Date</span></span>   |
| <span data-ttu-id="eacd0-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="eacd0-113">reportPeriod</span></span>      | <span data-ttu-id="eacd0-114">String</span><span class="sxs-lookup"><span data-stu-id="eacd0-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eacd0-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eacd0-115">JSON representation</span></span>

<span data-ttu-id="eacd0-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eacd0-116">The following is a JSON representation of the resource.</span></span>

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
