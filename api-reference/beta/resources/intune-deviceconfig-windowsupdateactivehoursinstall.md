---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0c40fc7ade30a73212d1917294671fdb5423483
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978767"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="0d972-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d972-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="0d972-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d972-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d972-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0d972-106">Not yet documented</span></span>


<span data-ttu-id="0d972-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0d972-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d972-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d972-108">Properties</span></span>
|<span data-ttu-id="0d972-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d972-109">Property</span></span>|<span data-ttu-id="0d972-110">型</span><span class="sxs-lookup"><span data-stu-id="0d972-110">Type</span></span>|<span data-ttu-id="0d972-111">説明</span><span class="sxs-lookup"><span data-stu-id="0d972-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d972-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="0d972-112">activeHoursStart</span></span>|<span data-ttu-id="0d972-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0d972-113">TimeOfDay</span></span>|<span data-ttu-id="0d972-114">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="0d972-114">Active Hours Start</span></span>|
|<span data-ttu-id="0d972-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="0d972-115">activeHoursEnd</span></span>|<span data-ttu-id="0d972-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0d972-116">TimeOfDay</span></span>|<span data-ttu-id="0d972-117">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="0d972-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d972-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0d972-118">Relationships</span></span>
<span data-ttu-id="0d972-119">なし</span><span class="sxs-lookup"><span data-stu-id="0d972-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d972-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d972-120">JSON Representation</span></span>
<span data-ttu-id="0d972-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0d972-121">Here is a JSON representation of the resource.</span></span>
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





