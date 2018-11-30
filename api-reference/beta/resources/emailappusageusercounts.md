---
title: emailAppUsageUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: c8669c8a34987bc1e71152ae717f9be3ba101107
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071881"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="82d4c-103">emailAppUsageUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82d4c-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="82d4c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82d4c-104">Properties</span></span>

| <span data-ttu-id="82d4c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82d4c-105">Property</span></span>          | <span data-ttu-id="82d4c-106">型</span><span class="sxs-lookup"><span data-stu-id="82d4c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="82d4c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="82d4c-107">reportRefreshDate</span></span> | <span data-ttu-id="82d4c-108">Date</span><span class="sxs-lookup"><span data-stu-id="82d4c-108">Date</span></span>   |
| <span data-ttu-id="82d4c-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="82d4c-109">mailForMac</span></span>        | <span data-ttu-id="82d4c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-110">Int64</span></span>  |
| <span data-ttu-id="82d4c-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="82d4c-111">outlookForMac</span></span>     | <span data-ttu-id="82d4c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-112">Int64</span></span>  |
| <span data-ttu-id="82d4c-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="82d4c-113">outlookForWindows</span></span> | <span data-ttu-id="82d4c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-114">Int64</span></span>  |
| <span data-ttu-id="82d4c-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="82d4c-115">outlookForMobile</span></span>  | <span data-ttu-id="82d4c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-116">Int64</span></span>  |
| <span data-ttu-id="82d4c-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="82d4c-117">otherForMobile</span></span>    | <span data-ttu-id="82d4c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-118">Int64</span></span>  |
| <span data-ttu-id="82d4c-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="82d4c-119">outlookForWeb</span></span>     | <span data-ttu-id="82d4c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-120">Int64</span></span>  |
| <span data-ttu-id="82d4c-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="82d4c-121">pop3App</span></span>           | <span data-ttu-id="82d4c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-122">Int64</span></span>  |
| <span data-ttu-id="82d4c-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="82d4c-123">imap4App</span></span>          | <span data-ttu-id="82d4c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-124">Int64</span></span>  |
| <span data-ttu-id="82d4c-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="82d4c-125">smtpApp</span></span>           | <span data-ttu-id="82d4c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="82d4c-126">Int64</span></span>  |
| <span data-ttu-id="82d4c-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="82d4c-127">reportDate</span></span>        | <span data-ttu-id="82d4c-128">Date</span><span class="sxs-lookup"><span data-stu-id="82d4c-128">Date</span></span>   |
| <span data-ttu-id="82d4c-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="82d4c-129">reportPeriod</span></span>      | <span data-ttu-id="82d4c-130">String</span><span class="sxs-lookup"><span data-stu-id="82d4c-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="82d4c-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82d4c-131">JSON representation</span></span>

<span data-ttu-id="82d4c-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="82d4c-132">The following is a JSON representation of the resource.</span></span>

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
