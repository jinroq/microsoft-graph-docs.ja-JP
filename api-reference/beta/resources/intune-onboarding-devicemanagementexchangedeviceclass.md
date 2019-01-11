---
title: deviceManagementExchangeDeviceClass リソースの種類
description: Exchange でのデバイスのクラスです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 80142f4e05752a37c324cd20ce96e4c8e6668c03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839026"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="bfe0e-103">deviceManagementExchangeDeviceClass リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bfe0e-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="bfe0e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bfe0e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfe0e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfe0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bfe0e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfe0e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfe0e-107">Exchange でのデバイスのクラスです。</span><span class="sxs-lookup"><span data-stu-id="bfe0e-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="bfe0e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfe0e-108">Properties</span></span>
|<span data-ttu-id="bfe0e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfe0e-109">Property</span></span>|<span data-ttu-id="bfe0e-110">種類</span><span class="sxs-lookup"><span data-stu-id="bfe0e-110">Type</span></span>|<span data-ttu-id="bfe0e-111">説明</span><span class="sxs-lookup"><span data-stu-id="bfe0e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfe0e-112">名前</span><span class="sxs-lookup"><span data-stu-id="bfe0e-112">name</span></span>|<span data-ttu-id="bfe0e-113">String</span><span class="sxs-lookup"><span data-stu-id="bfe0e-113">String</span></span>|<span data-ttu-id="bfe0e-114">このルールの影響を受けるデバイス クラスの名前です。</span><span class="sxs-lookup"><span data-stu-id="bfe0e-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="bfe0e-115">type</span><span class="sxs-lookup"><span data-stu-id="bfe0e-115">type</span></span>|[<span data-ttu-id="bfe0e-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="bfe0e-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="bfe0e-117">このルールの影響を受けるデバイスの種類など、ファミリです。</span><span class="sxs-lookup"><span data-stu-id="bfe0e-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="bfe0e-118">可能な値: `family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="bfe0e-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfe0e-119">関係</span><span class="sxs-lookup"><span data-stu-id="bfe0e-119">Relationships</span></span>
<span data-ttu-id="bfe0e-120">なし</span><span class="sxs-lookup"><span data-stu-id="bfe0e-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bfe0e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bfe0e-121">JSON Representation</span></span>
<span data-ttu-id="bfe0e-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bfe0e-122">Here is a JSON representation of the resource.</span></span>
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





