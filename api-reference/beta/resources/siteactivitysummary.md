---
title: siteactivitysummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a49b8e47ca2a6efcc5c5c87702fdea0122b208e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583600"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="fe1ea-103">siteactivitysummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe1ea-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fe1ea-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe1ea-104">Properties</span></span>

| <span data-ttu-id="fe1ea-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe1ea-105">Property</span></span>          | <span data-ttu-id="fe1ea-106">型</span><span class="sxs-lookup"><span data-stu-id="fe1ea-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fe1ea-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="fe1ea-107">reportRefreshDate</span></span> | <span data-ttu-id="fe1ea-108">Date</span><span class="sxs-lookup"><span data-stu-id="fe1ea-108">Date</span></span>   |
| <span data-ttu-id="fe1ea-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="fe1ea-109">viewedOrEdited</span></span>    | <span data-ttu-id="fe1ea-110">Int64</span><span class="sxs-lookup"><span data-stu-id="fe1ea-110">Int64</span></span>  |
| <span data-ttu-id="fe1ea-111">同期</span><span class="sxs-lookup"><span data-stu-id="fe1ea-111">synced</span></span>            | <span data-ttu-id="fe1ea-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fe1ea-112">Int64</span></span>  |
| <span data-ttu-id="fe1ea-113">sharedinternally</span><span class="sxs-lookup"><span data-stu-id="fe1ea-113">sharedInternally</span></span>  | <span data-ttu-id="fe1ea-114">Int64</span><span class="sxs-lookup"><span data-stu-id="fe1ea-114">Int64</span></span>  |
| <span data-ttu-id="fe1ea-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="fe1ea-115">sharedExternally</span></span>  | <span data-ttu-id="fe1ea-116">Int64</span><span class="sxs-lookup"><span data-stu-id="fe1ea-116">Int64</span></span>  |
| <span data-ttu-id="fe1ea-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="fe1ea-117">reportDate</span></span>        | <span data-ttu-id="fe1ea-118">Date</span><span class="sxs-lookup"><span data-stu-id="fe1ea-118">Date</span></span>   |
| <span data-ttu-id="fe1ea-119">reportperiod</span><span class="sxs-lookup"><span data-stu-id="fe1ea-119">reportPeriod</span></span>      | <span data-ttu-id="fe1ea-120">String</span><span class="sxs-lookup"><span data-stu-id="fe1ea-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fe1ea-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe1ea-121">JSON representation</span></span>

<span data-ttu-id="fe1ea-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fe1ea-122">The following is a JSON representation of the resource.</span></span>

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
