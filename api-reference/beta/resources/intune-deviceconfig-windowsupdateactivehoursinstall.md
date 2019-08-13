---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5d5c517e4b146c94b931caf09f354ed5a348080
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369571"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="16156-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="16156-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="16156-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16156-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16156-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="16156-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16156-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="16156-106">Not yet documented</span></span>


<span data-ttu-id="16156-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="16156-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16156-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16156-108">Properties</span></span>
|<span data-ttu-id="16156-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16156-109">Property</span></span>|<span data-ttu-id="16156-110">型</span><span class="sxs-lookup"><span data-stu-id="16156-110">Type</span></span>|<span data-ttu-id="16156-111">説明</span><span class="sxs-lookup"><span data-stu-id="16156-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16156-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="16156-112">activeHoursStart</span></span>|<span data-ttu-id="16156-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="16156-113">TimeOfDay</span></span>|<span data-ttu-id="16156-114">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="16156-114">Active Hours Start</span></span>|
|<span data-ttu-id="16156-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="16156-115">activeHoursEnd</span></span>|<span data-ttu-id="16156-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="16156-116">TimeOfDay</span></span>|<span data-ttu-id="16156-117">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="16156-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="16156-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="16156-118">Relationships</span></span>
<span data-ttu-id="16156-119">なし</span><span class="sxs-lookup"><span data-stu-id="16156-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16156-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16156-120">JSON Representation</span></span>
<span data-ttu-id="16156-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="16156-121">Here is a JSON representation of the resource.</span></span>
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



