---
title: deviceManagementExchangeAccessRule リソースの種類
description: Exchange でのデバイス アクセス ルールです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d7f0e649d2c5f2f27a4623fa0f65cf43965f576
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855189"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="67b5b-103">deviceManagementExchangeAccessRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="67b5b-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="67b5b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="67b5b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67b5b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67b5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67b5b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="67b5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67b5b-107">Exchange でのデバイス アクセス ルールです。</span><span class="sxs-lookup"><span data-stu-id="67b5b-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="67b5b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67b5b-108">Properties</span></span>
|<span data-ttu-id="67b5b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67b5b-109">Property</span></span>|<span data-ttu-id="67b5b-110">種類</span><span class="sxs-lookup"><span data-stu-id="67b5b-110">Type</span></span>|<span data-ttu-id="67b5b-111">説明</span><span class="sxs-lookup"><span data-stu-id="67b5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67b5b-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="67b5b-112">deviceClass</span></span>|[<span data-ttu-id="67b5b-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="67b5b-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="67b5b-114">デバイス クラスはこの規則の影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="67b5b-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="67b5b-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="67b5b-115">accessLevel</span></span>|[<span data-ttu-id="67b5b-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="67b5b-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="67b5b-117">この規則によって付与された Exchange のアクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="67b5b-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="67b5b-118">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="67b5b-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67b5b-119">関係</span><span class="sxs-lookup"><span data-stu-id="67b5b-119">Relationships</span></span>
<span data-ttu-id="67b5b-120">なし</span><span class="sxs-lookup"><span data-stu-id="67b5b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67b5b-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67b5b-121">JSON Representation</span></span>
<span data-ttu-id="67b5b-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="67b5b-122">Here is a JSON representation of the resource.</span></span>
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





