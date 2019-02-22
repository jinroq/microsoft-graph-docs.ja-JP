---
title: devicemanagementexchangeaccessrule リソースの種類
description: Exchange のデバイスアクセスルール。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38b021bc2f0a4ffa19ca551c2621b08f21e8a35e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165780"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="050f1-103">devicemanagementexchangeaccessrule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="050f1-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="050f1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="050f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="050f1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="050f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="050f1-106">Exchange のデバイスアクセスルール。</span><span class="sxs-lookup"><span data-stu-id="050f1-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="050f1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="050f1-107">Properties</span></span>
|<span data-ttu-id="050f1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="050f1-108">Property</span></span>|<span data-ttu-id="050f1-109">型</span><span class="sxs-lookup"><span data-stu-id="050f1-109">Type</span></span>|<span data-ttu-id="050f1-110">説明</span><span class="sxs-lookup"><span data-stu-id="050f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="050f1-111">deviceclass</span><span class="sxs-lookup"><span data-stu-id="050f1-111">deviceClass</span></span>|[<span data-ttu-id="050f1-112">devicemanagementexchangedeviceclass</span><span class="sxs-lookup"><span data-stu-id="050f1-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="050f1-113">このルールの影響を受けるデバイスクラス。</span><span class="sxs-lookup"><span data-stu-id="050f1-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="050f1-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="050f1-114">accessLevel</span></span>|[<span data-ttu-id="050f1-115">devicemanagementexchangeaccesslevel</span><span class="sxs-lookup"><span data-stu-id="050f1-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="050f1-116">このルールによって付与される Exchange のアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="050f1-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="050f1-117">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="050f1-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="050f1-118">関係</span><span class="sxs-lookup"><span data-stu-id="050f1-118">Relationships</span></span>
<span data-ttu-id="050f1-119">なし</span><span class="sxs-lookup"><span data-stu-id="050f1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="050f1-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="050f1-120">JSON Representation</span></span>
<span data-ttu-id="050f1-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="050f1-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```




