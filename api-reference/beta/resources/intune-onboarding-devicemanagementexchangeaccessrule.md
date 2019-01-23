---
title: deviceManagementExchangeAccessRule リソースの種類
description: Exchange でのデバイス アクセス ルールです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c46bff30bf5f88723a789bb13160bf5aedb1ef2a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409441"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="a0ab0-103">deviceManagementExchangeAccessRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0ab0-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="a0ab0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a0ab0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a0ab0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0ab0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0ab0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0ab0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0ab0-107">Exchange でのデバイス アクセス ルールです。</span><span class="sxs-lookup"><span data-stu-id="a0ab0-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="a0ab0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0ab0-108">Properties</span></span>
|<span data-ttu-id="a0ab0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0ab0-109">Property</span></span>|<span data-ttu-id="a0ab0-110">型</span><span class="sxs-lookup"><span data-stu-id="a0ab0-110">Type</span></span>|<span data-ttu-id="a0ab0-111">説明</span><span class="sxs-lookup"><span data-stu-id="a0ab0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0ab0-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="a0ab0-112">deviceClass</span></span>|[<span data-ttu-id="a0ab0-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="a0ab0-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="a0ab0-114">デバイス クラスはこの規則の影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="a0ab0-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="a0ab0-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="a0ab0-115">accessLevel</span></span>|[<span data-ttu-id="a0ab0-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="a0ab0-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="a0ab0-117">この規則によって付与された Exchange のアクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="a0ab0-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="a0ab0-118">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="a0ab0-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0ab0-119">関係</span><span class="sxs-lookup"><span data-stu-id="a0ab0-119">Relationships</span></span>
<span data-ttu-id="a0ab0-120">なし</span><span class="sxs-lookup"><span data-stu-id="a0ab0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0ab0-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0ab0-121">JSON Representation</span></span>
<span data-ttu-id="a0ab0-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a0ab0-122">Here is a JSON representation of the resource.</span></span>
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




