---
title: mobileAppSupportedDeviceType リソースの種類
description: デバイスのプロパティ
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c01691b3f6fcb2ed5838c1c9103c99ad6fbe792f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399753"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="99ffc-103">mobileAppSupportedDeviceType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99ffc-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="99ffc-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="99ffc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99ffc-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99ffc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99ffc-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="99ffc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99ffc-107">デバイスのプロパティ</span><span class="sxs-lookup"><span data-stu-id="99ffc-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="99ffc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99ffc-108">Properties</span></span>
|<span data-ttu-id="99ffc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99ffc-109">Property</span></span>|<span data-ttu-id="99ffc-110">型</span><span class="sxs-lookup"><span data-stu-id="99ffc-110">Type</span></span>|<span data-ttu-id="99ffc-111">説明</span><span class="sxs-lookup"><span data-stu-id="99ffc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99ffc-112">type</span><span class="sxs-lookup"><span data-stu-id="99ffc-112">type</span></span>|[<span data-ttu-id="99ffc-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="99ffc-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="99ffc-114">デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="99ffc-114">Device type.</span></span> <span data-ttu-id="99ffc-115">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="99ffc-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="99ffc-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="99ffc-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="99ffc-117">String</span><span class="sxs-lookup"><span data-stu-id="99ffc-117">String</span></span>|<span data-ttu-id="99ffc-118">OS の最小バージョン</span><span class="sxs-lookup"><span data-stu-id="99ffc-118">Minimum OS version</span></span>|
|<span data-ttu-id="99ffc-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="99ffc-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="99ffc-120">String</span><span class="sxs-lookup"><span data-stu-id="99ffc-120">String</span></span>|<span data-ttu-id="99ffc-121">OS の最大バージョン</span><span class="sxs-lookup"><span data-stu-id="99ffc-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="99ffc-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="99ffc-122">Relationships</span></span>
<span data-ttu-id="99ffc-123">なし</span><span class="sxs-lookup"><span data-stu-id="99ffc-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99ffc-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99ffc-124">JSON Representation</span></span>
<span data-ttu-id="99ffc-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="99ffc-125">Here is a JSON representation of the resource.</span></span>
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




