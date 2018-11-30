---
title: teamsDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: 4eeec5f07a0a604249617ac87a62ea12b4052395
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073764"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="766f5-103">teamsDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="766f5-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="766f5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="766f5-104">Properties</span></span>

| <span data-ttu-id="766f5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="766f5-105">Property</span></span>          | <span data-ttu-id="766f5-106">型</span><span class="sxs-lookup"><span data-stu-id="766f5-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="766f5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="766f5-107">reportRefreshDate</span></span> | <span data-ttu-id="766f5-108">Date</span><span class="sxs-lookup"><span data-stu-id="766f5-108">Date</span></span>    |
| <span data-ttu-id="766f5-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="766f5-109">userPrincipalName</span></span> | <span data-ttu-id="766f5-110">String</span><span class="sxs-lookup"><span data-stu-id="766f5-110">String</span></span>  |
| <span data-ttu-id="766f5-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="766f5-111">lastActivityDate</span></span>  | <span data-ttu-id="766f5-112">Date</span><span class="sxs-lookup"><span data-stu-id="766f5-112">Date</span></span>    |
| <span data-ttu-id="766f5-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="766f5-113">isDeleted</span></span>         | <span data-ttu-id="766f5-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="766f5-114">Boolean</span></span> |
| <span data-ttu-id="766f5-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="766f5-115">deletedDate</span></span>       | <span data-ttu-id="766f5-116">Date</span><span class="sxs-lookup"><span data-stu-id="766f5-116">Date</span></span>    |
| <span data-ttu-id="766f5-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="766f5-117">usedWeb</span></span>           | <span data-ttu-id="766f5-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="766f5-118">Boolean</span></span> |
| <span data-ttu-id="766f5-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="766f5-119">usedWindowsPhone</span></span>  | <span data-ttu-id="766f5-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="766f5-120">Boolean</span></span> |
| <span data-ttu-id="766f5-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="766f5-121">usediOS</span></span>           | <span data-ttu-id="766f5-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="766f5-122">Boolean</span></span> |
| <span data-ttu-id="766f5-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="766f5-123">usedMac</span></span>           | <span data-ttu-id="766f5-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="766f5-124">Boolean</span></span> |
| <span data-ttu-id="766f5-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="766f5-125">usedAndroidPhone</span></span>  | <span data-ttu-id="766f5-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="766f5-126">Boolean</span></span> |
| <span data-ttu-id="766f5-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="766f5-127">usedWindows</span></span>       | <span data-ttu-id="766f5-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="766f5-128">Boolean</span></span> |
| <span data-ttu-id="766f5-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="766f5-129">reportPeriod</span></span>      | <span data-ttu-id="766f5-130">String</span><span class="sxs-lookup"><span data-stu-id="766f5-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="766f5-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="766f5-131">JSON representation</span></span>

<span data-ttu-id="766f5-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="766f5-132">The following is a JSON representation of the resource.</span></span>

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
