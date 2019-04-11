---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f65d986fa59a3087a5fe1578eec626a27a4154b0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792721"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="92060-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92060-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="92060-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92060-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92060-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92060-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92060-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="92060-106">Not yet documented</span></span>


<span data-ttu-id="92060-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="92060-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92060-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92060-108">Properties</span></span>
|<span data-ttu-id="92060-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92060-109">Property</span></span>|<span data-ttu-id="92060-110">型</span><span class="sxs-lookup"><span data-stu-id="92060-110">Type</span></span>|<span data-ttu-id="92060-111">説明</span><span class="sxs-lookup"><span data-stu-id="92060-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92060-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="92060-112">activeHoursStart</span></span>|<span data-ttu-id="92060-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="92060-113">TimeOfDay</span></span>|<span data-ttu-id="92060-114">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="92060-114">Active Hours Start</span></span>|
|<span data-ttu-id="92060-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="92060-115">activeHoursEnd</span></span>|<span data-ttu-id="92060-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="92060-116">TimeOfDay</span></span>|<span data-ttu-id="92060-117">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="92060-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="92060-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92060-118">Relationships</span></span>
<span data-ttu-id="92060-119">なし</span><span class="sxs-lookup"><span data-stu-id="92060-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92060-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92060-120">JSON Representation</span></span>
<span data-ttu-id="92060-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92060-121">Here is a JSON representation of the resource.</span></span>
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





