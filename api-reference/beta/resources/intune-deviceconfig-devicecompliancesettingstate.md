---
title: deviceComplianceSettingState リソース タイプ
description: 特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22fe0611d4ad583200032b8721076184f168d3c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565815"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="43250-103">deviceComplianceSettingState リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="43250-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="43250-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43250-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43250-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43250-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43250-106">特定のデバイスに関する、デバイスのコンプライアンスの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="43250-106">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="43250-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="43250-107">Methods</span></span>
|<span data-ttu-id="43250-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="43250-108">Method</span></span>|<span data-ttu-id="43250-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="43250-109">Return Type</span></span>|<span data-ttu-id="43250-110">説明</span><span class="sxs-lookup"><span data-stu-id="43250-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="43250-111">List deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="43250-111">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="43250-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="43250-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="43250-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="43250-113">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="43250-114">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="43250-114">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="43250-115">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="43250-115">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="43250-116">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="43250-116">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="43250-117">Create deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="43250-117">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="43250-118">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="43250-118">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="43250-119">新しい [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="43250-119">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="43250-120">Delete deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="43250-120">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="43250-121">なし</span><span class="sxs-lookup"><span data-stu-id="43250-121">None</span></span>|<span data-ttu-id="43250-122">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="43250-122">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="43250-123">Update deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="43250-123">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="43250-124">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="43250-124">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="43250-125">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="43250-125">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="43250-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43250-126">Properties</span></span>
|<span data-ttu-id="43250-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43250-127">Property</span></span>|<span data-ttu-id="43250-128">型</span><span class="sxs-lookup"><span data-stu-id="43250-128">Type</span></span>|<span data-ttu-id="43250-129">説明</span><span class="sxs-lookup"><span data-stu-id="43250-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43250-130">id</span><span class="sxs-lookup"><span data-stu-id="43250-130">id</span></span>|<span data-ttu-id="43250-131">String</span><span class="sxs-lookup"><span data-stu-id="43250-131">String</span></span>|<span data-ttu-id="43250-132">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="43250-132">Key of the entity</span></span>|
|<span data-ttu-id="43250-133">platformType</span><span class="sxs-lookup"><span data-stu-id="43250-133">platformType</span></span>|[<span data-ttu-id="43250-134">deviceType</span><span class="sxs-lookup"><span data-stu-id="43250-134">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="43250-135">デバイスプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="43250-135">Device platform type.</span></span> <span data-ttu-id="43250-136">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="43250-136">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="43250-137">setting</span><span class="sxs-lookup"><span data-stu-id="43250-137">setting</span></span>|<span data-ttu-id="43250-138">String</span><span class="sxs-lookup"><span data-stu-id="43250-138">String</span></span>|<span data-ttu-id="43250-139">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="43250-139">The setting class name and property name.</span></span>|
|<span data-ttu-id="43250-140">settingName</span><span class="sxs-lookup"><span data-stu-id="43250-140">settingName</span></span>|<span data-ttu-id="43250-141">String</span><span class="sxs-lookup"><span data-stu-id="43250-141">String</span></span>|<span data-ttu-id="43250-142">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="43250-142">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="43250-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="43250-143">deviceId</span></span>|<span data-ttu-id="43250-144">String</span><span class="sxs-lookup"><span data-stu-id="43250-144">String</span></span>|<span data-ttu-id="43250-145">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="43250-145">The Device Id that is being reported</span></span>|
|<span data-ttu-id="43250-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="43250-146">deviceName</span></span>|<span data-ttu-id="43250-147">String</span><span class="sxs-lookup"><span data-stu-id="43250-147">String</span></span>|<span data-ttu-id="43250-148">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="43250-148">The Device Name that is being reported</span></span>|
|<span data-ttu-id="43250-149">userId</span><span class="sxs-lookup"><span data-stu-id="43250-149">userId</span></span>|<span data-ttu-id="43250-150">String</span><span class="sxs-lookup"><span data-stu-id="43250-150">String</span></span>|<span data-ttu-id="43250-151">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="43250-151">The user Id that is being reported</span></span>|
|<span data-ttu-id="43250-152">userEmail</span><span class="sxs-lookup"><span data-stu-id="43250-152">userEmail</span></span>|<span data-ttu-id="43250-153">String</span><span class="sxs-lookup"><span data-stu-id="43250-153">String</span></span>|<span data-ttu-id="43250-154">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="43250-154">The User email address that is being reported</span></span>|
|<span data-ttu-id="43250-155">userName</span><span class="sxs-lookup"><span data-stu-id="43250-155">userName</span></span>|<span data-ttu-id="43250-156">String</span><span class="sxs-lookup"><span data-stu-id="43250-156">String</span></span>|<span data-ttu-id="43250-157">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="43250-157">The User Name that is being reported</span></span>|
|<span data-ttu-id="43250-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43250-158">userPrincipalName</span></span>|<span data-ttu-id="43250-159">String</span><span class="sxs-lookup"><span data-stu-id="43250-159">String</span></span>|<span data-ttu-id="43250-160">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="43250-160">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="43250-161">deviceModel</span><span class="sxs-lookup"><span data-stu-id="43250-161">deviceModel</span></span>|<span data-ttu-id="43250-162">String</span><span class="sxs-lookup"><span data-stu-id="43250-162">String</span></span>|<span data-ttu-id="43250-163">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="43250-163">The device model that is being reported</span></span>|
|<span data-ttu-id="43250-164">state</span><span class="sxs-lookup"><span data-stu-id="43250-164">state</span></span>|[<span data-ttu-id="43250-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="43250-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="43250-166">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="43250-166">The compliance state of the setting.</span></span> <span data-ttu-id="43250-167">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="43250-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="43250-168">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="43250-168">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="43250-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43250-169">DateTimeOffset</span></span>|<span data-ttu-id="43250-170">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="43250-170">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="43250-171">関係</span><span class="sxs-lookup"><span data-stu-id="43250-171">Relationships</span></span>
<span data-ttu-id="43250-172">なし</span><span class="sxs-lookup"><span data-stu-id="43250-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43250-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43250-173">JSON Representation</span></span>
<span data-ttu-id="43250-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43250-174">Here is a JSON representation of the resource.</span></span>
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





