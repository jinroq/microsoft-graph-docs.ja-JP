---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ee91ed2541c02adbb7a130f0a9de869d86044632
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395630"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="49ab2-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49ab2-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="49ab2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="49ab2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="49ab2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49ab2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49ab2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49ab2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49ab2-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49ab2-107">Not yet documented</span></span>


<span data-ttu-id="49ab2-108">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="49ab2-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49ab2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49ab2-109">Properties</span></span>
|<span data-ttu-id="49ab2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49ab2-110">Property</span></span>|<span data-ttu-id="49ab2-111">型</span><span class="sxs-lookup"><span data-stu-id="49ab2-111">Type</span></span>|<span data-ttu-id="49ab2-112">説明</span><span class="sxs-lookup"><span data-stu-id="49ab2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49ab2-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="49ab2-113">scheduledInstallDay</span></span>|[<span data-ttu-id="49ab2-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="49ab2-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="49ab2-115">スケジュールされたインストールの週の曜日です。</span><span class="sxs-lookup"><span data-stu-id="49ab2-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="49ab2-116">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="49ab2-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="49ab2-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="49ab2-117">scheduledInstallTime</span></span>|<span data-ttu-id="49ab2-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="49ab2-118">TimeOfDay</span></span>|<span data-ttu-id="49ab2-119">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="49ab2-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="49ab2-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49ab2-120">Relationships</span></span>
<span data-ttu-id="49ab2-121">なし</span><span class="sxs-lookup"><span data-stu-id="49ab2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49ab2-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49ab2-122">JSON Representation</span></span>
<span data-ttu-id="49ab2-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49ab2-123">Here is a JSON representation of the resource.</span></span>
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




