---
title: yammerActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 14cd88848e85d8260ccdadfbec8925faf4acba85
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006991"
---
# <a name="yammeractivitysummary-resource-type"></a><span data-ttu-id="71429-103">yammerActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71429-103">yammerActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="71429-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71429-104">Properties</span></span>

| <span data-ttu-id="71429-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71429-105">Property</span></span>          | <span data-ttu-id="71429-106">型</span><span class="sxs-lookup"><span data-stu-id="71429-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="71429-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="71429-107">reportRefreshDate</span></span> | <span data-ttu-id="71429-108">日付</span><span class="sxs-lookup"><span data-stu-id="71429-108">Date</span></span>   |
| <span data-ttu-id="71429-109">好き</span><span class="sxs-lookup"><span data-stu-id="71429-109">liked</span></span>             | <span data-ttu-id="71429-110">Int64</span><span class="sxs-lookup"><span data-stu-id="71429-110">Int64</span></span>  |
| <span data-ttu-id="71429-111">れ</span><span class="sxs-lookup"><span data-stu-id="71429-111">posted</span></span>            | <span data-ttu-id="71429-112">Int64</span><span class="sxs-lookup"><span data-stu-id="71429-112">Int64</span></span>  |
| <span data-ttu-id="71429-113">読み込む</span><span class="sxs-lookup"><span data-stu-id="71429-113">read</span></span>              | <span data-ttu-id="71429-114">Int64</span><span class="sxs-lookup"><span data-stu-id="71429-114">Int64</span></span>  |
| <span data-ttu-id="71429-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="71429-115">reportDate</span></span>        | <span data-ttu-id="71429-116">日付</span><span class="sxs-lookup"><span data-stu-id="71429-116">Date</span></span>   |
| <span data-ttu-id="71429-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="71429-117">reportPeriod</span></span>      | <span data-ttu-id="71429-118">String</span><span class="sxs-lookup"><span data-stu-id="71429-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="71429-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71429-119">JSON representation</span></span>

<span data-ttu-id="71429-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="71429-120">The following is a JSON representation of the resource.</span></span>

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
