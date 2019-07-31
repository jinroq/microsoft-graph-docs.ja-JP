---
title: yammerDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 083ace4b10b24e8e5de5d287ddf418d93658c879
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006982"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="010bd-103">yammerDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="010bd-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="010bd-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="010bd-104">Properties</span></span>

| <span data-ttu-id="010bd-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="010bd-105">Property</span></span>          | <span data-ttu-id="010bd-106">型</span><span class="sxs-lookup"><span data-stu-id="010bd-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="010bd-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="010bd-107">reportRefreshDate</span></span> | <span data-ttu-id="010bd-108">日付</span><span class="sxs-lookup"><span data-stu-id="010bd-108">Date</span></span>    |
| <span data-ttu-id="010bd-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="010bd-109">userPrincipalName</span></span> | <span data-ttu-id="010bd-110">String</span><span class="sxs-lookup"><span data-stu-id="010bd-110">String</span></span>  |
| <span data-ttu-id="010bd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="010bd-111">displayName</span></span>       | <span data-ttu-id="010bd-112">文字列</span><span class="sxs-lookup"><span data-stu-id="010bd-112">String</span></span>  |
| <span data-ttu-id="010bd-113">userState</span><span class="sxs-lookup"><span data-stu-id="010bd-113">userState</span></span>         | <span data-ttu-id="010bd-114">String</span><span class="sxs-lookup"><span data-stu-id="010bd-114">String</span></span>  |
| <span data-ttu-id="010bd-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="010bd-115">stateChangeDate</span></span>   | <span data-ttu-id="010bd-116">日付</span><span class="sxs-lookup"><span data-stu-id="010bd-116">Date</span></span>    |
| <span data-ttu-id="010bd-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="010bd-117">lastActivityDate</span></span>  | <span data-ttu-id="010bd-118">日付</span><span class="sxs-lookup"><span data-stu-id="010bd-118">Date</span></span>    |
| <span data-ttu-id="010bd-119">Used Web</span><span class="sxs-lookup"><span data-stu-id="010bd-119">usedWeb</span></span>           | <span data-ttu-id="010bd-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="010bd-120">Boolean</span></span> |
| <span data-ttu-id="010bd-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="010bd-121">usedWindowsPhone</span></span>  | <span data-ttu-id="010bd-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="010bd-122">Boolean</span></span> |
| <span data-ttu-id="010bd-123">Used Androidphone</span><span class="sxs-lookup"><span data-stu-id="010bd-123">usedAndroidPhone</span></span>  | <span data-ttu-id="010bd-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="010bd-124">Boolean</span></span> |
| <span data-ttu-id="010bd-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="010bd-125">usediPhone</span></span>        | <span data-ttu-id="010bd-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="010bd-126">Boolean</span></span> |
| <span data-ttu-id="010bd-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="010bd-127">usediPad</span></span>          | <span data-ttu-id="010bd-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="010bd-128">Boolean</span></span> |
| <span data-ttu-id="010bd-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="010bd-129">usedOthers</span></span>        | <span data-ttu-id="010bd-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="010bd-130">Boolean</span></span> |
| <span data-ttu-id="010bd-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="010bd-131">reportPeriod</span></span>      | <span data-ttu-id="010bd-132">String</span><span class="sxs-lookup"><span data-stu-id="010bd-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="010bd-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="010bd-133">JSON representation</span></span>

<span data-ttu-id="010bd-134">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="010bd-134">The following is a JSON representation of the resource.</span></span>

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
