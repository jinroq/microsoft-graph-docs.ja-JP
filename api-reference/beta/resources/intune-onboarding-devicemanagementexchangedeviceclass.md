---
title: deviceManagementExchangeDeviceClass リソースの種類
description: Exchange でのデバイスのクラスです。
author: tfitzmac
ms.openlocfilehash: 01e0877388391deaebbda18e48247f4e3585a63a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316780"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="17594-103">deviceManagementExchangeDeviceClass リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17594-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="17594-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="17594-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17594-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17594-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17594-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="17594-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17594-107">Exchange でのデバイスのクラスです。</span><span class="sxs-lookup"><span data-stu-id="17594-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="17594-108">Properties</span><span class="sxs-lookup"><span data-stu-id="17594-108">Properties</span></span>
|<span data-ttu-id="17594-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17594-109">Property</span></span>|<span data-ttu-id="17594-110">種類</span><span class="sxs-lookup"><span data-stu-id="17594-110">Type</span></span>|<span data-ttu-id="17594-111">説明</span><span class="sxs-lookup"><span data-stu-id="17594-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17594-112">名前</span><span class="sxs-lookup"><span data-stu-id="17594-112">name</span></span>|<span data-ttu-id="17594-113">String</span><span class="sxs-lookup"><span data-stu-id="17594-113">String</span></span>|<span data-ttu-id="17594-114">このルールの影響を受けるデバイス クラスの名前です。</span><span class="sxs-lookup"><span data-stu-id="17594-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="17594-115">type</span><span class="sxs-lookup"><span data-stu-id="17594-115">type</span></span>|[<span data-ttu-id="17594-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="17594-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="17594-117">このルールの影響を受けるデバイスの種類など、ファミリです。</span><span class="sxs-lookup"><span data-stu-id="17594-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="17594-118">可能な値: `family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="17594-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17594-119">関係</span><span class="sxs-lookup"><span data-stu-id="17594-119">Relationships</span></span>
<span data-ttu-id="17594-120">なし</span><span class="sxs-lookup"><span data-stu-id="17594-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17594-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17594-121">JSON Representation</span></span>
<span data-ttu-id="17594-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17594-122">Here is a JSON representation of the resource.</span></span>
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





