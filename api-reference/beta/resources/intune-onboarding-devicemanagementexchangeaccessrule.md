---
title: deviceManagementExchangeAccessRule リソースの種類
description: Exchange のデバイスアクセスルール。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d435d699b2cd30617a9e709ef8e9ba86eabd46b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010792"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="03ee5-103">deviceManagementExchangeAccessRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03ee5-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="03ee5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03ee5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03ee5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="03ee5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03ee5-106">Exchange のデバイスアクセスルール。</span><span class="sxs-lookup"><span data-stu-id="03ee5-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="03ee5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03ee5-107">Properties</span></span>
|<span data-ttu-id="03ee5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03ee5-108">Property</span></span>|<span data-ttu-id="03ee5-109">型</span><span class="sxs-lookup"><span data-stu-id="03ee5-109">Type</span></span>|<span data-ttu-id="03ee5-110">説明</span><span class="sxs-lookup"><span data-stu-id="03ee5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03ee5-111">deviceClass</span><span class="sxs-lookup"><span data-stu-id="03ee5-111">deviceClass</span></span>|[<span data-ttu-id="03ee5-112">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="03ee5-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="03ee5-113">このルールの影響を受けるデバイスクラス。</span><span class="sxs-lookup"><span data-stu-id="03ee5-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="03ee5-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="03ee5-114">accessLevel</span></span>|[<span data-ttu-id="03ee5-115">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="03ee5-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="03ee5-116">このルールによって付与される Exchange のアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="03ee5-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="03ee5-117">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="03ee5-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03ee5-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="03ee5-118">Relationships</span></span>
<span data-ttu-id="03ee5-119">なし</span><span class="sxs-lookup"><span data-stu-id="03ee5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03ee5-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03ee5-120">JSON Representation</span></span>
<span data-ttu-id="03ee5-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="03ee5-121">Here is a JSON representation of the resource.</span></span>
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





