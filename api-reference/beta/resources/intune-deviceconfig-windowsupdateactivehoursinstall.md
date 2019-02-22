---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9deab255749e70cfd165f28c27c09182b298e00a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144094"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="95271-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95271-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="95271-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95271-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95271-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95271-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95271-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="95271-106">Not yet documented</span></span>


<span data-ttu-id="95271-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="95271-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95271-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95271-108">Properties</span></span>
|<span data-ttu-id="95271-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95271-109">Property</span></span>|<span data-ttu-id="95271-110">型</span><span class="sxs-lookup"><span data-stu-id="95271-110">Type</span></span>|<span data-ttu-id="95271-111">説明</span><span class="sxs-lookup"><span data-stu-id="95271-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95271-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="95271-112">activeHoursStart</span></span>|<span data-ttu-id="95271-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="95271-113">TimeOfDay</span></span>|<span data-ttu-id="95271-114">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="95271-114">Active Hours Start</span></span>|
|<span data-ttu-id="95271-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="95271-115">activeHoursEnd</span></span>|<span data-ttu-id="95271-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="95271-116">TimeOfDay</span></span>|<span data-ttu-id="95271-117">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="95271-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="95271-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95271-118">Relationships</span></span>
<span data-ttu-id="95271-119">なし</span><span class="sxs-lookup"><span data-stu-id="95271-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95271-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95271-120">JSON Representation</span></span>
<span data-ttu-id="95271-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95271-121">Here is a JSON representation of the resource.</span></span>
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




