---
title: mobileAppSupportedDeviceType リソースの種類
description: デバイスのプロパティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76b3ca431bc68f93144a33dd8c5e8e5f036764a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140580"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="dba61-103">mobileAppSupportedDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dba61-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="dba61-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dba61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dba61-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dba61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dba61-106">デバイスのプロパティ</span><span class="sxs-lookup"><span data-stu-id="dba61-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="dba61-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dba61-107">Properties</span></span>
|<span data-ttu-id="dba61-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dba61-108">Property</span></span>|<span data-ttu-id="dba61-109">型</span><span class="sxs-lookup"><span data-stu-id="dba61-109">Type</span></span>|<span data-ttu-id="dba61-110">説明</span><span class="sxs-lookup"><span data-stu-id="dba61-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dba61-111">type</span><span class="sxs-lookup"><span data-stu-id="dba61-111">type</span></span>|[<span data-ttu-id="dba61-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="dba61-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="dba61-113">デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="dba61-113">Device type.</span></span> <span data-ttu-id="dba61-114">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="dba61-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="dba61-115">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="dba61-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="dba61-116">String</span><span class="sxs-lookup"><span data-stu-id="dba61-116">String</span></span>|<span data-ttu-id="dba61-117">最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="dba61-117">Minimum OS version</span></span>|
|<span data-ttu-id="dba61-118">最大化 umoper/systemversion</span><span class="sxs-lookup"><span data-stu-id="dba61-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="dba61-119">String</span><span class="sxs-lookup"><span data-stu-id="dba61-119">String</span></span>|<span data-ttu-id="dba61-120">最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="dba61-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="dba61-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dba61-121">Relationships</span></span>
<span data-ttu-id="dba61-122">なし</span><span class="sxs-lookup"><span data-stu-id="dba61-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dba61-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dba61-123">JSON Representation</span></span>
<span data-ttu-id="dba61-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dba61-124">Here is a JSON representation of the resource.</span></span>
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




