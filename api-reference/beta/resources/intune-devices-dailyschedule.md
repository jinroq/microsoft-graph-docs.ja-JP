---
title: 社員のリソースの種類
description: 定期的なデバイスの管理スクリプトの実行スケジュールを日単位です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c4cbe48aecf3fe561becad4734f7de0b5f68ffa0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415251"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="53f7e-103">社員のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="53f7e-103">dailySchedule resource type</span></span>

> <span data-ttu-id="53f7e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="53f7e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53f7e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53f7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53f7e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53f7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53f7e-107">定期的なデバイスの管理スクリプトの実行スケジュールを日単位です。</span><span class="sxs-lookup"><span data-stu-id="53f7e-107">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="53f7e-108">[RunSchedule](../resources/intune-devices-runschedule.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="53f7e-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="53f7e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53f7e-109">Properties</span></span>
|<span data-ttu-id="53f7e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53f7e-110">Property</span></span>|<span data-ttu-id="53f7e-111">型</span><span class="sxs-lookup"><span data-stu-id="53f7e-111">Type</span></span>|<span data-ttu-id="53f7e-112">説明</span><span class="sxs-lookup"><span data-stu-id="53f7e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53f7e-113">interval</span><span class="sxs-lookup"><span data-stu-id="53f7e-113">interval</span></span>|<span data-ttu-id="53f7e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="53f7e-114">Int32</span></span>|<span data-ttu-id="53f7e-115">間隔の日数</span><span class="sxs-lookup"><span data-stu-id="53f7e-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="53f7e-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="53f7e-116">Relationships</span></span>
<span data-ttu-id="53f7e-117">なし</span><span class="sxs-lookup"><span data-stu-id="53f7e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53f7e-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="53f7e-118">JSON Representation</span></span>
<span data-ttu-id="53f7e-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="53f7e-119">Here is a JSON representation of the resource.</span></span>
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




