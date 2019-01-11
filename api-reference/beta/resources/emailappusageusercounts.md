---
title: emailAppUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: a018776f092e9b7f378e8069666d015e1cd3e4a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835449"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="61e8d-103">emailAppUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61e8d-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="61e8d-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61e8d-104">Properties</span></span>

| <span data-ttu-id="61e8d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61e8d-105">Property</span></span>          | <span data-ttu-id="61e8d-106">種類</span><span class="sxs-lookup"><span data-stu-id="61e8d-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="61e8d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="61e8d-107">reportRefreshDate</span></span> | <span data-ttu-id="61e8d-108">日付</span><span class="sxs-lookup"><span data-stu-id="61e8d-108">Date</span></span>   |
| <span data-ttu-id="61e8d-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="61e8d-109">mailForMac</span></span>        | <span data-ttu-id="61e8d-110">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-110">Int64</span></span>  |
| <span data-ttu-id="61e8d-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="61e8d-111">outlookForMac</span></span>     | <span data-ttu-id="61e8d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-112">Int64</span></span>  |
| <span data-ttu-id="61e8d-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="61e8d-113">outlookForWindows</span></span> | <span data-ttu-id="61e8d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-114">Int64</span></span>  |
| <span data-ttu-id="61e8d-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="61e8d-115">outlookForMobile</span></span>  | <span data-ttu-id="61e8d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-116">Int64</span></span>  |
| <span data-ttu-id="61e8d-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="61e8d-117">otherForMobile</span></span>    | <span data-ttu-id="61e8d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-118">Int64</span></span>  |
| <span data-ttu-id="61e8d-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="61e8d-119">outlookForWeb</span></span>     | <span data-ttu-id="61e8d-120">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-120">Int64</span></span>  |
| <span data-ttu-id="61e8d-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="61e8d-121">pop3App</span></span>           | <span data-ttu-id="61e8d-122">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-122">Int64</span></span>  |
| <span data-ttu-id="61e8d-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="61e8d-123">imap4App</span></span>          | <span data-ttu-id="61e8d-124">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-124">Int64</span></span>  |
| <span data-ttu-id="61e8d-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="61e8d-125">smtpApp</span></span>           | <span data-ttu-id="61e8d-126">Int64</span><span class="sxs-lookup"><span data-stu-id="61e8d-126">Int64</span></span>  |
| <span data-ttu-id="61e8d-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="61e8d-127">reportDate</span></span>        | <span data-ttu-id="61e8d-128">日付</span><span class="sxs-lookup"><span data-stu-id="61e8d-128">Date</span></span>   |
| <span data-ttu-id="61e8d-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="61e8d-129">reportPeriod</span></span>      | <span data-ttu-id="61e8d-130">String</span><span class="sxs-lookup"><span data-stu-id="61e8d-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61e8d-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61e8d-131">JSON representation</span></span>

<span data-ttu-id="61e8d-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61e8d-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
