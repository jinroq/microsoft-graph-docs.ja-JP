---
title: emailActivitySummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 64c9468d79a93b6f82fff0f04206a0fb6e95e4fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972223"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="2f323-103">emailActivitySummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f323-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2f323-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f323-104">Properties</span></span>

| <span data-ttu-id="2f323-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f323-105">Property</span></span>          | <span data-ttu-id="2f323-106">型</span><span class="sxs-lookup"><span data-stu-id="2f323-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2f323-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2f323-107">reportRefreshDate</span></span> | <span data-ttu-id="2f323-108">日付</span><span class="sxs-lookup"><span data-stu-id="2f323-108">Date</span></span>   |
| <span data-ttu-id="2f323-109">送信</span><span class="sxs-lookup"><span data-stu-id="2f323-109">send</span></span>              | <span data-ttu-id="2f323-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2f323-110">Int64</span></span>  |
| <span data-ttu-id="2f323-111">送信</span><span class="sxs-lookup"><span data-stu-id="2f323-111">receive</span></span>           | <span data-ttu-id="2f323-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2f323-112">Int64</span></span>  |
| <span data-ttu-id="2f323-113">読み込む</span><span class="sxs-lookup"><span data-stu-id="2f323-113">read</span></span>              | <span data-ttu-id="2f323-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2f323-114">Int64</span></span>  |
| <span data-ttu-id="2f323-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="2f323-115">reportDate</span></span>        | <span data-ttu-id="2f323-116">日付</span><span class="sxs-lookup"><span data-stu-id="2f323-116">Date</span></span>   |
| <span data-ttu-id="2f323-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2f323-117">reportPeriod</span></span>      | <span data-ttu-id="2f323-118">String</span><span class="sxs-lookup"><span data-stu-id="2f323-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f323-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f323-119">JSON representation</span></span>

<span data-ttu-id="2f323-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f323-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
