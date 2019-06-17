---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63d73fbf584daeda20de327c1b62a9ccaf38b3ac
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995463"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="a3018-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="a3018-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="a3018-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3018-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3018-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3018-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3018-106">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="a3018-106">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="a3018-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3018-107">Methods</span></span>
|<span data-ttu-id="a3018-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="a3018-108">Method</span></span>|<span data-ttu-id="a3018-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a3018-109">Return Type</span></span>|<span data-ttu-id="a3018-110">説明</span><span class="sxs-lookup"><span data-stu-id="a3018-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3018-111">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="a3018-111">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="a3018-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a3018-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="a3018-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a3018-113">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="a3018-114">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a3018-114">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="a3018-115">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a3018-115">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a3018-116">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a3018-116">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="a3018-117">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a3018-117">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="a3018-118">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a3018-118">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a3018-119">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a3018-119">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="a3018-120">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a3018-120">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="a3018-121">なし</span><span class="sxs-lookup"><span data-stu-id="a3018-121">None</span></span>|<span data-ttu-id="a3018-122">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a3018-122">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="a3018-123">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a3018-123">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="a3018-124">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a3018-124">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a3018-125">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a3018-125">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a3018-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3018-126">Properties</span></span>
|<span data-ttu-id="a3018-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3018-127">Property</span></span>|<span data-ttu-id="a3018-128">型</span><span class="sxs-lookup"><span data-stu-id="a3018-128">Type</span></span>|<span data-ttu-id="a3018-129">説明</span><span class="sxs-lookup"><span data-stu-id="a3018-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3018-130">id</span><span class="sxs-lookup"><span data-stu-id="a3018-130">id</span></span>|<span data-ttu-id="a3018-131">文字列</span><span class="sxs-lookup"><span data-stu-id="a3018-131">String</span></span>|<span data-ttu-id="a3018-132">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="a3018-132">Key of the entity</span></span>|
|<span data-ttu-id="a3018-133">platformType</span><span class="sxs-lookup"><span data-stu-id="a3018-133">platformType</span></span>|[<span data-ttu-id="a3018-134">deviceType</span><span class="sxs-lookup"><span data-stu-id="a3018-134">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a3018-135">デバイスプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="a3018-135">Device platform type.</span></span> <span data-ttu-id="a3018-136">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a3018-136">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a3018-137">setting</span><span class="sxs-lookup"><span data-stu-id="a3018-137">setting</span></span>|<span data-ttu-id="a3018-138">String</span><span class="sxs-lookup"><span data-stu-id="a3018-138">String</span></span>|<span data-ttu-id="a3018-139">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="a3018-139">The setting class name and property name.</span></span>|
|<span data-ttu-id="a3018-140">settingName</span><span class="sxs-lookup"><span data-stu-id="a3018-140">settingName</span></span>|<span data-ttu-id="a3018-141">String</span><span class="sxs-lookup"><span data-stu-id="a3018-141">String</span></span>|<span data-ttu-id="a3018-142">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="a3018-142">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="a3018-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="a3018-143">deviceId</span></span>|<span data-ttu-id="a3018-144">String</span><span class="sxs-lookup"><span data-stu-id="a3018-144">String</span></span>|<span data-ttu-id="a3018-145">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="a3018-145">The Device Id that is being reported</span></span>|
|<span data-ttu-id="a3018-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="a3018-146">deviceName</span></span>|<span data-ttu-id="a3018-147">String</span><span class="sxs-lookup"><span data-stu-id="a3018-147">String</span></span>|<span data-ttu-id="a3018-148">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="a3018-148">The Device Name that is being reported</span></span>|
|<span data-ttu-id="a3018-149">userId</span><span class="sxs-lookup"><span data-stu-id="a3018-149">userId</span></span>|<span data-ttu-id="a3018-150">String</span><span class="sxs-lookup"><span data-stu-id="a3018-150">String</span></span>|<span data-ttu-id="a3018-151">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="a3018-151">The user Id that is being reported</span></span>|
|<span data-ttu-id="a3018-152">userEmail</span><span class="sxs-lookup"><span data-stu-id="a3018-152">userEmail</span></span>|<span data-ttu-id="a3018-153">String</span><span class="sxs-lookup"><span data-stu-id="a3018-153">String</span></span>|<span data-ttu-id="a3018-154">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="a3018-154">The User email address that is being reported</span></span>|
|<span data-ttu-id="a3018-155">userName</span><span class="sxs-lookup"><span data-stu-id="a3018-155">userName</span></span>|<span data-ttu-id="a3018-156">String</span><span class="sxs-lookup"><span data-stu-id="a3018-156">String</span></span>|<span data-ttu-id="a3018-157">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="a3018-157">The User Name that is being reported</span></span>|
|<span data-ttu-id="a3018-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3018-158">userPrincipalName</span></span>|<span data-ttu-id="a3018-159">String</span><span class="sxs-lookup"><span data-stu-id="a3018-159">String</span></span>|<span data-ttu-id="a3018-160">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3018-160">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="a3018-161">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a3018-161">deviceModel</span></span>|<span data-ttu-id="a3018-162">String</span><span class="sxs-lookup"><span data-stu-id="a3018-162">String</span></span>|<span data-ttu-id="a3018-163">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="a3018-163">The device model that is being reported</span></span>|
|<span data-ttu-id="a3018-164">state</span><span class="sxs-lookup"><span data-stu-id="a3018-164">state</span></span>|[<span data-ttu-id="a3018-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a3018-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a3018-166">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="a3018-166">The compliance state of the setting.</span></span> <span data-ttu-id="a3018-167">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="a3018-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a3018-168">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a3018-168">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a3018-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3018-169">DateTimeOffset</span></span>|<span data-ttu-id="a3018-170">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="a3018-170">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3018-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a3018-171">Relationships</span></span>
<span data-ttu-id="a3018-172">なし</span><span class="sxs-lookup"><span data-stu-id="a3018-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3018-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3018-173">JSON Representation</span></span>
<span data-ttu-id="a3018-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a3018-174">Here is a JSON representation of the resource.</span></span>
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
  "platformType": "String",
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





