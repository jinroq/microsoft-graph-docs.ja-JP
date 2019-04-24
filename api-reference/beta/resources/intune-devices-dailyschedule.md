---
title: dailySchedule リソースの種類
description: 定期的なデバイス管理スクリプトの日単位の実行スケジュール。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd2b226255f433b4f82d042b6389830143515033
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454140"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="be908-103">dailySchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be908-103">dailySchedule resource type</span></span>

> <span data-ttu-id="be908-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be908-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be908-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="be908-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be908-106">定期的なデバイス管理スクリプトの日単位の実行スケジュール。</span><span class="sxs-lookup"><span data-stu-id="be908-106">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="be908-107">[runschedule](../resources/intune-devices-runschedule.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="be908-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="be908-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be908-108">Properties</span></span>
|<span data-ttu-id="be908-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be908-109">Property</span></span>|<span data-ttu-id="be908-110">型</span><span class="sxs-lookup"><span data-stu-id="be908-110">Type</span></span>|<span data-ttu-id="be908-111">説明</span><span class="sxs-lookup"><span data-stu-id="be908-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be908-112">interval</span><span class="sxs-lookup"><span data-stu-id="be908-112">interval</span></span>|<span data-ttu-id="be908-113">Int32</span><span class="sxs-lookup"><span data-stu-id="be908-113">Int32</span></span>|<span data-ttu-id="be908-114">日数で指定した間隔</span><span class="sxs-lookup"><span data-stu-id="be908-114">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="be908-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="be908-115">Relationships</span></span>
<span data-ttu-id="be908-116">なし</span><span class="sxs-lookup"><span data-stu-id="be908-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be908-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be908-117">JSON Representation</span></span>
<span data-ttu-id="be908-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be908-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```





