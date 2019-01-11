---
title: oneDriveUsageAccountCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 021d0089969a6272996f604630b900af61a7a5a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868195"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="257eb-103">oneDriveUsageAccountCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="257eb-103">oneDriveUsageAccountCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="257eb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="257eb-104">Properties</span></span>

| <span data-ttu-id="257eb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="257eb-105">Property</span></span>          | <span data-ttu-id="257eb-106">種類</span><span class="sxs-lookup"><span data-stu-id="257eb-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="257eb-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="257eb-107">reportRefreshDate</span></span> | <span data-ttu-id="257eb-108">日付</span><span class="sxs-lookup"><span data-stu-id="257eb-108">Date</span></span>   |
| <span data-ttu-id="257eb-109">ある</span><span class="sxs-lookup"><span data-stu-id="257eb-109">siteType</span></span>          | <span data-ttu-id="257eb-110">String</span><span class="sxs-lookup"><span data-stu-id="257eb-110">String</span></span> |
| <span data-ttu-id="257eb-111">total</span><span class="sxs-lookup"><span data-stu-id="257eb-111">total</span></span>             | <span data-ttu-id="257eb-112">Int64</span><span class="sxs-lookup"><span data-stu-id="257eb-112">Int64</span></span>  |
| <span data-ttu-id="257eb-113">アクティブです</span><span class="sxs-lookup"><span data-stu-id="257eb-113">active</span></span>            | <span data-ttu-id="257eb-114">Int64</span><span class="sxs-lookup"><span data-stu-id="257eb-114">Int64</span></span>  |
| <span data-ttu-id="257eb-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="257eb-115">reportDate</span></span>        | <span data-ttu-id="257eb-116">日付</span><span class="sxs-lookup"><span data-stu-id="257eb-116">Date</span></span>   |
| <span data-ttu-id="257eb-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="257eb-117">reportPeriod</span></span>      | <span data-ttu-id="257eb-118">String</span><span class="sxs-lookup"><span data-stu-id="257eb-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="257eb-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="257eb-119">JSON representation</span></span>

<span data-ttu-id="257eb-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="257eb-120">The following is a JSON representation of the resource.</span></span>

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
