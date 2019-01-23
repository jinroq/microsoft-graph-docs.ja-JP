---
title: windows10AppsForceUpdateSchedule リソースの種類
description: アプリケーションの Windows 10 強制更新のスケジュール
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e0bd9b0963f8547b03243aa7ef791a351dc2b08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418835"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="a286d-103">windows10AppsForceUpdateSchedule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a286d-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="a286d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a286d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a286d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a286d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a286d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a286d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a286d-107">アプリケーションの Windows 10 強制更新のスケジュール</span><span class="sxs-lookup"><span data-stu-id="a286d-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="a286d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a286d-108">Properties</span></span>
|<span data-ttu-id="a286d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a286d-109">Property</span></span>|<span data-ttu-id="a286d-110">型</span><span class="sxs-lookup"><span data-stu-id="a286d-110">Type</span></span>|<span data-ttu-id="a286d-111">説明</span><span class="sxs-lookup"><span data-stu-id="a286d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a286d-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a286d-112">startDateTime</span></span>|<span data-ttu-id="a286d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a286d-113">DateTimeOffset</span></span>|<span data-ttu-id="a286d-114">力の開始時刻を再起動します。</span><span class="sxs-lookup"><span data-stu-id="a286d-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="a286d-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="a286d-115">recurrence</span></span>|[<span data-ttu-id="a286d-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="a286d-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="a286d-117">定期的なスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="a286d-117">Recurrence schedule.</span></span> <span data-ttu-id="a286d-118">可能な値は、`none`、`daily`、`weekly`、`monthly` です。</span><span class="sxs-lookup"><span data-stu-id="a286d-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="a286d-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="a286d-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="a286d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a286d-120">Boolean</span></span>|<span data-ttu-id="a286d-121">True の場合、タスクはすぐに実行させるまでは、他の次の反復の実行の場合です。</span><span class="sxs-lookup"><span data-stu-id="a286d-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a286d-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a286d-122">Relationships</span></span>
<span data-ttu-id="a286d-123">なし</span><span class="sxs-lookup"><span data-stu-id="a286d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a286d-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a286d-124">JSON Representation</span></span>
<span data-ttu-id="a286d-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a286d-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```




