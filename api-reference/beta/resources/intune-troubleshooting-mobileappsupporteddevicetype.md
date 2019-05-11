---
title: mobileAppSupportedDeviceType リソースの種類
description: デバイスのプロパティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 001e80621709bdb2dcdb9b5cf8e17753ee3458b3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939118"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="6b3f2-103">mobileAppSupportedDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b3f2-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="6b3f2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b3f2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b3f2-106">デバイスのプロパティ</span><span class="sxs-lookup"><span data-stu-id="6b3f2-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="6b3f2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b3f2-107">Properties</span></span>
|<span data-ttu-id="6b3f2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b3f2-108">Property</span></span>|<span data-ttu-id="6b3f2-109">種類</span><span class="sxs-lookup"><span data-stu-id="6b3f2-109">Type</span></span>|<span data-ttu-id="6b3f2-110">説明</span><span class="sxs-lookup"><span data-stu-id="6b3f2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b3f2-111">type</span><span class="sxs-lookup"><span data-stu-id="6b3f2-111">type</span></span>|[<span data-ttu-id="6b3f2-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="6b3f2-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="6b3f2-113">デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-113">Device type.</span></span> <span data-ttu-id="6b3f2-114">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6b3f2-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="6b3f2-115">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="6b3f2-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="6b3f2-116">String</span><span class="sxs-lookup"><span data-stu-id="6b3f2-116">String</span></span>|<span data-ttu-id="6b3f2-117">最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="6b3f2-117">Minimum OS version</span></span>|
|<span data-ttu-id="6b3f2-118">最大化 Umoper/Systemversion</span><span class="sxs-lookup"><span data-stu-id="6b3f2-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="6b3f2-119">String</span><span class="sxs-lookup"><span data-stu-id="6b3f2-119">String</span></span>|<span data-ttu-id="6b3f2-120">最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="6b3f2-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b3f2-121">関係</span><span class="sxs-lookup"><span data-stu-id="6b3f2-121">Relationships</span></span>
<span data-ttu-id="6b3f2-122">なし</span><span class="sxs-lookup"><span data-stu-id="6b3f2-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b3f2-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b3f2-123">JSON Representation</span></span>
<span data-ttu-id="6b3f2-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6b3f2-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```




