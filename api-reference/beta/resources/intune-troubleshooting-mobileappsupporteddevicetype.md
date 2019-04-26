---
title: mobileAppSupportedDeviceType リソースの種類
description: デバイスのプロパティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba2998e1312d24fe6f86420cea883e6039f813a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570660"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="f3480-103">mobileAppSupportedDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3480-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="f3480-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3480-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3480-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3480-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3480-106">デバイスのプロパティ</span><span class="sxs-lookup"><span data-stu-id="f3480-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="f3480-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3480-107">Properties</span></span>
|<span data-ttu-id="f3480-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3480-108">Property</span></span>|<span data-ttu-id="f3480-109">型</span><span class="sxs-lookup"><span data-stu-id="f3480-109">Type</span></span>|<span data-ttu-id="f3480-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3480-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3480-111">type</span><span class="sxs-lookup"><span data-stu-id="f3480-111">type</span></span>|[<span data-ttu-id="f3480-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="f3480-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="f3480-113">デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="f3480-113">Device type.</span></span> <span data-ttu-id="f3480-114">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f3480-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="f3480-115">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="f3480-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="f3480-116">String</span><span class="sxs-lookup"><span data-stu-id="f3480-116">String</span></span>|<span data-ttu-id="f3480-117">最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="f3480-117">Minimum OS version</span></span>|
|<span data-ttu-id="f3480-118">最大化 umoper/systemversion</span><span class="sxs-lookup"><span data-stu-id="f3480-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="f3480-119">String</span><span class="sxs-lookup"><span data-stu-id="f3480-119">String</span></span>|<span data-ttu-id="f3480-120">最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="f3480-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3480-121">関係</span><span class="sxs-lookup"><span data-stu-id="f3480-121">Relationships</span></span>
<span data-ttu-id="f3480-122">なし</span><span class="sxs-lookup"><span data-stu-id="f3480-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3480-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3480-123">JSON Representation</span></span>
<span data-ttu-id="f3480-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3480-124">Here is a JSON representation of the resource.</span></span>
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



