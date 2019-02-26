---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42d0ecbb7745346d5fc8d25fbc1aa595c8f1887f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264058"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="868dc-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="868dc-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="868dc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="868dc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="868dc-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="868dc-105">Not yet documented</span></span>


<span data-ttu-id="868dc-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="868dc-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="868dc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="868dc-107">Properties</span></span>
|<span data-ttu-id="868dc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="868dc-108">Property</span></span>|<span data-ttu-id="868dc-109">型</span><span class="sxs-lookup"><span data-stu-id="868dc-109">Type</span></span>|<span data-ttu-id="868dc-110">説明</span><span class="sxs-lookup"><span data-stu-id="868dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="868dc-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="868dc-111">activeHoursStart</span></span>|<span data-ttu-id="868dc-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="868dc-112">TimeOfDay</span></span>|<span data-ttu-id="868dc-113">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="868dc-113">Active Hours Start</span></span>|
|<span data-ttu-id="868dc-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="868dc-114">activeHoursEnd</span></span>|<span data-ttu-id="868dc-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="868dc-115">TimeOfDay</span></span>|<span data-ttu-id="868dc-116">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="868dc-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="868dc-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="868dc-117">Relationships</span></span>
<span data-ttu-id="868dc-118">なし</span><span class="sxs-lookup"><span data-stu-id="868dc-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="868dc-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="868dc-119">JSON Representation</span></span>
<span data-ttu-id="868dc-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="868dc-120">Here is a JSON representation of the resource.</span></span>
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



