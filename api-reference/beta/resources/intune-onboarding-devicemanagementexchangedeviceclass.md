---
title: deviceManagementExchangeDeviceClass リソースの種類
description: Exchange のデバイスクラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16ed6730363a8f33eeb9ad430f5d2fb56c518032
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940296"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="cfac8-103">deviceManagementExchangeDeviceClass リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cfac8-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="cfac8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfac8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfac8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cfac8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfac8-106">Exchange のデバイスクラス。</span><span class="sxs-lookup"><span data-stu-id="cfac8-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="cfac8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfac8-107">Properties</span></span>
|<span data-ttu-id="cfac8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfac8-108">Property</span></span>|<span data-ttu-id="cfac8-109">型</span><span class="sxs-lookup"><span data-stu-id="cfac8-109">Type</span></span>|<span data-ttu-id="cfac8-110">説明</span><span class="sxs-lookup"><span data-stu-id="cfac8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfac8-111">name</span><span class="sxs-lookup"><span data-stu-id="cfac8-111">name</span></span>|<span data-ttu-id="cfac8-112">String</span><span class="sxs-lookup"><span data-stu-id="cfac8-112">String</span></span>|<span data-ttu-id="cfac8-113">このルールの影響を受けるデバイスクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="cfac8-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="cfac8-114">type</span><span class="sxs-lookup"><span data-stu-id="cfac8-114">type</span></span>|[<span data-ttu-id="cfac8-115">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="cfac8-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="cfac8-116">このルールの影響を受けるデバイスの種類 (例: Model, Family)。</span><span class="sxs-lookup"><span data-stu-id="cfac8-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="cfac8-117">可能な値: `family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="cfac8-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfac8-118">関係</span><span class="sxs-lookup"><span data-stu-id="cfac8-118">Relationships</span></span>
<span data-ttu-id="cfac8-119">なし</span><span class="sxs-lookup"><span data-stu-id="cfac8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfac8-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cfac8-120">JSON Representation</span></span>
<span data-ttu-id="cfac8-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cfac8-121">Here is a JSON representation of the resource.</span></span>
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




