---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42d0ecbb7745346d5fc8d25fbc1aa595c8f1887f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573460"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="5e0f3-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5e0f3-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="5e0f3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5e0f3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e0f3-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5e0f3-105">Not yet documented</span></span>


<span data-ttu-id="5e0f3-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="5e0f3-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e0f3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e0f3-107">Properties</span></span>
|<span data-ttu-id="5e0f3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e0f3-108">Property</span></span>|<span data-ttu-id="5e0f3-109">型</span><span class="sxs-lookup"><span data-stu-id="5e0f3-109">Type</span></span>|<span data-ttu-id="5e0f3-110">説明</span><span class="sxs-lookup"><span data-stu-id="5e0f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e0f3-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="5e0f3-111">activeHoursStart</span></span>|<span data-ttu-id="5e0f3-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5e0f3-112">TimeOfDay</span></span>|<span data-ttu-id="5e0f3-113">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="5e0f3-113">Active Hours Start</span></span>|
|<span data-ttu-id="5e0f3-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="5e0f3-114">activeHoursEnd</span></span>|<span data-ttu-id="5e0f3-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5e0f3-115">TimeOfDay</span></span>|<span data-ttu-id="5e0f3-116">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="5e0f3-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e0f3-117">関係</span><span class="sxs-lookup"><span data-stu-id="5e0f3-117">Relationships</span></span>
<span data-ttu-id="5e0f3-118">なし</span><span class="sxs-lookup"><span data-stu-id="5e0f3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e0f3-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5e0f3-119">JSON Representation</span></span>
<span data-ttu-id="5e0f3-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5e0f3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



