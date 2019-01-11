---
title: skypeForBusinessDeviceUsageUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858381"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="b772c-103">skypeForBusinessDeviceUsageUserDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b772c-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b772c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b772c-104">Properties</span></span>

| <span data-ttu-id="b772c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b772c-105">Property</span></span>          | <span data-ttu-id="b772c-106">種類</span><span class="sxs-lookup"><span data-stu-id="b772c-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="b772c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b772c-107">reportRefreshDate</span></span> | <span data-ttu-id="b772c-108">日付</span><span class="sxs-lookup"><span data-stu-id="b772c-108">Date</span></span>    |
| <span data-ttu-id="b772c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b772c-109">userPrincipalName</span></span> | <span data-ttu-id="b772c-110">String</span><span class="sxs-lookup"><span data-stu-id="b772c-110">String</span></span>  |
| <span data-ttu-id="b772c-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="b772c-111">lastActivityDate</span></span>  | <span data-ttu-id="b772c-112">日付</span><span class="sxs-lookup"><span data-stu-id="b772c-112">Date</span></span>    |
| <span data-ttu-id="b772c-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="b772c-113">usedWindows</span></span>       | <span data-ttu-id="b772c-114">ブール型</span><span class="sxs-lookup"><span data-stu-id="b772c-114">Boolean</span></span> |
| <span data-ttu-id="b772c-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="b772c-115">usedWindowsPhone</span></span>  | <span data-ttu-id="b772c-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="b772c-116">Boolean</span></span> |
| <span data-ttu-id="b772c-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="b772c-117">usedAndroidPhone</span></span>  | <span data-ttu-id="b772c-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="b772c-118">Boolean</span></span> |
| <span data-ttu-id="b772c-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="b772c-119">usediPhone</span></span>        | <span data-ttu-id="b772c-120">ブール型</span><span class="sxs-lookup"><span data-stu-id="b772c-120">Boolean</span></span> |
| <span data-ttu-id="b772c-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="b772c-121">usediPad</span></span>          | <span data-ttu-id="b772c-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="b772c-122">Boolean</span></span> |
| <span data-ttu-id="b772c-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b772c-123">reportPeriod</span></span>      | <span data-ttu-id="b772c-124">String</span><span class="sxs-lookup"><span data-stu-id="b772c-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="b772c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b772c-125">JSON representation</span></span>

<span data-ttu-id="b772c-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b772c-126">The following is a JSON representation of the resource.</span></span>

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
