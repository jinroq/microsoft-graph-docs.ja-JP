---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3635441f015d49ffb402f5314896e9e68b15e8e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030927"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="86534-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86534-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="86534-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86534-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86534-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86534-105">Not yet documented</span></span>


<span data-ttu-id="86534-106">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="86534-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="86534-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86534-107">Properties</span></span>
|<span data-ttu-id="86534-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86534-108">Property</span></span>|<span data-ttu-id="86534-109">型</span><span class="sxs-lookup"><span data-stu-id="86534-109">Type</span></span>|<span data-ttu-id="86534-110">説明</span><span class="sxs-lookup"><span data-stu-id="86534-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86534-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="86534-111">activeHoursStart</span></span>|<span data-ttu-id="86534-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="86534-112">TimeOfDay</span></span>|<span data-ttu-id="86534-113">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="86534-113">Active Hours Start</span></span>|
|<span data-ttu-id="86534-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="86534-114">activeHoursEnd</span></span>|<span data-ttu-id="86534-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="86534-115">TimeOfDay</span></span>|<span data-ttu-id="86534-116">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="86534-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="86534-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86534-117">Relationships</span></span>
<span data-ttu-id="86534-118">なし</span><span class="sxs-lookup"><span data-stu-id="86534-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86534-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86534-119">JSON Representation</span></span>
<span data-ttu-id="86534-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86534-120">Here is a JSON representation of the resource.</span></span>
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



