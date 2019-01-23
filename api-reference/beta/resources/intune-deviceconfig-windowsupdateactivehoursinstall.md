---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 28f40501123f465d8fcbfa05c3febb8ffab6f27a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409469"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="6dfaa-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6dfaa-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="6dfaa-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6dfaa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6dfaa-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dfaa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6dfaa-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dfaa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dfaa-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6dfaa-107">Not yet documented</span></span>


<span data-ttu-id="6dfaa-108">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6dfaa-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6dfaa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dfaa-109">Properties</span></span>
|<span data-ttu-id="6dfaa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6dfaa-110">Property</span></span>|<span data-ttu-id="6dfaa-111">型</span><span class="sxs-lookup"><span data-stu-id="6dfaa-111">Type</span></span>|<span data-ttu-id="6dfaa-112">説明</span><span class="sxs-lookup"><span data-stu-id="6dfaa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dfaa-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="6dfaa-113">activeHoursStart</span></span>|<span data-ttu-id="6dfaa-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6dfaa-114">TimeOfDay</span></span>|<span data-ttu-id="6dfaa-115">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="6dfaa-115">Active Hours Start</span></span>|
|<span data-ttu-id="6dfaa-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="6dfaa-116">activeHoursEnd</span></span>|<span data-ttu-id="6dfaa-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6dfaa-117">TimeOfDay</span></span>|<span data-ttu-id="6dfaa-118">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="6dfaa-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dfaa-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6dfaa-119">Relationships</span></span>
<span data-ttu-id="6dfaa-120">なし</span><span class="sxs-lookup"><span data-stu-id="6dfaa-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6dfaa-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6dfaa-121">JSON Representation</span></span>
<span data-ttu-id="6dfaa-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6dfaa-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```




