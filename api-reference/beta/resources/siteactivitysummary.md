---
title: siteActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1258530aea56f7ec26a2f48274935afc809f2fd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965020"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="41d44-103">siteActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41d44-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="41d44-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41d44-104">Properties</span></span>

| <span data-ttu-id="41d44-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41d44-105">Property</span></span>          | <span data-ttu-id="41d44-106">型</span><span class="sxs-lookup"><span data-stu-id="41d44-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="41d44-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="41d44-107">reportRefreshDate</span></span> | <span data-ttu-id="41d44-108">日付</span><span class="sxs-lookup"><span data-stu-id="41d44-108">Date</span></span>   |
| <span data-ttu-id="41d44-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="41d44-109">viewedOrEdited</span></span>    | <span data-ttu-id="41d44-110">Int64</span><span class="sxs-lookup"><span data-stu-id="41d44-110">Int64</span></span>  |
| <span data-ttu-id="41d44-111">同期</span><span class="sxs-lookup"><span data-stu-id="41d44-111">synced</span></span>            | <span data-ttu-id="41d44-112">Int64</span><span class="sxs-lookup"><span data-stu-id="41d44-112">Int64</span></span>  |
| <span data-ttu-id="41d44-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="41d44-113">sharedInternally</span></span>  | <span data-ttu-id="41d44-114">Int64</span><span class="sxs-lookup"><span data-stu-id="41d44-114">Int64</span></span>  |
| <span data-ttu-id="41d44-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="41d44-115">sharedExternally</span></span>  | <span data-ttu-id="41d44-116">Int64</span><span class="sxs-lookup"><span data-stu-id="41d44-116">Int64</span></span>  |
| <span data-ttu-id="41d44-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="41d44-117">reportDate</span></span>        | <span data-ttu-id="41d44-118">日付</span><span class="sxs-lookup"><span data-stu-id="41d44-118">Date</span></span>   |
| <span data-ttu-id="41d44-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="41d44-119">reportPeriod</span></span>      | <span data-ttu-id="41d44-120">String</span><span class="sxs-lookup"><span data-stu-id="41d44-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41d44-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41d44-121">JSON representation</span></span>

<span data-ttu-id="41d44-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="41d44-122">The following is a JSON representation of the resource.</span></span>

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
