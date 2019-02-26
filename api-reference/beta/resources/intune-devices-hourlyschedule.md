---
title: 時間のスケジュールリソースの種類
description: 定期的なデバイス管理スクリプトの時間単位の実行スケジュール。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb3eacf4e17ed1137ce78d21112c394a45423c6b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173417"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="1b5ce-103">時間のスケジュールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="1b5ce-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="1b5ce-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b5ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b5ce-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1b5ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b5ce-106">定期的なデバイス管理スクリプトの時間単位の実行スケジュール。</span><span class="sxs-lookup"><span data-stu-id="1b5ce-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="1b5ce-107">[runschedule](../resources/intune-devices-runschedule.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1b5ce-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1b5ce-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b5ce-108">Properties</span></span>
|<span data-ttu-id="1b5ce-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b5ce-109">Property</span></span>|<span data-ttu-id="1b5ce-110">型</span><span class="sxs-lookup"><span data-stu-id="1b5ce-110">Type</span></span>|<span data-ttu-id="1b5ce-111">説明</span><span class="sxs-lookup"><span data-stu-id="1b5ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b5ce-112">interval</span><span class="sxs-lookup"><span data-stu-id="1b5ce-112">interval</span></span>|<span data-ttu-id="1b5ce-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1b5ce-113">Int32</span></span>|<span data-ttu-id="1b5ce-114">間隔 (時間単位)</span><span class="sxs-lookup"><span data-stu-id="1b5ce-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b5ce-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1b5ce-115">Relationships</span></span>
<span data-ttu-id="1b5ce-116">なし</span><span class="sxs-lookup"><span data-stu-id="1b5ce-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b5ce-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1b5ce-117">JSON Representation</span></span>
<span data-ttu-id="1b5ce-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1b5ce-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```




