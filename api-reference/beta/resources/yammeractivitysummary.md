---
title: yammerActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c220ce211c9c6b61d41aa5773e3bcc01697f4e31
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555116"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="7fcee-103">yammerActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7fcee-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7fcee-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fcee-104">Properties</span></span>

| <span data-ttu-id="7fcee-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7fcee-105">Property</span></span>          | <span data-ttu-id="7fcee-106">型</span><span class="sxs-lookup"><span data-stu-id="7fcee-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="7fcee-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="7fcee-107">reportRefreshDate</span></span> | <span data-ttu-id="7fcee-108">Date</span><span class="sxs-lookup"><span data-stu-id="7fcee-108">Date</span></span>   |
| <span data-ttu-id="7fcee-109">好き</span><span class="sxs-lookup"><span data-stu-id="7fcee-109">liked</span></span>             | <span data-ttu-id="7fcee-110">Int64</span><span class="sxs-lookup"><span data-stu-id="7fcee-110">Int64</span></span>  |
| <span data-ttu-id="7fcee-111">れ</span><span class="sxs-lookup"><span data-stu-id="7fcee-111">posted</span></span>            | <span data-ttu-id="7fcee-112">Int64</span><span class="sxs-lookup"><span data-stu-id="7fcee-112">Int64</span></span>  |
| <span data-ttu-id="7fcee-113">読み込む</span><span class="sxs-lookup"><span data-stu-id="7fcee-113">read</span></span>              | <span data-ttu-id="7fcee-114">Int64</span><span class="sxs-lookup"><span data-stu-id="7fcee-114">Int64</span></span>  |
| <span data-ttu-id="7fcee-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="7fcee-115">reportDate</span></span>        | <span data-ttu-id="7fcee-116">Date</span><span class="sxs-lookup"><span data-stu-id="7fcee-116">Date</span></span>   |
| <span data-ttu-id="7fcee-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="7fcee-117">reportPeriod</span></span>      | <span data-ttu-id="7fcee-118">String</span><span class="sxs-lookup"><span data-stu-id="7fcee-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7fcee-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7fcee-119">JSON representation</span></span>

<span data-ttu-id="7fcee-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7fcee-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
