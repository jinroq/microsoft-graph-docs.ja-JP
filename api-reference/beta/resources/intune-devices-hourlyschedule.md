---
title: 時間のスケジュールリソースの種類
description: 定期的なデバイス管理スクリプトの時間単位の実行スケジュール。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 78afa43149f35645f2167a8f593124f01ea11c12
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369900"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="96215-103">時間のスケジュールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="96215-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="96215-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96215-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96215-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96215-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96215-106">定期的なデバイス管理スクリプトの時間単位の実行スケジュール。</span><span class="sxs-lookup"><span data-stu-id="96215-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="96215-107">[Runschedule](../resources/intune-devices-runschedule.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="96215-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96215-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96215-108">Properties</span></span>
|<span data-ttu-id="96215-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96215-109">Property</span></span>|<span data-ttu-id="96215-110">型</span><span class="sxs-lookup"><span data-stu-id="96215-110">Type</span></span>|<span data-ttu-id="96215-111">説明</span><span class="sxs-lookup"><span data-stu-id="96215-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96215-112">interval</span><span class="sxs-lookup"><span data-stu-id="96215-112">interval</span></span>|<span data-ttu-id="96215-113">Int32</span><span class="sxs-lookup"><span data-stu-id="96215-113">Int32</span></span>|<span data-ttu-id="96215-114">間隔 (時間単位)</span><span class="sxs-lookup"><span data-stu-id="96215-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="96215-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96215-115">Relationships</span></span>
<span data-ttu-id="96215-116">なし</span><span class="sxs-lookup"><span data-stu-id="96215-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96215-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96215-117">JSON Representation</span></span>
<span data-ttu-id="96215-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96215-118">Here is a JSON representation of the resource.</span></span>
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



