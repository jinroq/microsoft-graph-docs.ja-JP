---
title: deviceManagementExchangeOnPremisesPolicy リソースの種類
description: テナントに対して構成された Exchange onpremises ポリシーを表すシングルトンエンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8605a3062d8808ea6a4d0b5397283f0ca82d920
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566571"
---
# <a name="devicemanagementexchangeonpremisespolicy-resource-type"></a><span data-ttu-id="25cee-103">deviceManagementExchangeOnPremisesPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25cee-103">deviceManagementExchangeOnPremisesPolicy resource type</span></span>

> <span data-ttu-id="25cee-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25cee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25cee-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="25cee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25cee-106">テナントに対して構成された Exchange onpremises ポリシーを表すシングルトンエンティティ。</span><span class="sxs-lookup"><span data-stu-id="25cee-106">Singleton entity which represents the Exchange OnPremises policy configured for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="25cee-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="25cee-107">Methods</span></span>
|<span data-ttu-id="25cee-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="25cee-108">Method</span></span>|<span data-ttu-id="25cee-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="25cee-109">Return Type</span></span>|<span data-ttu-id="25cee-110">説明</span><span class="sxs-lookup"><span data-stu-id="25cee-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="25cee-111">deviceManagementExchangeOnPremisesPolicy を取得する</span><span class="sxs-lookup"><span data-stu-id="25cee-111">Get deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-get.md)|[<span data-ttu-id="25cee-112">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="25cee-112">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="25cee-113">[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="25cee-113">Read properties and relationships of the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|
|[<span data-ttu-id="25cee-114">deviceManagementExchangeOnPremisesPolicy の更新</span><span class="sxs-lookup"><span data-stu-id="25cee-114">Update deviceManagementExchangeOnPremisesPolicy</span></span>](../api/intune-onboarding-devicemanagementexchangeonpremisespolicy-update.md)|[<span data-ttu-id="25cee-115">deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="25cee-115">deviceManagementExchangeOnPremisesPolicy</span></span>](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)|<span data-ttu-id="25cee-116">[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="25cee-116">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="25cee-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25cee-117">Properties</span></span>
|<span data-ttu-id="25cee-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25cee-118">Property</span></span>|<span data-ttu-id="25cee-119">型</span><span class="sxs-lookup"><span data-stu-id="25cee-119">Type</span></span>|<span data-ttu-id="25cee-120">説明</span><span class="sxs-lookup"><span data-stu-id="25cee-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25cee-121">id</span><span class="sxs-lookup"><span data-stu-id="25cee-121">id</span></span>|<span data-ttu-id="25cee-122">String</span><span class="sxs-lookup"><span data-stu-id="25cee-122">String</span></span>|<span data-ttu-id="25cee-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="25cee-123">Not yet documented</span></span>|
|<span data-ttu-id="25cee-124">notificationContent</span><span class="sxs-lookup"><span data-stu-id="25cee-124">notificationContent</span></span>|<span data-ttu-id="25cee-125">Binary</span><span class="sxs-lookup"><span data-stu-id="25cee-125">Binary</span></span>|<span data-ttu-id="25cee-126">このポリシーによって検疫されたユーザーに送信される通知テキスト。</span><span class="sxs-lookup"><span data-stu-id="25cee-126">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="25cee-127">これは、UTF8 でエンコードされたバイト配列 HTML です。</span><span class="sxs-lookup"><span data-stu-id="25cee-127">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="25cee-128">defaultaccesslevel</span><span class="sxs-lookup"><span data-stu-id="25cee-128">defaultAccessLevel</span></span>|[<span data-ttu-id="25cee-129">devicemanagementexchangeaccesslevel</span><span class="sxs-lookup"><span data-stu-id="25cee-129">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="25cee-130">Exchange の既定のアクセス状態。</span><span class="sxs-lookup"><span data-stu-id="25cee-130">Default access state in Exchange.</span></span> <span data-ttu-id="25cee-131">このルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="25cee-131">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="25cee-132">使用可能な値は、`none`、`allow`、`block`、`quarantine` です。</span><span class="sxs-lookup"><span data-stu-id="25cee-132">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="25cee-133">accessrules</span><span class="sxs-lookup"><span data-stu-id="25cee-133">accessRules</span></span>|<span data-ttu-id="25cee-134">[devicemanagementexchangeaccessrule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="25cee-134">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="25cee-135">Exchange のデバイスアクセスルールの一覧。</span><span class="sxs-lookup"><span data-stu-id="25cee-135">The list of device access rules in Exchange.</span></span> <span data-ttu-id="25cee-136">アクセスルールは、Exchange 組織全体にグローバルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="25cee-136">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="25cee-137">knowndeviceclasses 場合</span><span class="sxs-lookup"><span data-stu-id="25cee-137">knownDeviceClasses</span></span>|<span data-ttu-id="25cee-138">[devicemanagementexchangedeviceclass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="25cee-138">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="25cee-139">Exchange に認識されているデバイスクラスの一覧</span><span class="sxs-lookup"><span data-stu-id="25cee-139">The list of device classes known to Exchange</span></span>|

## <a name="relationships"></a><span data-ttu-id="25cee-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25cee-140">Relationships</span></span>
|<span data-ttu-id="25cee-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25cee-141">Relationship</span></span>|<span data-ttu-id="25cee-142">型</span><span class="sxs-lookup"><span data-stu-id="25cee-142">Type</span></span>|<span data-ttu-id="25cee-143">説明</span><span class="sxs-lookup"><span data-stu-id="25cee-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25cee-144">conditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="25cee-144">conditionalAccessSettings</span></span>|[<span data-ttu-id="25cee-145">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="25cee-145">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="25cee-146">Exchange のオンプレミスでの条件付きアクセス設定。</span><span class="sxs-lookup"><span data-stu-id="25cee-146">The Exchange on premises conditional access settings.</span></span> <span data-ttu-id="25cee-147">オンプレミスの条件付きアクセスでは、デバイスを登録し、メール アクセスに準拠させる必要があります</span><span class="sxs-lookup"><span data-stu-id="25cee-147">On premises conditional access will require devices to be both enrolled and compliant for mail access</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25cee-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25cee-148">JSON Representation</span></span>
<span data-ttu-id="25cee-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="25cee-149">Here is a JSON representation of the resource.</span></span>
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





