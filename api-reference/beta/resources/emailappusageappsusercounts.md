---
title: emailAppUsageAppsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: efbc4ce75293237813e9a835cb45ff0bf0ec4b26
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807820"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="2018c-103">emailAppUsageAppsUserCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2018c-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2018c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2018c-104">Properties</span></span>

| <span data-ttu-id="2018c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2018c-105">Property</span></span>          | <span data-ttu-id="2018c-106">種類</span><span class="sxs-lookup"><span data-stu-id="2018c-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2018c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2018c-107">reportRefreshDate</span></span> | <span data-ttu-id="2018c-108">日付</span><span class="sxs-lookup"><span data-stu-id="2018c-108">Date</span></span>   |
| <span data-ttu-id="2018c-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="2018c-109">mailForMac</span></span>        | <span data-ttu-id="2018c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-110">Int64</span></span>  |
| <span data-ttu-id="2018c-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="2018c-111">outlookForMac</span></span>     | <span data-ttu-id="2018c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-112">Int64</span></span>  |
| <span data-ttu-id="2018c-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="2018c-113">outlookForWindows</span></span> | <span data-ttu-id="2018c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-114">Int64</span></span>  |
| <span data-ttu-id="2018c-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="2018c-115">outlookForMobile</span></span>  | <span data-ttu-id="2018c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-116">Int64</span></span>  |
| <span data-ttu-id="2018c-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="2018c-117">otherForMobile</span></span>    | <span data-ttu-id="2018c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-118">Int64</span></span>  |
| <span data-ttu-id="2018c-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="2018c-119">outlookForWeb</span></span>     | <span data-ttu-id="2018c-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-120">Int64</span></span>  |
| <span data-ttu-id="2018c-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="2018c-121">pop3App</span></span>           | <span data-ttu-id="2018c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-122">Int64</span></span>  |
| <span data-ttu-id="2018c-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="2018c-123">imap4App</span></span>          | <span data-ttu-id="2018c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-124">Int64</span></span>  |
| <span data-ttu-id="2018c-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="2018c-125">smtpApp</span></span>           | <span data-ttu-id="2018c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="2018c-126">Int64</span></span>  |
| <span data-ttu-id="2018c-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2018c-127">reportPeriod</span></span>      | <span data-ttu-id="2018c-128">String</span><span class="sxs-lookup"><span data-stu-id="2018c-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2018c-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2018c-129">JSON representation</span></span>

<span data-ttu-id="2018c-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2018c-130">The following is a JSON representation of the resource.</span></span>

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
