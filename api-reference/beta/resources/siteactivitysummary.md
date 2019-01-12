---
title: siteActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a49b8e47ca2a6efcc5c5c87702fdea0122b208e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957138"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="5352f-103">siteActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5352f-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5352f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5352f-104">Properties</span></span>

| <span data-ttu-id="5352f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5352f-105">Property</span></span>          | <span data-ttu-id="5352f-106">種類</span><span class="sxs-lookup"><span data-stu-id="5352f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5352f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5352f-107">reportRefreshDate</span></span> | <span data-ttu-id="5352f-108">日付</span><span class="sxs-lookup"><span data-stu-id="5352f-108">Date</span></span>   |
| <span data-ttu-id="5352f-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="5352f-109">viewedOrEdited</span></span>    | <span data-ttu-id="5352f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5352f-110">Int64</span></span>  |
| <span data-ttu-id="5352f-111">同期</span><span class="sxs-lookup"><span data-stu-id="5352f-111">synced</span></span>            | <span data-ttu-id="5352f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5352f-112">Int64</span></span>  |
| <span data-ttu-id="5352f-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="5352f-113">sharedInternally</span></span>  | <span data-ttu-id="5352f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5352f-114">Int64</span></span>  |
| <span data-ttu-id="5352f-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="5352f-115">sharedExternally</span></span>  | <span data-ttu-id="5352f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5352f-116">Int64</span></span>  |
| <span data-ttu-id="5352f-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="5352f-117">reportDate</span></span>        | <span data-ttu-id="5352f-118">日付</span><span class="sxs-lookup"><span data-stu-id="5352f-118">Date</span></span>   |
| <span data-ttu-id="5352f-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5352f-119">reportPeriod</span></span>      | <span data-ttu-id="5352f-120">String</span><span class="sxs-lookup"><span data-stu-id="5352f-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5352f-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5352f-121">JSON representation</span></span>

<span data-ttu-id="5352f-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5352f-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
