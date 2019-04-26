---
title: skypeforbusinessdevice使い方 userdetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: 95f2f6cf1f3f6c54c4b6b4b39a7118cd8a94b224
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555935"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="78ff8-103">skypeforbusinessdevice使い方 userdetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78ff8-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="78ff8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78ff8-104">Properties</span></span>

| <span data-ttu-id="78ff8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78ff8-105">Property</span></span>          | <span data-ttu-id="78ff8-106">型</span><span class="sxs-lookup"><span data-stu-id="78ff8-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="78ff8-107">reportrefreshdate</span><span class="sxs-lookup"><span data-stu-id="78ff8-107">reportRefreshDate</span></span> | <span data-ttu-id="78ff8-108">Date</span><span class="sxs-lookup"><span data-stu-id="78ff8-108">Date</span></span>    |
| <span data-ttu-id="78ff8-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="78ff8-109">userPrincipalName</span></span> | <span data-ttu-id="78ff8-110">String</span><span class="sxs-lookup"><span data-stu-id="78ff8-110">String</span></span>  |
| <span data-ttu-id="78ff8-111">lastactivitydate</span><span class="sxs-lookup"><span data-stu-id="78ff8-111">lastActivityDate</span></span>  | <span data-ttu-id="78ff8-112">Date</span><span class="sxs-lookup"><span data-stu-id="78ff8-112">Date</span></span>    |
| <span data-ttu-id="78ff8-113">未使用のウィンドウ</span><span class="sxs-lookup"><span data-stu-id="78ff8-113">usedWindows</span></span>       | <span data-ttu-id="78ff8-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="78ff8-114">Boolean</span></span> |
| <span data-ttu-id="78ff8-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="78ff8-115">usedWindowsPhone</span></span>  | <span data-ttu-id="78ff8-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="78ff8-116">Boolean</span></span> |
| <span data-ttu-id="78ff8-117">used androidphone</span><span class="sxs-lookup"><span data-stu-id="78ff8-117">usedAndroidPhone</span></span>  | <span data-ttu-id="78ff8-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="78ff8-118">Boolean</span></span> |
| <span data-ttu-id="78ff8-119">usediphone</span><span class="sxs-lookup"><span data-stu-id="78ff8-119">usediPhone</span></span>        | <span data-ttu-id="78ff8-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="78ff8-120">Boolean</span></span> |
| <span data-ttu-id="78ff8-121">usedipad</span><span class="sxs-lookup"><span data-stu-id="78ff8-121">usediPad</span></span>          | <span data-ttu-id="78ff8-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="78ff8-122">Boolean</span></span> |
| <span data-ttu-id="78ff8-123">reportperiod</span><span class="sxs-lookup"><span data-stu-id="78ff8-123">reportPeriod</span></span>      | <span data-ttu-id="78ff8-124">String</span><span class="sxs-lookup"><span data-stu-id="78ff8-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="78ff8-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78ff8-125">JSON representation</span></span>

<span data-ttu-id="78ff8-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="78ff8-126">The following is a JSON representation of the resource.</span></span>

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
