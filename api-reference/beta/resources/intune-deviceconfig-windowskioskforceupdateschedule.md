---
title: Windowskioskforceて Chedule リソースの種類
description: Windows 10 では、キオスクデバイスの更新スケジュールを強制します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e308d0ea6fc8015281515ce0d60d859ed326c16
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370892"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="a5af4-103">Windowskioskforceて Chedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a5af4-103">windowsKioskForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="a5af4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5af4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5af4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5af4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5af4-106">Windows 10 では、キオスクデバイスの更新スケジュールを強制します。</span><span class="sxs-lookup"><span data-stu-id="a5af4-106">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="a5af4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5af4-107">Properties</span></span>
|<span data-ttu-id="a5af4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5af4-108">Property</span></span>|<span data-ttu-id="a5af4-109">型</span><span class="sxs-lookup"><span data-stu-id="a5af4-109">Type</span></span>|<span data-ttu-id="a5af4-110">説明</span><span class="sxs-lookup"><span data-stu-id="a5af4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5af4-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a5af4-111">startDateTime</span></span>|<span data-ttu-id="a5af4-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5af4-112">DateTimeOffset</span></span>|<span data-ttu-id="a5af4-113">強制再起動の開始時刻。</span><span class="sxs-lookup"><span data-stu-id="a5af4-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="a5af4-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="a5af4-114">recurrence</span></span>|[<span data-ttu-id="a5af4-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5af4-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="a5af4-116">定期的なスケジュール。</span><span class="sxs-lookup"><span data-stu-id="a5af4-116">Recurrence schedule.</span></span> <span data-ttu-id="a5af4-117">使用可能な値は、`none`、`daily`、`weekly`、`monthly` です。</span><span class="sxs-lookup"><span data-stu-id="a5af4-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="a5af4-118">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="a5af4-118">dayofWeek</span></span>|[<span data-ttu-id="a5af4-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="a5af4-119">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="a5af4-120">曜日。</span><span class="sxs-lookup"><span data-stu-id="a5af4-120">Day of week.</span></span> <span data-ttu-id="a5af4-121">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="a5af4-121">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a5af4-122">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="a5af4-122">dayofMonth</span></span>|<span data-ttu-id="a5af4-123">Int32</span><span class="sxs-lookup"><span data-stu-id="a5af4-123">Int32</span></span>|<span data-ttu-id="a5af4-124">月の日付。</span><span class="sxs-lookup"><span data-stu-id="a5af4-124">Day of month.</span></span> <span data-ttu-id="a5af4-125">有効な値は1から31までです</span><span class="sxs-lookup"><span data-stu-id="a5af4-125">Valid values 1 to 31</span></span>|
|<span data-ttu-id="a5af4-126">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a5af4-126">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="a5af4-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5af4-127">Boolean</span></span>|<span data-ttu-id="a5af4-128">True の場合は、StartDateTime が過去の場合はすぐにタスクを実行します。それ以外の場合は、次の定期的なパターンが実行されます。</span><span class="sxs-lookup"><span data-stu-id="a5af4-128">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5af4-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a5af4-129">Relationships</span></span>
<span data-ttu-id="a5af4-130">なし</span><span class="sxs-lookup"><span data-stu-id="a5af4-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5af4-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a5af4-131">JSON Representation</span></span>
<span data-ttu-id="a5af4-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a5af4-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```



