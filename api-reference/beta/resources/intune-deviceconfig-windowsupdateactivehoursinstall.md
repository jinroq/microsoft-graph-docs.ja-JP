---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49238831005d579baba2dd55e431f1ac684e67d3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943656"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="97048-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97048-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="97048-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97048-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97048-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97048-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97048-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97048-106">Not yet documented</span></span>


<span data-ttu-id="97048-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="97048-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97048-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97048-108">Properties</span></span>
|<span data-ttu-id="97048-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97048-109">Property</span></span>|<span data-ttu-id="97048-110">型</span><span class="sxs-lookup"><span data-stu-id="97048-110">Type</span></span>|<span data-ttu-id="97048-111">説明</span><span class="sxs-lookup"><span data-stu-id="97048-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97048-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="97048-112">activeHoursStart</span></span>|<span data-ttu-id="97048-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="97048-113">TimeOfDay</span></span>|<span data-ttu-id="97048-114">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="97048-114">Active Hours Start</span></span>|
|<span data-ttu-id="97048-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="97048-115">activeHoursEnd</span></span>|<span data-ttu-id="97048-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="97048-116">TimeOfDay</span></span>|<span data-ttu-id="97048-117">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="97048-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="97048-118">関係</span><span class="sxs-lookup"><span data-stu-id="97048-118">Relationships</span></span>
<span data-ttu-id="97048-119">なし</span><span class="sxs-lookup"><span data-stu-id="97048-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97048-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97048-120">JSON Representation</span></span>
<span data-ttu-id="97048-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97048-121">Here is a JSON representation of the resource.</span></span>
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




