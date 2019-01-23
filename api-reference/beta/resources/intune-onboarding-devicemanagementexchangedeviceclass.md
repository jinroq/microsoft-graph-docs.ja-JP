---
title: deviceManagementExchangeDeviceClass リソースの種類
description: Exchange でのデバイスのクラスです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e512253a9b9bc4228d41c369501bec1e7a5e031
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413732"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="c0876-103">deviceManagementExchangeDeviceClass リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0876-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="c0876-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0876-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0876-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0876-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0876-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c0876-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0876-107">Exchange でのデバイスのクラスです。</span><span class="sxs-lookup"><span data-stu-id="c0876-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="c0876-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0876-108">Properties</span></span>
|<span data-ttu-id="c0876-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0876-109">Property</span></span>|<span data-ttu-id="c0876-110">型</span><span class="sxs-lookup"><span data-stu-id="c0876-110">Type</span></span>|<span data-ttu-id="c0876-111">説明</span><span class="sxs-lookup"><span data-stu-id="c0876-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0876-112">name</span><span class="sxs-lookup"><span data-stu-id="c0876-112">name</span></span>|<span data-ttu-id="c0876-113">String</span><span class="sxs-lookup"><span data-stu-id="c0876-113">String</span></span>|<span data-ttu-id="c0876-114">このルールの影響を受けるデバイス クラスの名前です。</span><span class="sxs-lookup"><span data-stu-id="c0876-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="c0876-115">type</span><span class="sxs-lookup"><span data-stu-id="c0876-115">type</span></span>|[<span data-ttu-id="c0876-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="c0876-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="c0876-117">このルールの影響を受けるデバイスの種類など、ファミリです。</span><span class="sxs-lookup"><span data-stu-id="c0876-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="c0876-118">可能な値: `family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="c0876-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0876-119">関係</span><span class="sxs-lookup"><span data-stu-id="c0876-119">Relationships</span></span>
<span data-ttu-id="c0876-120">なし</span><span class="sxs-lookup"><span data-stu-id="c0876-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0876-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0876-121">JSON Representation</span></span>
<span data-ttu-id="c0876-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c0876-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```




