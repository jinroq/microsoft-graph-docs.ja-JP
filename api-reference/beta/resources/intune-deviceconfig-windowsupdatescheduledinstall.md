---
title: windowsUpdateScheduledInstall リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 93866da8e1dff5b53303dfd6cbd358fc0280ee30
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337686"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="7d4c0-103">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7d4c0-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="7d4c0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d4c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d4c0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d4c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d4c0-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7d4c0-106">Not yet documented</span></span>


<span data-ttu-id="7d4c0-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7d4c0-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d4c0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d4c0-108">Properties</span></span>
|<span data-ttu-id="7d4c0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d4c0-109">Property</span></span>|<span data-ttu-id="7d4c0-110">型</span><span class="sxs-lookup"><span data-stu-id="7d4c0-110">Type</span></span>|<span data-ttu-id="7d4c0-111">説明</span><span class="sxs-lookup"><span data-stu-id="7d4c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d4c0-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="7d4c0-112">scheduledInstallDay</span></span>|[<span data-ttu-id="7d4c0-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="7d4c0-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="7d4c0-114">スケジュールされたインストール日 (週単位)。</span><span class="sxs-lookup"><span data-stu-id="7d4c0-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="7d4c0-115">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`noScheduledScan` です。</span><span class="sxs-lookup"><span data-stu-id="7d4c0-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="7d4c0-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="7d4c0-116">scheduledInstallTime</span></span>|<span data-ttu-id="7d4c0-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7d4c0-117">TimeOfDay</span></span>|<span data-ttu-id="7d4c0-118">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="7d4c0-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d4c0-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7d4c0-119">Relationships</span></span>
<span data-ttu-id="7d4c0-120">なし</span><span class="sxs-lookup"><span data-stu-id="7d4c0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d4c0-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d4c0-121">JSON Representation</span></span>
<span data-ttu-id="7d4c0-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7d4c0-122">Here is a JSON representation of the resource.</span></span>
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



