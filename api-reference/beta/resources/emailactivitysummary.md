---
title: emailactivitysummary リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 84958874af09b31aafed694c1a62d080a5c798ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506672"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="ecc67-103">emailactivitysummary リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecc67-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ecc67-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecc67-104">Properties</span></span>

| <span data-ttu-id="ecc67-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecc67-105">Property</span></span>          | <span data-ttu-id="ecc67-106">型</span><span class="sxs-lookup"><span data-stu-id="ecc67-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="ecc67-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="ecc67-107">reportRefreshDate</span></span> | <span data-ttu-id="ecc67-108">Date</span><span class="sxs-lookup"><span data-stu-id="ecc67-108">Date</span></span>   |
| <span data-ttu-id="ecc67-109">送信</span><span class="sxs-lookup"><span data-stu-id="ecc67-109">send</span></span>              | <span data-ttu-id="ecc67-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ecc67-110">Int64</span></span>  |
| <span data-ttu-id="ecc67-111">送信</span><span class="sxs-lookup"><span data-stu-id="ecc67-111">receive</span></span>           | <span data-ttu-id="ecc67-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ecc67-112">Int64</span></span>  |
| <span data-ttu-id="ecc67-113">読み込む</span><span class="sxs-lookup"><span data-stu-id="ecc67-113">read</span></span>              | <span data-ttu-id="ecc67-114">Int64</span><span class="sxs-lookup"><span data-stu-id="ecc67-114">Int64</span></span>  |
| <span data-ttu-id="ecc67-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="ecc67-115">reportDate</span></span>        | <span data-ttu-id="ecc67-116">Date</span><span class="sxs-lookup"><span data-stu-id="ecc67-116">Date</span></span>   |
| <span data-ttu-id="ecc67-117">reportperiod</span><span class="sxs-lookup"><span data-stu-id="ecc67-117">reportPeriod</span></span>      | <span data-ttu-id="ecc67-118">String</span><span class="sxs-lookup"><span data-stu-id="ecc67-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ecc67-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecc67-119">JSON representation</span></span>

<span data-ttu-id="ecc67-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ecc67-120">The following is a JSON representation of the resource.</span></span>

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
