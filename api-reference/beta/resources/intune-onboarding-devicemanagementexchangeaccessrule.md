---
title: deviceManagementExchangeAccessRule リソースの種類
description: Exchange でのデバイス アクセス ルールです。
author: tfitzmac
ms.openlocfilehash: 3d56365bb30825c48139d746fe048649940b5d55
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339593"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="b3bb9-103">deviceManagementExchangeAccessRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3bb9-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="b3bb9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b3bb9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3bb9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3bb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3bb9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3bb9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3bb9-107">Exchange でのデバイス アクセス ルールです。</span><span class="sxs-lookup"><span data-stu-id="b3bb9-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="b3bb9-108">Properties</span><span class="sxs-lookup"><span data-stu-id="b3bb9-108">Properties</span></span>
|<span data-ttu-id="b3bb9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3bb9-109">Property</span></span>|<span data-ttu-id="b3bb9-110">種類</span><span class="sxs-lookup"><span data-stu-id="b3bb9-110">Type</span></span>|<span data-ttu-id="b3bb9-111">説明</span><span class="sxs-lookup"><span data-stu-id="b3bb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3bb9-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="b3bb9-112">deviceClass</span></span>|[<span data-ttu-id="b3bb9-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="b3bb9-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="b3bb9-114">デバイス クラスはこの規則の影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="b3bb9-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="b3bb9-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="b3bb9-115">accessLevel</span></span>|[<span data-ttu-id="b3bb9-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="b3bb9-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="b3bb9-117">この規則によって付与された Exchange のアクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="b3bb9-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="b3bb9-118">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="b3bb9-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3bb9-119">関係</span><span class="sxs-lookup"><span data-stu-id="b3bb9-119">Relationships</span></span>
<span data-ttu-id="b3bb9-120">なし</span><span class="sxs-lookup"><span data-stu-id="b3bb9-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3bb9-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3bb9-121">JSON Representation</span></span>
<span data-ttu-id="b3bb9-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3bb9-122">Here is a JSON representation of the resource.</span></span>
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





