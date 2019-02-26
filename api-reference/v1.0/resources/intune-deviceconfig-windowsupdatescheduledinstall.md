---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b8f0eea6eb81f9e06243101bb2433fbcafaecae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264317"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="67d83-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67d83-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="67d83-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67d83-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67d83-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="67d83-105">Not yet documented</span></span>


<span data-ttu-id="67d83-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="67d83-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="67d83-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67d83-107">Properties</span></span>
|<span data-ttu-id="67d83-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67d83-108">Property</span></span>|<span data-ttu-id="67d83-109">型</span><span class="sxs-lookup"><span data-stu-id="67d83-109">Type</span></span>|<span data-ttu-id="67d83-110">説明</span><span class="sxs-lookup"><span data-stu-id="67d83-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67d83-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="67d83-111">scheduledInstallDay</span></span>|[<span data-ttu-id="67d83-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="67d83-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="67d83-113">スケジュールされたインストール日 (週単位)。</span><span class="sxs-lookup"><span data-stu-id="67d83-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="67d83-114">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="67d83-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="67d83-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="67d83-115">scheduledInstallTime</span></span>|<span data-ttu-id="67d83-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="67d83-116">TimeOfDay</span></span>|<span data-ttu-id="67d83-117">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="67d83-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="67d83-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="67d83-118">Relationships</span></span>
<span data-ttu-id="67d83-119">なし</span><span class="sxs-lookup"><span data-stu-id="67d83-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67d83-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67d83-120">JSON Representation</span></span>
<span data-ttu-id="67d83-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="67d83-121">Here is a JSON representation of the resource.</span></span>
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



