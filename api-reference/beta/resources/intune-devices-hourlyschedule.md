---
title: 時間のスケジュールリソースの種類
description: 定期的なデバイス管理スクリプトの時間単位の実行スケジュール。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f86591326f2b4df8e887c657c05ad3d5021946e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522182"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="9abcf-103">時間のスケジュールリソースの種類</span><span class="sxs-lookup"><span data-stu-id="9abcf-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="9abcf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9abcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9abcf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9abcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9abcf-106">定期的なデバイス管理スクリプトの時間単位の実行スケジュール。</span><span class="sxs-lookup"><span data-stu-id="9abcf-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="9abcf-107">[runschedule](../resources/intune-devices-runschedule.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="9abcf-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9abcf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9abcf-108">Properties</span></span>
|<span data-ttu-id="9abcf-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9abcf-109">Property</span></span>|<span data-ttu-id="9abcf-110">型</span><span class="sxs-lookup"><span data-stu-id="9abcf-110">Type</span></span>|<span data-ttu-id="9abcf-111">説明</span><span class="sxs-lookup"><span data-stu-id="9abcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9abcf-112">interval</span><span class="sxs-lookup"><span data-stu-id="9abcf-112">interval</span></span>|<span data-ttu-id="9abcf-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9abcf-113">Int32</span></span>|<span data-ttu-id="9abcf-114">間隔 (時間単位)</span><span class="sxs-lookup"><span data-stu-id="9abcf-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="9abcf-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9abcf-115">Relationships</span></span>
<span data-ttu-id="9abcf-116">なし</span><span class="sxs-lookup"><span data-stu-id="9abcf-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9abcf-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9abcf-117">JSON Representation</span></span>
<span data-ttu-id="9abcf-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9abcf-118">Here is a JSON representation of the resource.</span></span>
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





