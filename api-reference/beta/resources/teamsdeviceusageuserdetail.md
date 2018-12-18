---
title: teamsDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
author: nkramer
ms.openlocfilehash: 1947b66a59190945e5a6b823b47ef8df7d02683a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329002"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="f4211-103">teamsDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4211-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f4211-104">Properties</span><span class="sxs-lookup"><span data-stu-id="f4211-104">Properties</span></span>

| <span data-ttu-id="f4211-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4211-105">Property</span></span>          | <span data-ttu-id="f4211-106">種類</span><span class="sxs-lookup"><span data-stu-id="f4211-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="f4211-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f4211-107">reportRefreshDate</span></span> | <span data-ttu-id="f4211-108">日付</span><span class="sxs-lookup"><span data-stu-id="f4211-108">Date</span></span>    |
| <span data-ttu-id="f4211-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4211-109">userPrincipalName</span></span> | <span data-ttu-id="f4211-110">String</span><span class="sxs-lookup"><span data-stu-id="f4211-110">String</span></span>  |
| <span data-ttu-id="f4211-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f4211-111">lastActivityDate</span></span>  | <span data-ttu-id="f4211-112">日付</span><span class="sxs-lookup"><span data-stu-id="f4211-112">Date</span></span>    |
| <span data-ttu-id="f4211-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f4211-113">isDeleted</span></span>         | <span data-ttu-id="f4211-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="f4211-114">Boolean</span></span> |
| <span data-ttu-id="f4211-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="f4211-115">deletedDate</span></span>       | <span data-ttu-id="f4211-116">日付</span><span class="sxs-lookup"><span data-stu-id="f4211-116">Date</span></span>    |
| <span data-ttu-id="f4211-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="f4211-117">usedWeb</span></span>           | <span data-ttu-id="f4211-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="f4211-118">Boolean</span></span> |
| <span data-ttu-id="f4211-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="f4211-119">usedWindowsPhone</span></span>  | <span data-ttu-id="f4211-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="f4211-120">Boolean</span></span> |
| <span data-ttu-id="f4211-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="f4211-121">usediOS</span></span>           | <span data-ttu-id="f4211-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="f4211-122">Boolean</span></span> |
| <span data-ttu-id="f4211-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="f4211-123">usedMac</span></span>           | <span data-ttu-id="f4211-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="f4211-124">Boolean</span></span> |
| <span data-ttu-id="f4211-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="f4211-125">usedAndroidPhone</span></span>  | <span data-ttu-id="f4211-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="f4211-126">Boolean</span></span> |
| <span data-ttu-id="f4211-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="f4211-127">usedWindows</span></span>       | <span data-ttu-id="f4211-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="f4211-128">Boolean</span></span> |
| <span data-ttu-id="f4211-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f4211-129">reportPeriod</span></span>      | <span data-ttu-id="f4211-130">String</span><span class="sxs-lookup"><span data-stu-id="f4211-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f4211-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4211-131">JSON representation</span></span>

<span data-ttu-id="f4211-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4211-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
