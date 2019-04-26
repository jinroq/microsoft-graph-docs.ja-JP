---
title: windowsUpdateActiveHoursInstall リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f65d986fa59a3087a5fe1578eec626a27a4154b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555193"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="76a3c-103">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76a3c-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="76a3c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76a3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76a3c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76a3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76a3c-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="76a3c-106">Not yet documented</span></span>


<span data-ttu-id="76a3c-107">[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="76a3c-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76a3c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76a3c-108">Properties</span></span>
|<span data-ttu-id="76a3c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76a3c-109">Property</span></span>|<span data-ttu-id="76a3c-110">型</span><span class="sxs-lookup"><span data-stu-id="76a3c-110">Type</span></span>|<span data-ttu-id="76a3c-111">説明</span><span class="sxs-lookup"><span data-stu-id="76a3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76a3c-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="76a3c-112">activeHoursStart</span></span>|<span data-ttu-id="76a3c-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="76a3c-113">TimeOfDay</span></span>|<span data-ttu-id="76a3c-114">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="76a3c-114">Active Hours Start</span></span>|
|<span data-ttu-id="76a3c-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="76a3c-115">activeHoursEnd</span></span>|<span data-ttu-id="76a3c-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="76a3c-116">TimeOfDay</span></span>|<span data-ttu-id="76a3c-117">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="76a3c-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="76a3c-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="76a3c-118">Relationships</span></span>
<span data-ttu-id="76a3c-119">なし</span><span class="sxs-lookup"><span data-stu-id="76a3c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76a3c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76a3c-120">JSON Representation</span></span>
<span data-ttu-id="76a3c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76a3c-121">Here is a JSON representation of the resource.</span></span>
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





