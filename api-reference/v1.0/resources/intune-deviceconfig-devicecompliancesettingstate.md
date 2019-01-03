---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: tfitzmac
ms.openlocfilehash: e4edce4b22b70c6018703e086d606b84781b6b91
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326174"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="a2380-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="a2380-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="a2380-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2380-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2380-105">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="a2380-105">Device compliance setting State for a given device.</span></span>
## <a name="methods"></a><span data-ttu-id="a2380-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2380-106">Methods</span></span>
|<span data-ttu-id="a2380-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a2380-107">Method</span></span>|<span data-ttu-id="a2380-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a2380-108">Return Type</span></span>|<span data-ttu-id="a2380-109">説明</span><span class="sxs-lookup"><span data-stu-id="a2380-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2380-110">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="a2380-110">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="a2380-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a2380-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="a2380-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a2380-112">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="a2380-113">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a2380-113">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="a2380-114">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a2380-114">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a2380-115">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a2380-115">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="a2380-116">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a2380-116">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="a2380-117">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a2380-117">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a2380-118">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a2380-118">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="a2380-119">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a2380-119">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="a2380-120">なし</span><span class="sxs-lookup"><span data-stu-id="a2380-120">None</span></span>|<span data-ttu-id="a2380-121">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a2380-121">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="a2380-122">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a2380-122">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="a2380-123">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a2380-123">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a2380-124">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a2380-124">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2380-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2380-125">Properties</span></span>
|<span data-ttu-id="a2380-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2380-126">Property</span></span>|<span data-ttu-id="a2380-127">種類</span><span class="sxs-lookup"><span data-stu-id="a2380-127">Type</span></span>|<span data-ttu-id="a2380-128">説明</span><span class="sxs-lookup"><span data-stu-id="a2380-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2380-129">ID</span><span class="sxs-lookup"><span data-stu-id="a2380-129">id</span></span>|<span data-ttu-id="a2380-130">String</span><span class="sxs-lookup"><span data-stu-id="a2380-130">String</span></span>|<span data-ttu-id="a2380-131">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="a2380-131">Key of the entity</span></span>|
|<span data-ttu-id="a2380-132">setting</span><span class="sxs-lookup"><span data-stu-id="a2380-132">setting</span></span>|<span data-ttu-id="a2380-133">String</span><span class="sxs-lookup"><span data-stu-id="a2380-133">String</span></span>|<span data-ttu-id="a2380-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="a2380-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="a2380-135">settingName</span><span class="sxs-lookup"><span data-stu-id="a2380-135">settingName</span></span>|<span data-ttu-id="a2380-136">String</span><span class="sxs-lookup"><span data-stu-id="a2380-136">String</span></span>|<span data-ttu-id="a2380-137">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="a2380-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="a2380-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="a2380-138">deviceId</span></span>|<span data-ttu-id="a2380-139">String</span><span class="sxs-lookup"><span data-stu-id="a2380-139">String</span></span>|<span data-ttu-id="a2380-140">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="a2380-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="a2380-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="a2380-141">deviceName</span></span>|<span data-ttu-id="a2380-142">String</span><span class="sxs-lookup"><span data-stu-id="a2380-142">String</span></span>|<span data-ttu-id="a2380-143">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="a2380-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="a2380-144">userId</span><span class="sxs-lookup"><span data-stu-id="a2380-144">userId</span></span>|<span data-ttu-id="a2380-145">String</span><span class="sxs-lookup"><span data-stu-id="a2380-145">String</span></span>|<span data-ttu-id="a2380-146">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="a2380-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="a2380-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="a2380-147">userEmail</span></span>|<span data-ttu-id="a2380-148">String</span><span class="sxs-lookup"><span data-stu-id="a2380-148">String</span></span>|<span data-ttu-id="a2380-149">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="a2380-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="a2380-150">userName</span><span class="sxs-lookup"><span data-stu-id="a2380-150">userName</span></span>|<span data-ttu-id="a2380-151">String</span><span class="sxs-lookup"><span data-stu-id="a2380-151">String</span></span>|<span data-ttu-id="a2380-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="a2380-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="a2380-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2380-153">userPrincipalName</span></span>|<span data-ttu-id="a2380-154">String</span><span class="sxs-lookup"><span data-stu-id="a2380-154">String</span></span>|<span data-ttu-id="a2380-155">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2380-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="a2380-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a2380-156">deviceModel</span></span>|<span data-ttu-id="a2380-157">String</span><span class="sxs-lookup"><span data-stu-id="a2380-157">String</span></span>|<span data-ttu-id="a2380-158">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="a2380-158">The device model that is being reported</span></span>|
|<span data-ttu-id="a2380-159">state</span><span class="sxs-lookup"><span data-stu-id="a2380-159">state</span></span>|[<span data-ttu-id="a2380-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a2380-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a2380-161">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="a2380-161">The compliance state of the setting.</span></span> <span data-ttu-id="a2380-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="a2380-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a2380-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a2380-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a2380-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2380-164">DateTimeOffset</span></span>|<span data-ttu-id="a2380-165">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="a2380-165">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2380-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2380-166">Relationships</span></span>
<span data-ttu-id="a2380-167">なし</span><span class="sxs-lookup"><span data-stu-id="a2380-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a2380-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2380-168">JSON Representation</span></span>
<span data-ttu-id="a2380-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2380-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```


