---
title: yammerDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5fe3aa7fa9da243c9cc8f9b015ee85d779b84eb3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574153"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="7ba80-103">yammerDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7ba80-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="7ba80-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ba80-104">Properties</span></span>

| <span data-ttu-id="7ba80-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ba80-105">Property</span></span>          | <span data-ttu-id="7ba80-106">型</span><span class="sxs-lookup"><span data-stu-id="7ba80-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="7ba80-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7ba80-107">reportRefreshDate</span></span> | <span data-ttu-id="7ba80-108">日付</span><span class="sxs-lookup"><span data-stu-id="7ba80-108">Date</span></span>    |
| <span data-ttu-id="7ba80-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7ba80-109">userPrincipalName</span></span> | <span data-ttu-id="7ba80-110">String</span><span class="sxs-lookup"><span data-stu-id="7ba80-110">String</span></span>  |
| <span data-ttu-id="7ba80-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7ba80-111">displayName</span></span>       | <span data-ttu-id="7ba80-112">String</span><span class="sxs-lookup"><span data-stu-id="7ba80-112">String</span></span>  |
| <span data-ttu-id="7ba80-113">userState</span><span class="sxs-lookup"><span data-stu-id="7ba80-113">userState</span></span>         | <span data-ttu-id="7ba80-114">String</span><span class="sxs-lookup"><span data-stu-id="7ba80-114">String</span></span>  |
| <span data-ttu-id="7ba80-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="7ba80-115">stateChangeDate</span></span>   | <span data-ttu-id="7ba80-116">日付</span><span class="sxs-lookup"><span data-stu-id="7ba80-116">Date</span></span>    |
| <span data-ttu-id="7ba80-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7ba80-117">lastActivityDate</span></span>  | <span data-ttu-id="7ba80-118">日付</span><span class="sxs-lookup"><span data-stu-id="7ba80-118">Date</span></span>    |
| <span data-ttu-id="7ba80-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="7ba80-119">usedWeb</span></span>           | <span data-ttu-id="7ba80-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba80-120">Boolean</span></span> |
| <span data-ttu-id="7ba80-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="7ba80-121">usedWindowsPhone</span></span>  | <span data-ttu-id="7ba80-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba80-122">Boolean</span></span> |
| <span data-ttu-id="7ba80-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="7ba80-123">usedAndroidPhone</span></span>  | <span data-ttu-id="7ba80-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba80-124">Boolean</span></span> |
| <span data-ttu-id="7ba80-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="7ba80-125">usediPhone</span></span>        | <span data-ttu-id="7ba80-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba80-126">Boolean</span></span> |
| <span data-ttu-id="7ba80-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="7ba80-127">usediPad</span></span>          | <span data-ttu-id="7ba80-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba80-128">Boolean</span></span> |
| <span data-ttu-id="7ba80-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="7ba80-129">usedOthers</span></span>        | <span data-ttu-id="7ba80-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ba80-130">Boolean</span></span> |
| <span data-ttu-id="7ba80-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7ba80-131">reportPeriod</span></span>      | <span data-ttu-id="7ba80-132">String</span><span class="sxs-lookup"><span data-stu-id="7ba80-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7ba80-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7ba80-133">JSON representation</span></span>

<span data-ttu-id="7ba80-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ba80-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
