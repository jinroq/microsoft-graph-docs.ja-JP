---
title: devicemanagementexchangedeviceclass リソースの種類
description: Exchange のデバイスクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ec9f0242521bf23b4ed5f1c9f002211d542e48c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774660"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="eb18a-103">devicemanagementexchangedeviceclass リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb18a-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="eb18a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb18a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb18a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb18a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb18a-106">Exchange のデバイスクラス。</span><span class="sxs-lookup"><span data-stu-id="eb18a-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="eb18a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb18a-107">Properties</span></span>
|<span data-ttu-id="eb18a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb18a-108">Property</span></span>|<span data-ttu-id="eb18a-109">型</span><span class="sxs-lookup"><span data-stu-id="eb18a-109">Type</span></span>|<span data-ttu-id="eb18a-110">説明</span><span class="sxs-lookup"><span data-stu-id="eb18a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb18a-111">name</span><span class="sxs-lookup"><span data-stu-id="eb18a-111">name</span></span>|<span data-ttu-id="eb18a-112">String</span><span class="sxs-lookup"><span data-stu-id="eb18a-112">String</span></span>|<span data-ttu-id="eb18a-113">このルールの影響を受けるデバイスクラスの名前。</span><span class="sxs-lookup"><span data-stu-id="eb18a-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="eb18a-114">type</span><span class="sxs-lookup"><span data-stu-id="eb18a-114">type</span></span>|[<span data-ttu-id="eb18a-115">devicemanagementexchangeaccessruletype</span><span class="sxs-lookup"><span data-stu-id="eb18a-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="eb18a-116">このルールの影響を受けるデバイスの種類 (例: Model, Family)。</span><span class="sxs-lookup"><span data-stu-id="eb18a-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="eb18a-117">可能な値: `family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="eb18a-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb18a-118">関係</span><span class="sxs-lookup"><span data-stu-id="eb18a-118">Relationships</span></span>
<span data-ttu-id="eb18a-119">なし</span><span class="sxs-lookup"><span data-stu-id="eb18a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb18a-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb18a-120">JSON Representation</span></span>
<span data-ttu-id="eb18a-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb18a-121">Here is a JSON representation of the resource.</span></span>
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





