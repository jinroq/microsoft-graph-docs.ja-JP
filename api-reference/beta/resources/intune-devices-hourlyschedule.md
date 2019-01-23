---
title: hourlySchedule リソースの種類
description: 定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf62c11da0932f5f10b6cc7a76ccecfd1e74ee92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396827"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="a89a4-103">hourlySchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a89a4-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="a89a4-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a89a4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a89a4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a89a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a89a4-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a89a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a89a4-107">定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。</span><span class="sxs-lookup"><span data-stu-id="a89a4-107">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="a89a4-108">[RunSchedule](../resources/intune-devices-runschedule.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a89a4-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a89a4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a89a4-109">Properties</span></span>
|<span data-ttu-id="a89a4-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a89a4-110">Property</span></span>|<span data-ttu-id="a89a4-111">型</span><span class="sxs-lookup"><span data-stu-id="a89a4-111">Type</span></span>|<span data-ttu-id="a89a4-112">説明</span><span class="sxs-lookup"><span data-stu-id="a89a4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a89a4-113">interval</span><span class="sxs-lookup"><span data-stu-id="a89a4-113">interval</span></span>|<span data-ttu-id="a89a4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a89a4-114">Int32</span></span>|<span data-ttu-id="a89a4-115">間隔 (時間数単位)</span><span class="sxs-lookup"><span data-stu-id="a89a4-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="a89a4-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a89a4-116">Relationships</span></span>
<span data-ttu-id="a89a4-117">なし</span><span class="sxs-lookup"><span data-stu-id="a89a4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a89a4-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a89a4-118">JSON Representation</span></span>
<span data-ttu-id="a89a4-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a89a4-119">Here is a JSON representation of the resource.</span></span>
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




