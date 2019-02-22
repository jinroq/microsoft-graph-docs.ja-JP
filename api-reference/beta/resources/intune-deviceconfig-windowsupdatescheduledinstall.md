---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de36e3777518cf7c79a7590c19147d014e2aee7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172507"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="894e8-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="894e8-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="894e8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="894e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="894e8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="894e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="894e8-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="894e8-106">Not yet documented</span></span>


<span data-ttu-id="894e8-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="894e8-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="894e8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="894e8-108">Properties</span></span>
|<span data-ttu-id="894e8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="894e8-109">Property</span></span>|<span data-ttu-id="894e8-110">型</span><span class="sxs-lookup"><span data-stu-id="894e8-110">Type</span></span>|<span data-ttu-id="894e8-111">説明</span><span class="sxs-lookup"><span data-stu-id="894e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="894e8-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="894e8-112">scheduledInstallDay</span></span>|[<span data-ttu-id="894e8-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="894e8-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="894e8-114">スケジュールされたインストール日 (週単位)。</span><span class="sxs-lookup"><span data-stu-id="894e8-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="894e8-115">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="894e8-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="894e8-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="894e8-116">scheduledInstallTime</span></span>|<span data-ttu-id="894e8-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="894e8-117">TimeOfDay</span></span>|<span data-ttu-id="894e8-118">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="894e8-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="894e8-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="894e8-119">Relationships</span></span>
<span data-ttu-id="894e8-120">なし</span><span class="sxs-lookup"><span data-stu-id="894e8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="894e8-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="894e8-121">JSON Representation</span></span>
<span data-ttu-id="894e8-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="894e8-122">Here is a JSON representation of the resource.</span></span>
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




