---
title: emailappの appsuser計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542812"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="89db0-103">emailappの appsuser計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89db0-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="89db0-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89db0-104">Properties</span></span>

| <span data-ttu-id="89db0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89db0-105">Property</span></span>          | <span data-ttu-id="89db0-106">型</span><span class="sxs-lookup"><span data-stu-id="89db0-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="89db0-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="89db0-107">reportRefreshDate</span></span> | <span data-ttu-id="89db0-108">Date</span><span class="sxs-lookup"><span data-stu-id="89db0-108">Date</span></span>   |
| <span data-ttu-id="89db0-109">mailformac</span><span class="sxs-lookup"><span data-stu-id="89db0-109">mailForMac</span></span>        | <span data-ttu-id="89db0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-110">Int64</span></span>  |
| <span data-ttu-id="89db0-111">outlookformac</span><span class="sxs-lookup"><span data-stu-id="89db0-111">outlookForMac</span></span>     | <span data-ttu-id="89db0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-112">Int64</span></span>  |
| <span data-ttu-id="89db0-113">outlookforwindows</span><span class="sxs-lookup"><span data-stu-id="89db0-113">outlookForWindows</span></span> | <span data-ttu-id="89db0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-114">Int64</span></span>  |
| <span data-ttu-id="89db0-115">outlookformobile</span><span class="sxs-lookup"><span data-stu-id="89db0-115">outlookForMobile</span></span>  | <span data-ttu-id="89db0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-116">Int64</span></span>  |
| <span data-ttu-id="89db0-117">otherformobile</span><span class="sxs-lookup"><span data-stu-id="89db0-117">otherForMobile</span></span>    | <span data-ttu-id="89db0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-118">Int64</span></span>  |
| <span data-ttu-id="89db0-119">outlookforweb</span><span class="sxs-lookup"><span data-stu-id="89db0-119">outlookForWeb</span></span>     | <span data-ttu-id="89db0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-120">Int64</span></span>  |
| <span data-ttu-id="89db0-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="89db0-121">pop3App</span></span>           | <span data-ttu-id="89db0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-122">Int64</span></span>  |
| <span data-ttu-id="89db0-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="89db0-123">imap4App</span></span>          | <span data-ttu-id="89db0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-124">Int64</span></span>  |
| <span data-ttu-id="89db0-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="89db0-125">smtpApp</span></span>           | <span data-ttu-id="89db0-126">Int64</span><span class="sxs-lookup"><span data-stu-id="89db0-126">Int64</span></span>  |
| <span data-ttu-id="89db0-127">reportperiod</span><span class="sxs-lookup"><span data-stu-id="89db0-127">reportPeriod</span></span>      | <span data-ttu-id="89db0-128">String</span><span class="sxs-lookup"><span data-stu-id="89db0-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="89db0-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89db0-129">JSON representation</span></span>

<span data-ttu-id="89db0-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89db0-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
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
  "reportPeriod": "String"
}
```
