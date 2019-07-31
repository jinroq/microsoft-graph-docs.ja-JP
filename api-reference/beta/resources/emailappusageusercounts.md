---
title: Emailappの User計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d8af9e9337c68fcd4434514b85fa9217c79add26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972174"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="26591-103">Emailappの User計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="26591-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="26591-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26591-104">Properties</span></span>

| <span data-ttu-id="26591-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26591-105">Property</span></span>          | <span data-ttu-id="26591-106">型</span><span class="sxs-lookup"><span data-stu-id="26591-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="26591-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="26591-107">reportRefreshDate</span></span> | <span data-ttu-id="26591-108">日付</span><span class="sxs-lookup"><span data-stu-id="26591-108">Date</span></span>   |
| <span data-ttu-id="26591-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="26591-109">mailForMac</span></span>        | <span data-ttu-id="26591-110">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-110">Int64</span></span>  |
| <span data-ttu-id="26591-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="26591-111">outlookForMac</span></span>     | <span data-ttu-id="26591-112">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-112">Int64</span></span>  |
| <span data-ttu-id="26591-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="26591-113">outlookForWindows</span></span> | <span data-ttu-id="26591-114">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-114">Int64</span></span>  |
| <span data-ttu-id="26591-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="26591-115">outlookForMobile</span></span>  | <span data-ttu-id="26591-116">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-116">Int64</span></span>  |
| <span data-ttu-id="26591-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="26591-117">otherForMobile</span></span>    | <span data-ttu-id="26591-118">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-118">Int64</span></span>  |
| <span data-ttu-id="26591-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="26591-119">outlookForWeb</span></span>     | <span data-ttu-id="26591-120">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-120">Int64</span></span>  |
| <span data-ttu-id="26591-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="26591-121">pop3App</span></span>           | <span data-ttu-id="26591-122">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-122">Int64</span></span>  |
| <span data-ttu-id="26591-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="26591-123">imap4App</span></span>          | <span data-ttu-id="26591-124">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-124">Int64</span></span>  |
| <span data-ttu-id="26591-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="26591-125">smtpApp</span></span>           | <span data-ttu-id="26591-126">Int64</span><span class="sxs-lookup"><span data-stu-id="26591-126">Int64</span></span>  |
| <span data-ttu-id="26591-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="26591-127">reportDate</span></span>        | <span data-ttu-id="26591-128">日付</span><span class="sxs-lookup"><span data-stu-id="26591-128">Date</span></span>   |
| <span data-ttu-id="26591-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="26591-129">reportPeriod</span></span>      | <span data-ttu-id="26591-130">String</span><span class="sxs-lookup"><span data-stu-id="26591-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="26591-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="26591-131">JSON representation</span></span>

<span data-ttu-id="26591-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26591-132">The following is a JSON representation of the resource.</span></span>

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
