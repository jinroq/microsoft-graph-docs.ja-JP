---
title: yammerDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2b74222c1a636fac271268e228c8140e7d1cf33f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912009"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="f20fb-103">yammerDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f20fb-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f20fb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f20fb-104">Properties</span></span>

| <span data-ttu-id="f20fb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f20fb-105">Property</span></span>          | <span data-ttu-id="f20fb-106">種類</span><span class="sxs-lookup"><span data-stu-id="f20fb-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="f20fb-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f20fb-107">reportRefreshDate</span></span> | <span data-ttu-id="f20fb-108">日付</span><span class="sxs-lookup"><span data-stu-id="f20fb-108">Date</span></span>    |
| <span data-ttu-id="f20fb-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f20fb-109">userPrincipalName</span></span> | <span data-ttu-id="f20fb-110">String</span><span class="sxs-lookup"><span data-stu-id="f20fb-110">String</span></span>  |
| <span data-ttu-id="f20fb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f20fb-111">displayName</span></span>       | <span data-ttu-id="f20fb-112">String</span><span class="sxs-lookup"><span data-stu-id="f20fb-112">String</span></span>  |
| <span data-ttu-id="f20fb-113">userState</span><span class="sxs-lookup"><span data-stu-id="f20fb-113">userState</span></span>         | <span data-ttu-id="f20fb-114">String</span><span class="sxs-lookup"><span data-stu-id="f20fb-114">String</span></span>  |
| <span data-ttu-id="f20fb-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="f20fb-115">stateChangeDate</span></span>   | <span data-ttu-id="f20fb-116">日付</span><span class="sxs-lookup"><span data-stu-id="f20fb-116">Date</span></span>    |
| <span data-ttu-id="f20fb-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f20fb-117">lastActivityDate</span></span>  | <span data-ttu-id="f20fb-118">日付</span><span class="sxs-lookup"><span data-stu-id="f20fb-118">Date</span></span>    |
| <span data-ttu-id="f20fb-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="f20fb-119">usedWeb</span></span>           | <span data-ttu-id="f20fb-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="f20fb-120">Boolean</span></span> |
| <span data-ttu-id="f20fb-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="f20fb-121">usedWindowsPhone</span></span>  | <span data-ttu-id="f20fb-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="f20fb-122">Boolean</span></span> |
| <span data-ttu-id="f20fb-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="f20fb-123">usedAndroidPhone</span></span>  | <span data-ttu-id="f20fb-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="f20fb-124">Boolean</span></span> |
| <span data-ttu-id="f20fb-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="f20fb-125">usediPhone</span></span>        | <span data-ttu-id="f20fb-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="f20fb-126">Boolean</span></span> |
| <span data-ttu-id="f20fb-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="f20fb-127">usediPad</span></span>          | <span data-ttu-id="f20fb-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="f20fb-128">Boolean</span></span> |
| <span data-ttu-id="f20fb-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="f20fb-129">usedOthers</span></span>        | <span data-ttu-id="f20fb-130">ブール型</span><span class="sxs-lookup"><span data-stu-id="f20fb-130">Boolean</span></span> |
| <span data-ttu-id="f20fb-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f20fb-131">reportPeriod</span></span>      | <span data-ttu-id="f20fb-132">String</span><span class="sxs-lookup"><span data-stu-id="f20fb-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f20fb-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f20fb-133">JSON representation</span></span>

<span data-ttu-id="f20fb-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f20fb-134">The following is a JSON representation of the resource.</span></span>

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
