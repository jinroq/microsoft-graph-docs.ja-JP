---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b3c6d5fa7e517713d1904d33c94bcd8dccec5d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030899"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="41f2d-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41f2d-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="41f2d-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="41f2d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41f2d-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="41f2d-105">Not yet documented</span></span>


<span data-ttu-id="41f2d-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="41f2d-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="41f2d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41f2d-107">Properties</span></span>
|<span data-ttu-id="41f2d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41f2d-108">Property</span></span>|<span data-ttu-id="41f2d-109">型</span><span class="sxs-lookup"><span data-stu-id="41f2d-109">Type</span></span>|<span data-ttu-id="41f2d-110">説明</span><span class="sxs-lookup"><span data-stu-id="41f2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41f2d-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="41f2d-111">scheduledInstallDay</span></span>|[<span data-ttu-id="41f2d-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="41f2d-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="41f2d-113">スケジュールされたインストール日 (週単位)。</span><span class="sxs-lookup"><span data-stu-id="41f2d-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="41f2d-114">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="41f2d-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="41f2d-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="41f2d-115">scheduledInstallTime</span></span>|<span data-ttu-id="41f2d-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="41f2d-116">TimeOfDay</span></span>|<span data-ttu-id="41f2d-117">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="41f2d-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="41f2d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41f2d-118">Relationships</span></span>
<span data-ttu-id="41f2d-119">なし</span><span class="sxs-lookup"><span data-stu-id="41f2d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41f2d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41f2d-120">JSON Representation</span></span>
<span data-ttu-id="41f2d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41f2d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



