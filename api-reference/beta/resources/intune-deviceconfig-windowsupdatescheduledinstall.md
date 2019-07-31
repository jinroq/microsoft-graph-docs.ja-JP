---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5819770fb09c36240761a5b54deee4bbe7c638a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000117"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="ac7b9-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac7b9-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="ac7b9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac7b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac7b9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ac7b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac7b9-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ac7b9-106">Not yet documented</span></span>


<span data-ttu-id="ac7b9-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ac7b9-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ac7b9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac7b9-108">Properties</span></span>
|<span data-ttu-id="ac7b9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac7b9-109">Property</span></span>|<span data-ttu-id="ac7b9-110">型</span><span class="sxs-lookup"><span data-stu-id="ac7b9-110">Type</span></span>|<span data-ttu-id="ac7b9-111">説明</span><span class="sxs-lookup"><span data-stu-id="ac7b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac7b9-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="ac7b9-112">scheduledInstallDay</span></span>|[<span data-ttu-id="ac7b9-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="ac7b9-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="ac7b9-114">スケジュールされたインストール日 (週単位)。</span><span class="sxs-lookup"><span data-stu-id="ac7b9-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="ac7b9-115">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="ac7b9-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="ac7b9-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="ac7b9-116">scheduledInstallTime</span></span>|<span data-ttu-id="ac7b9-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ac7b9-117">TimeOfDay</span></span>|<span data-ttu-id="ac7b9-118">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="ac7b9-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac7b9-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac7b9-119">Relationships</span></span>
<span data-ttu-id="ac7b9-120">なし</span><span class="sxs-lookup"><span data-stu-id="ac7b9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac7b9-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac7b9-121">JSON Representation</span></span>
<span data-ttu-id="ac7b9-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac7b9-122">Here is a JSON representation of the resource.</span></span>
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





