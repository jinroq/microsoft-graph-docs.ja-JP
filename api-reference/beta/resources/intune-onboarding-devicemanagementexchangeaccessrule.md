---
title: devicemanagementexchangeaccessrule リソースの種類
description: Exchange のデバイスアクセスルール。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 832e11829300ccd1ac4e1d4e6b08acafb908f3b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566606"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="c9859-103">devicemanagementexchangeaccessrule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9859-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="c9859-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9859-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9859-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9859-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9859-106">Exchange のデバイスアクセスルール。</span><span class="sxs-lookup"><span data-stu-id="c9859-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="c9859-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9859-107">Properties</span></span>
|<span data-ttu-id="c9859-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9859-108">Property</span></span>|<span data-ttu-id="c9859-109">型</span><span class="sxs-lookup"><span data-stu-id="c9859-109">Type</span></span>|<span data-ttu-id="c9859-110">説明</span><span class="sxs-lookup"><span data-stu-id="c9859-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9859-111">deviceclass</span><span class="sxs-lookup"><span data-stu-id="c9859-111">deviceClass</span></span>|[<span data-ttu-id="c9859-112">devicemanagementexchangedeviceclass</span><span class="sxs-lookup"><span data-stu-id="c9859-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="c9859-113">このルールの影響を受けるデバイスクラス。</span><span class="sxs-lookup"><span data-stu-id="c9859-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="c9859-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="c9859-114">accessLevel</span></span>|[<span data-ttu-id="c9859-115">devicemanagementexchangeaccesslevel</span><span class="sxs-lookup"><span data-stu-id="c9859-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="c9859-116">このルールによって付与される Exchange のアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="c9859-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="c9859-117">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="c9859-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9859-118">関係</span><span class="sxs-lookup"><span data-stu-id="c9859-118">Relationships</span></span>
<span data-ttu-id="c9859-119">なし</span><span class="sxs-lookup"><span data-stu-id="c9859-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9859-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9859-120">JSON Representation</span></span>
<span data-ttu-id="c9859-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9859-121">Here is a JSON representation of the resource.</span></span>
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





