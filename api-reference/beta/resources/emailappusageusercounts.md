---
title: emailappの user計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7822528aacc9d6f104012d43004fbb9aabba127c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506693"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="313b6-103">emailappの user計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="313b6-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="313b6-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="313b6-104">Properties</span></span>

| <span data-ttu-id="313b6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="313b6-105">Property</span></span>          | <span data-ttu-id="313b6-106">型</span><span class="sxs-lookup"><span data-stu-id="313b6-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="313b6-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="313b6-107">reportRefreshDate</span></span> | <span data-ttu-id="313b6-108">Date</span><span class="sxs-lookup"><span data-stu-id="313b6-108">Date</span></span>   |
| <span data-ttu-id="313b6-109">mailformac</span><span class="sxs-lookup"><span data-stu-id="313b6-109">mailForMac</span></span>        | <span data-ttu-id="313b6-110">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-110">Int64</span></span>  |
| <span data-ttu-id="313b6-111">outlookformac</span><span class="sxs-lookup"><span data-stu-id="313b6-111">outlookForMac</span></span>     | <span data-ttu-id="313b6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-112">Int64</span></span>  |
| <span data-ttu-id="313b6-113">outlookforwindows</span><span class="sxs-lookup"><span data-stu-id="313b6-113">outlookForWindows</span></span> | <span data-ttu-id="313b6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-114">Int64</span></span>  |
| <span data-ttu-id="313b6-115">outlookformobile</span><span class="sxs-lookup"><span data-stu-id="313b6-115">outlookForMobile</span></span>  | <span data-ttu-id="313b6-116">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-116">Int64</span></span>  |
| <span data-ttu-id="313b6-117">otherformobile</span><span class="sxs-lookup"><span data-stu-id="313b6-117">otherForMobile</span></span>    | <span data-ttu-id="313b6-118">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-118">Int64</span></span>  |
| <span data-ttu-id="313b6-119">outlookforweb</span><span class="sxs-lookup"><span data-stu-id="313b6-119">outlookForWeb</span></span>     | <span data-ttu-id="313b6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-120">Int64</span></span>  |
| <span data-ttu-id="313b6-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="313b6-121">pop3App</span></span>           | <span data-ttu-id="313b6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-122">Int64</span></span>  |
| <span data-ttu-id="313b6-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="313b6-123">imap4App</span></span>          | <span data-ttu-id="313b6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-124">Int64</span></span>  |
| <span data-ttu-id="313b6-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="313b6-125">smtpApp</span></span>           | <span data-ttu-id="313b6-126">Int64</span><span class="sxs-lookup"><span data-stu-id="313b6-126">Int64</span></span>  |
| <span data-ttu-id="313b6-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="313b6-127">reportDate</span></span>        | <span data-ttu-id="313b6-128">Date</span><span class="sxs-lookup"><span data-stu-id="313b6-128">Date</span></span>   |
| <span data-ttu-id="313b6-129">reportperiod</span><span class="sxs-lookup"><span data-stu-id="313b6-129">reportPeriod</span></span>      | <span data-ttu-id="313b6-130">String</span><span class="sxs-lookup"><span data-stu-id="313b6-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="313b6-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="313b6-131">JSON representation</span></span>

<span data-ttu-id="313b6-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="313b6-132">The following is a JSON representation of the resource.</span></span>

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
