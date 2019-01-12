---
title: emailAppUsageAppsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970382"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="28f89-103">emailAppUsageAppsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28f89-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="28f89-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28f89-104">Properties</span></span>

| <span data-ttu-id="28f89-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28f89-105">Property</span></span>          | <span data-ttu-id="28f89-106">種類</span><span class="sxs-lookup"><span data-stu-id="28f89-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="28f89-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="28f89-107">reportRefreshDate</span></span> | <span data-ttu-id="28f89-108">日付</span><span class="sxs-lookup"><span data-stu-id="28f89-108">Date</span></span>   |
| <span data-ttu-id="28f89-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="28f89-109">mailForMac</span></span>        | <span data-ttu-id="28f89-110">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-110">Int64</span></span>  |
| <span data-ttu-id="28f89-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="28f89-111">outlookForMac</span></span>     | <span data-ttu-id="28f89-112">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-112">Int64</span></span>  |
| <span data-ttu-id="28f89-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="28f89-113">outlookForWindows</span></span> | <span data-ttu-id="28f89-114">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-114">Int64</span></span>  |
| <span data-ttu-id="28f89-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="28f89-115">outlookForMobile</span></span>  | <span data-ttu-id="28f89-116">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-116">Int64</span></span>  |
| <span data-ttu-id="28f89-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="28f89-117">otherForMobile</span></span>    | <span data-ttu-id="28f89-118">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-118">Int64</span></span>  |
| <span data-ttu-id="28f89-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="28f89-119">outlookForWeb</span></span>     | <span data-ttu-id="28f89-120">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-120">Int64</span></span>  |
| <span data-ttu-id="28f89-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="28f89-121">pop3App</span></span>           | <span data-ttu-id="28f89-122">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-122">Int64</span></span>  |
| <span data-ttu-id="28f89-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="28f89-123">imap4App</span></span>          | <span data-ttu-id="28f89-124">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-124">Int64</span></span>  |
| <span data-ttu-id="28f89-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="28f89-125">smtpApp</span></span>           | <span data-ttu-id="28f89-126">Int64</span><span class="sxs-lookup"><span data-stu-id="28f89-126">Int64</span></span>  |
| <span data-ttu-id="28f89-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="28f89-127">reportPeriod</span></span>      | <span data-ttu-id="28f89-128">String</span><span class="sxs-lookup"><span data-stu-id="28f89-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="28f89-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28f89-129">JSON representation</span></span>

<span data-ttu-id="28f89-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="28f89-130">The following is a JSON representation of the resource.</span></span>

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
