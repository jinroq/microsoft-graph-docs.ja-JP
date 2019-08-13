---
title: dailySchedule リソースの種類
description: 定期的なデバイス管理スクリプトの日単位の実行スケジュール。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4f7714614f0f3d73067b60e6ed50c090cec02d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370257"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="d7986-103">dailySchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7986-103">dailySchedule resource type</span></span>

> <span data-ttu-id="d7986-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7986-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7986-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7986-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7986-106">定期的なデバイス管理スクリプトの日単位の実行スケジュール。</span><span class="sxs-lookup"><span data-stu-id="d7986-106">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="d7986-107">[Runschedule](../resources/intune-devices-runschedule.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d7986-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7986-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7986-108">Properties</span></span>
|<span data-ttu-id="d7986-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7986-109">Property</span></span>|<span data-ttu-id="d7986-110">型</span><span class="sxs-lookup"><span data-stu-id="d7986-110">Type</span></span>|<span data-ttu-id="d7986-111">説明</span><span class="sxs-lookup"><span data-stu-id="d7986-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7986-112">interval</span><span class="sxs-lookup"><span data-stu-id="d7986-112">interval</span></span>|<span data-ttu-id="d7986-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d7986-113">Int32</span></span>|<span data-ttu-id="d7986-114">日数で指定した間隔</span><span class="sxs-lookup"><span data-stu-id="d7986-114">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7986-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7986-115">Relationships</span></span>
<span data-ttu-id="d7986-116">なし</span><span class="sxs-lookup"><span data-stu-id="d7986-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7986-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7986-117">JSON Representation</span></span>
<span data-ttu-id="d7986-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d7986-118">Here is a JSON representation of the resource.</span></span>
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



