---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd3a1aafe751bd5db334387cc3872c68e6de6637
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797922"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="a7288-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a7288-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="a7288-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7288-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7288-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7288-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7288-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a7288-106">Not yet documented</span></span>


<span data-ttu-id="a7288-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a7288-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a7288-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7288-108">Properties</span></span>
|<span data-ttu-id="a7288-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7288-109">Property</span></span>|<span data-ttu-id="a7288-110">型</span><span class="sxs-lookup"><span data-stu-id="a7288-110">Type</span></span>|<span data-ttu-id="a7288-111">説明</span><span class="sxs-lookup"><span data-stu-id="a7288-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7288-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="a7288-112">scheduledInstallDay</span></span>|[<span data-ttu-id="a7288-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="a7288-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="a7288-114">スケジュールされたインストール日 (週単位)。</span><span class="sxs-lookup"><span data-stu-id="a7288-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="a7288-115">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="a7288-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a7288-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="a7288-116">scheduledInstallTime</span></span>|<span data-ttu-id="a7288-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a7288-117">TimeOfDay</span></span>|<span data-ttu-id="a7288-118">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="a7288-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7288-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a7288-119">Relationships</span></span>
<span data-ttu-id="a7288-120">なし</span><span class="sxs-lookup"><span data-stu-id="a7288-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7288-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7288-121">JSON Representation</span></span>
<span data-ttu-id="a7288-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7288-122">Here is a JSON representation of the resource.</span></span>
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





