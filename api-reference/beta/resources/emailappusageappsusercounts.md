---
title: Emailappの Appsuser計数リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0ca694c5d416dcc062984ba03a3521a39a010a87
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972181"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="31d01-103">Emailappの Appsuser計数リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31d01-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="31d01-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31d01-104">Properties</span></span>

| <span data-ttu-id="31d01-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31d01-105">Property</span></span>          | <span data-ttu-id="31d01-106">型</span><span class="sxs-lookup"><span data-stu-id="31d01-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="31d01-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="31d01-107">reportRefreshDate</span></span> | <span data-ttu-id="31d01-108">日付</span><span class="sxs-lookup"><span data-stu-id="31d01-108">Date</span></span>   |
| <span data-ttu-id="31d01-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="31d01-109">mailForMac</span></span>        | <span data-ttu-id="31d01-110">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-110">Int64</span></span>  |
| <span data-ttu-id="31d01-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="31d01-111">outlookForMac</span></span>     | <span data-ttu-id="31d01-112">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-112">Int64</span></span>  |
| <span data-ttu-id="31d01-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="31d01-113">outlookForWindows</span></span> | <span data-ttu-id="31d01-114">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-114">Int64</span></span>  |
| <span data-ttu-id="31d01-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="31d01-115">outlookForMobile</span></span>  | <span data-ttu-id="31d01-116">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-116">Int64</span></span>  |
| <span data-ttu-id="31d01-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="31d01-117">otherForMobile</span></span>    | <span data-ttu-id="31d01-118">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-118">Int64</span></span>  |
| <span data-ttu-id="31d01-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="31d01-119">outlookForWeb</span></span>     | <span data-ttu-id="31d01-120">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-120">Int64</span></span>  |
| <span data-ttu-id="31d01-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="31d01-121">pop3App</span></span>           | <span data-ttu-id="31d01-122">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-122">Int64</span></span>  |
| <span data-ttu-id="31d01-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="31d01-123">imap4App</span></span>          | <span data-ttu-id="31d01-124">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-124">Int64</span></span>  |
| <span data-ttu-id="31d01-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="31d01-125">smtpApp</span></span>           | <span data-ttu-id="31d01-126">Int64</span><span class="sxs-lookup"><span data-stu-id="31d01-126">Int64</span></span>  |
| <span data-ttu-id="31d01-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="31d01-127">reportPeriod</span></span>      | <span data-ttu-id="31d01-128">String</span><span class="sxs-lookup"><span data-stu-id="31d01-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31d01-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31d01-129">JSON representation</span></span>

<span data-ttu-id="31d01-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31d01-130">The following is a JSON representation of the resource.</span></span>

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
