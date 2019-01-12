---
title: deviceManagementExchangeOnPremisesPolicy リソースの種類
description: テナント用に構成された Exchange OnPremises ポリシーを表す単一のエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c4f513242694228b53268772d9b2910fa40bbd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990335"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a><span data-ttu-id="6bbad-103">deviceManagementExchangeOnPremisesPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6bbad-103">deviceManagementExchangeOnPremisesPolicy resource type</span></span>

> <span data-ttu-id="6bbad-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6bbad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bbad-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6bbad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bbad-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6bbad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bbad-107">テナント用に構成された Exchange OnPremises ポリシーを表す単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="6bbad-107">Singleton entity which represents the Exchange OnPremises policy configured for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="6bbad-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6bbad-108">Methods</span></span>
|<span data-ttu-id="6bbad-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="6bbad-109">Method</span></span>|<span data-ttu-id="6bbad-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6bbad-110">Return Type</span></span>|<span data-ttu-id="6bbad-111">説明</span><span class="sxs-lookup"><span data-stu-id="6bbad-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6bbad-112">DeviceManagementExchangeOnPremisesPolicy を取得します。</span><span class="sxs-lookup"><span data-stu-id="6bbad-112">Get deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[<span data-ttu-id="6bbad-113">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="6bbad-113">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="6bbad-114">[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6bbad-114">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|
|[<span data-ttu-id="6bbad-115">DeviceManagementExchangeOnPremisesPolicy を更新します。</span><span class="sxs-lookup"><span data-stu-id="6bbad-115">Update deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[<span data-ttu-id="6bbad-116">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="6bbad-116">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="6bbad-117">[DeviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6bbad-117">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6bbad-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bbad-118">Properties</span></span>
|<span data-ttu-id="6bbad-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bbad-119">Property</span></span>|<span data-ttu-id="6bbad-120">種類</span><span class="sxs-lookup"><span data-stu-id="6bbad-120">Type</span></span>|<span data-ttu-id="6bbad-121">説明</span><span class="sxs-lookup"><span data-stu-id="6bbad-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bbad-122">ID</span><span class="sxs-lookup"><span data-stu-id="6bbad-122">id</span></span>|<span data-ttu-id="6bbad-123">String</span><span class="sxs-lookup"><span data-stu-id="6bbad-123">String</span></span>|<span data-ttu-id="6bbad-124">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6bbad-124">Not yet documented</span></span>|
|<span data-ttu-id="6bbad-125">notificationContent</span><span class="sxs-lookup"><span data-stu-id="6bbad-125">notificationContent</span></span>|<span data-ttu-id="6bbad-126">Binary</span><span class="sxs-lookup"><span data-stu-id="6bbad-126">Binary</span></span>|<span data-ttu-id="6bbad-127">このポリシーで検疫されたユーザーに送信される通知のテキストです。</span><span class="sxs-lookup"><span data-stu-id="6bbad-127">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="6bbad-128">これは、UTF8 のエンコードされたバイト配列 HTML です。</span><span class="sxs-lookup"><span data-stu-id="6bbad-128">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="6bbad-129">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="6bbad-129">defaultAccessLevel</span></span>|[<span data-ttu-id="6bbad-130">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="6bbad-130">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="6bbad-131">Exchange の既定のアクセス状態。</span><span class="sxs-lookup"><span data-stu-id="6bbad-131">Default access state in Exchange.</span></span> <span data-ttu-id="6bbad-132">このルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="6bbad-132">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="6bbad-133">可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="6bbad-133">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="6bbad-134">accessRules</span><span class="sxs-lookup"><span data-stu-id="6bbad-134">accessRules</span></span>|<span data-ttu-id="6bbad-135">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6bbad-135">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="6bbad-136">デバイスへのアクセスの一覧で Exchange ルールします。</span><span class="sxs-lookup"><span data-stu-id="6bbad-136">The list of device access rules in Exchange.</span></span> <span data-ttu-id="6bbad-137">アクセス ルールは、Exchange 組織全体にグローバルに適用します。</span><span class="sxs-lookup"><span data-stu-id="6bbad-137">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="6bbad-138">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="6bbad-138">knownDeviceClasses</span></span>|<span data-ttu-id="6bbad-139">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6bbad-139">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="6bbad-140">Exchange に既知のデバイス クラスの一覧</span><span class="sxs-lookup"><span data-stu-id="6bbad-140">The list of device classes known to Exchange</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bbad-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bbad-141">Relationships</span></span>
|<span data-ttu-id="6bbad-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bbad-142">Relationship</span></span>|<span data-ttu-id="6bbad-143">型</span><span class="sxs-lookup"><span data-stu-id="6bbad-143">Type</span></span>|<span data-ttu-id="6bbad-144">説明</span><span class="sxs-lookup"><span data-stu-id="6bbad-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bbad-145">conditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="6bbad-145">conditionalAccessSettings</span></span>|[<span data-ttu-id="6bbad-146">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="6bbad-146">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="6bbad-147">Exchange のオンプレミスでの条件付きアクセス設定。</span><span class="sxs-lookup"><span data-stu-id="6bbad-147">The Exchange on premises conditional access settings.</span></span> <span data-ttu-id="6bbad-148">オンプレミスの条件付きアクセスでは、デバイスを登録し、メール アクセスに準拠させる必要があります</span><span class="sxs-lookup"><span data-stu-id="6bbad-148">On premises conditional access will require devices to be both enrolled and compliant for mail access</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bbad-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6bbad-149">JSON Representation</span></span>
<span data-ttu-id="6bbad-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6bbad-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeOnPremisesPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "String (identifier)",
  "notificationContent": "binary",
  "defaultAccessLevel": "String",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "String",
        "type": "String"
      },
      "accessLevel": "String"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "String",
      "type": "String"
    }
  ]
}
```





