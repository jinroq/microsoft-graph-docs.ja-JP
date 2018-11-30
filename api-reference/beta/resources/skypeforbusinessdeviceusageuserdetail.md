---
title: skypeForBusinessDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
ms.openlocfilehash: b62920d124fd52e0f653c128eeb0956cdfe0c680
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068048"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="129fc-103">skypeForBusinessDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="129fc-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="129fc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="129fc-104">Properties</span></span>

| <span data-ttu-id="129fc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="129fc-105">Property</span></span>          | <span data-ttu-id="129fc-106">型</span><span class="sxs-lookup"><span data-stu-id="129fc-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="129fc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="129fc-107">reportRefreshDate</span></span> | <span data-ttu-id="129fc-108">Date</span><span class="sxs-lookup"><span data-stu-id="129fc-108">Date</span></span>    |
| <span data-ttu-id="129fc-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="129fc-109">userPrincipalName</span></span> | <span data-ttu-id="129fc-110">String</span><span class="sxs-lookup"><span data-stu-id="129fc-110">String</span></span>  |
| <span data-ttu-id="129fc-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="129fc-111">lastActivityDate</span></span>  | <span data-ttu-id="129fc-112">Date</span><span class="sxs-lookup"><span data-stu-id="129fc-112">Date</span></span>    |
| <span data-ttu-id="129fc-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="129fc-113">usedWindows</span></span>       | <span data-ttu-id="129fc-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="129fc-114">Boolean</span></span> |
| <span data-ttu-id="129fc-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="129fc-115">usedWindowsPhone</span></span>  | <span data-ttu-id="129fc-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="129fc-116">Boolean</span></span> |
| <span data-ttu-id="129fc-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="129fc-117">usedAndroidPhone</span></span>  | <span data-ttu-id="129fc-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="129fc-118">Boolean</span></span> |
| <span data-ttu-id="129fc-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="129fc-119">usediPhone</span></span>        | <span data-ttu-id="129fc-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="129fc-120">Boolean</span></span> |
| <span data-ttu-id="129fc-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="129fc-121">usediPad</span></span>          | <span data-ttu-id="129fc-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="129fc-122">Boolean</span></span> |
| <span data-ttu-id="129fc-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="129fc-123">reportPeriod</span></span>      | <span data-ttu-id="129fc-124">String</span><span class="sxs-lookup"><span data-stu-id="129fc-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="129fc-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="129fc-125">JSON representation</span></span>

<span data-ttu-id="129fc-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="129fc-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
