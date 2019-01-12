---
title: oneDriveUsageAccountCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: dd70875c272f63a1c9a7988c001225c2d200e0c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947184"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="5fb80-103">oneDriveUsageAccountCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5fb80-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5fb80-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fb80-104">Properties</span></span>

| <span data-ttu-id="5fb80-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5fb80-105">Property</span></span>          | <span data-ttu-id="5fb80-106">種類</span><span class="sxs-lookup"><span data-stu-id="5fb80-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5fb80-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5fb80-107">reportRefreshDate</span></span> | <span data-ttu-id="5fb80-108">日付</span><span class="sxs-lookup"><span data-stu-id="5fb80-108">Date</span></span>   |
| <span data-ttu-id="5fb80-109">ある</span><span class="sxs-lookup"><span data-stu-id="5fb80-109">siteType</span></span>          | <span data-ttu-id="5fb80-110">String</span><span class="sxs-lookup"><span data-stu-id="5fb80-110">String</span></span> |
| <span data-ttu-id="5fb80-111">total</span><span class="sxs-lookup"><span data-stu-id="5fb80-111">total</span></span>             | <span data-ttu-id="5fb80-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5fb80-112">Int64</span></span>  |
| <span data-ttu-id="5fb80-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="5fb80-113">active</span></span>            | <span data-ttu-id="5fb80-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5fb80-114">Int64</span></span>  |
| <span data-ttu-id="5fb80-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="5fb80-115">reportDate</span></span>        | <span data-ttu-id="5fb80-116">日付</span><span class="sxs-lookup"><span data-stu-id="5fb80-116">Date</span></span>   |
| <span data-ttu-id="5fb80-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5fb80-117">reportPeriod</span></span>      | <span data-ttu-id="5fb80-118">String</span><span class="sxs-lookup"><span data-stu-id="5fb80-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5fb80-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5fb80-119">JSON representation</span></span>

<span data-ttu-id="5fb80-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5fb80-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
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
