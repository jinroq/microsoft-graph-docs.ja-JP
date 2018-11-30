---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
ms.openlocfilehash: f91e7eb4cdd72899b32419fc9401c055fff0bc3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023208"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="f12e9-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="f12e9-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="f12e9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f12e9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f12e9-105">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="f12e9-105">Device compliance setting State for a given device.</span></span>
## <a name="methods"></a><span data-ttu-id="f12e9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f12e9-106">Methods</span></span>
|<span data-ttu-id="f12e9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f12e9-107">Method</span></span>|<span data-ttu-id="f12e9-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f12e9-108">Return Type</span></span>|<span data-ttu-id="f12e9-109">説明</span><span class="sxs-lookup"><span data-stu-id="f12e9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f12e9-110">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="f12e9-110">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="f12e9-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f12e9-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="f12e9-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f12e9-112">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="f12e9-113">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f12e9-113">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="f12e9-114">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f12e9-114">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="f12e9-115">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f12e9-115">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="f12e9-116">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f12e9-116">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="f12e9-117">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f12e9-117">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="f12e9-118">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f12e9-118">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="f12e9-119">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f12e9-119">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="f12e9-120">なし</span><span class="sxs-lookup"><span data-stu-id="f12e9-120">None</span></span>|<span data-ttu-id="f12e9-121">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f12e9-121">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="f12e9-122">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f12e9-122">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="f12e9-123">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="f12e9-123">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="f12e9-124">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f12e9-124">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f12e9-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f12e9-125">Properties</span></span>
|<span data-ttu-id="f12e9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f12e9-126">Property</span></span>|<span data-ttu-id="f12e9-127">型</span><span class="sxs-lookup"><span data-stu-id="f12e9-127">Type</span></span>|<span data-ttu-id="f12e9-128">説明</span><span class="sxs-lookup"><span data-stu-id="f12e9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f12e9-129">id</span><span class="sxs-lookup"><span data-stu-id="f12e9-129">id</span></span>|<span data-ttu-id="f12e9-130">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-130">String</span></span>|<span data-ttu-id="f12e9-131">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="f12e9-131">Key of the entity</span></span>|
|<span data-ttu-id="f12e9-132">setting</span><span class="sxs-lookup"><span data-stu-id="f12e9-132">setting</span></span>|<span data-ttu-id="f12e9-133">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-133">String</span></span>|<span data-ttu-id="f12e9-134">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="f12e9-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="f12e9-135">settingName</span><span class="sxs-lookup"><span data-stu-id="f12e9-135">settingName</span></span>|<span data-ttu-id="f12e9-136">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-136">String</span></span>|<span data-ttu-id="f12e9-137">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="f12e9-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="f12e9-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="f12e9-138">deviceId</span></span>|<span data-ttu-id="f12e9-139">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-139">String</span></span>|<span data-ttu-id="f12e9-140">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="f12e9-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="f12e9-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="f12e9-141">deviceName</span></span>|<span data-ttu-id="f12e9-142">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-142">String</span></span>|<span data-ttu-id="f12e9-143">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="f12e9-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="f12e9-144">userId</span><span class="sxs-lookup"><span data-stu-id="f12e9-144">userId</span></span>|<span data-ttu-id="f12e9-145">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-145">String</span></span>|<span data-ttu-id="f12e9-146">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="f12e9-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="f12e9-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="f12e9-147">userEmail</span></span>|<span data-ttu-id="f12e9-148">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-148">String</span></span>|<span data-ttu-id="f12e9-149">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="f12e9-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="f12e9-150">userName</span><span class="sxs-lookup"><span data-stu-id="f12e9-150">userName</span></span>|<span data-ttu-id="f12e9-151">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-151">String</span></span>|<span data-ttu-id="f12e9-152">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="f12e9-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="f12e9-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f12e9-153">userPrincipalName</span></span>|<span data-ttu-id="f12e9-154">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-154">String</span></span>|<span data-ttu-id="f12e9-155">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="f12e9-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="f12e9-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f12e9-156">deviceModel</span></span>|<span data-ttu-id="f12e9-157">String</span><span class="sxs-lookup"><span data-stu-id="f12e9-157">String</span></span>|<span data-ttu-id="f12e9-158">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="f12e9-158">The device model that is being reported</span></span>|
|<span data-ttu-id="f12e9-159">state</span><span class="sxs-lookup"><span data-stu-id="f12e9-159">state</span></span>|[<span data-ttu-id="f12e9-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f12e9-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f12e9-161">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="f12e9-161">The compliance state of the setting.</span></span> <span data-ttu-id="f12e9-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="f12e9-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f12e9-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f12e9-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f12e9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f12e9-164">DateTimeOffset</span></span>|<span data-ttu-id="f12e9-165">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="f12e9-165">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="f12e9-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f12e9-166">Relationships</span></span>
<span data-ttu-id="f12e9-167">なし</span><span class="sxs-lookup"><span data-stu-id="f12e9-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f12e9-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f12e9-168">JSON Representation</span></span>
<span data-ttu-id="f12e9-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f12e9-169">Here is a JSON representation of the resource.</span></span>
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



