---
title: manageddeviceencryptionstate リソースの種類
description: デバイスごとの暗号化レポート
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9193c795f9c488b5f157014c81d00a4b5118d149
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779875"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="6ac99-103">manageddeviceencryptionstate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ac99-103">managedDeviceEncryptionState resource type</span></span>

> <span data-ttu-id="6ac99-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ac99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ac99-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ac99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ac99-106">デバイスごとの暗号化レポート</span><span class="sxs-lookup"><span data-stu-id="6ac99-106">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="6ac99-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ac99-107">Methods</span></span>
|<span data-ttu-id="6ac99-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6ac99-108">Method</span></span>|<span data-ttu-id="6ac99-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6ac99-109">Return Type</span></span>|<span data-ttu-id="6ac99-110">説明</span><span class="sxs-lookup"><span data-stu-id="6ac99-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6ac99-111">manageddeviceencryptionstates のリスト</span><span class="sxs-lookup"><span data-stu-id="6ac99-111">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="6ac99-112">[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6ac99-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="6ac99-113">[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6ac99-113">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="6ac99-114">manageddeviceencryptionstate の取得</span><span class="sxs-lookup"><span data-stu-id="6ac99-114">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="6ac99-115">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6ac99-115">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="6ac99-116">[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6ac99-116">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="6ac99-117">manageddeviceencryptionstate の作成</span><span class="sxs-lookup"><span data-stu-id="6ac99-117">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="6ac99-118">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6ac99-118">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="6ac99-119">新しい[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6ac99-119">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="6ac99-120">manageddeviceencryptionstate の削除</span><span class="sxs-lookup"><span data-stu-id="6ac99-120">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="6ac99-121">なし</span><span class="sxs-lookup"><span data-stu-id="6ac99-121">None</span></span>|<span data-ttu-id="6ac99-122">[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="6ac99-122">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="6ac99-123">manageddeviceencryptionstate の更新</span><span class="sxs-lookup"><span data-stu-id="6ac99-123">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="6ac99-124">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="6ac99-124">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="6ac99-125">[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6ac99-125">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ac99-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ac99-126">Properties</span></span>
|<span data-ttu-id="6ac99-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ac99-127">Property</span></span>|<span data-ttu-id="6ac99-128">型</span><span class="sxs-lookup"><span data-stu-id="6ac99-128">Type</span></span>|<span data-ttu-id="6ac99-129">説明</span><span class="sxs-lookup"><span data-stu-id="6ac99-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ac99-130">id</span><span class="sxs-lookup"><span data-stu-id="6ac99-130">id</span></span>|<span data-ttu-id="6ac99-131">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6ac99-131">String</span></span>|<span data-ttu-id="6ac99-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6ac99-132">Key of the entity.</span></span>|
|<span data-ttu-id="6ac99-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6ac99-133">userPrincipalName</span></span>|<span data-ttu-id="6ac99-134">String</span><span class="sxs-lookup"><span data-stu-id="6ac99-134">String</span></span>|<span data-ttu-id="6ac99-135">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="6ac99-135">User name</span></span>|
|<span data-ttu-id="6ac99-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="6ac99-136">deviceType</span></span>|[<span data-ttu-id="6ac99-137">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="6ac99-137">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="6ac99-138">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="6ac99-138">Platform of the device.</span></span> <span data-ttu-id="6ac99-139">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6ac99-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="6ac99-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="6ac99-140">osVersion</span></span>|<span data-ttu-id="6ac99-141">String</span><span class="sxs-lookup"><span data-stu-id="6ac99-141">String</span></span>|<span data-ttu-id="6ac99-142">デバイスのオペレーティングシステムのバージョン</span><span class="sxs-lookup"><span data-stu-id="6ac99-142">Operating system version of the device</span></span>|
|<span data-ttu-id="6ac99-143">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="6ac99-143">tpmSpecificationVersion</span></span>|<span data-ttu-id="6ac99-144">文字列</span><span class="sxs-lookup"><span data-stu-id="6ac99-144">String</span></span>|<span data-ttu-id="6ac99-145">デバイス TPM のバージョン</span><span class="sxs-lookup"><span data-stu-id="6ac99-145">Device TPM Version</span></span>|
|<span data-ttu-id="6ac99-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="6ac99-146">deviceName</span></span>|<span data-ttu-id="6ac99-147">文字列</span><span class="sxs-lookup"><span data-stu-id="6ac99-147">String</span></span>|<span data-ttu-id="6ac99-148">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="6ac99-148">Device name</span></span>|
|<span data-ttu-id="6ac99-149">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="6ac99-149">encryptionReadinessState</span></span>|[<span data-ttu-id="6ac99-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="6ac99-150">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="6ac99-151">暗号化の準備状態。</span><span class="sxs-lookup"><span data-stu-id="6ac99-151">Encryption readiness state.</span></span> <span data-ttu-id="6ac99-152">可能な値は、`notReady`、`ready` です。</span><span class="sxs-lookup"><span data-stu-id="6ac99-152">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="6ac99-153">encryptionState</span><span class="sxs-lookup"><span data-stu-id="6ac99-153">encryptionState</span></span>|[<span data-ttu-id="6ac99-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="6ac99-154">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="6ac99-155">デバイスの暗号化の状態。</span><span class="sxs-lookup"><span data-stu-id="6ac99-155">Device encryption state.</span></span> <span data-ttu-id="6ac99-156">可能な値は、`notEncrypted`、`encrypted` です。</span><span class="sxs-lookup"><span data-stu-id="6ac99-156">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="6ac99-157">encryptionpolicysettingstate</span><span class="sxs-lookup"><span data-stu-id="6ac99-157">encryptionPolicySettingState</span></span>|[<span data-ttu-id="6ac99-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6ac99-158">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6ac99-159">暗号化ポリシーの設定状態。</span><span class="sxs-lookup"><span data-stu-id="6ac99-159">Encryption policy setting state.</span></span> <span data-ttu-id="6ac99-160">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="6ac99-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6ac99-161">advanced bitlockerstates</span><span class="sxs-lookup"><span data-stu-id="6ac99-161">advancedBitLockerStates</span></span>|[<span data-ttu-id="6ac99-162">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="6ac99-162">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="6ac99-163">高度な BitLocker 状態。</span><span class="sxs-lookup"><span data-stu-id="6ac99-163">Advanced BitLocker State.</span></span> <span data-ttu-id="6ac99-164">可能な値は`success`、 `noUserConsent`、 `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、です。 `recoveryKeyBackupFailed` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="6ac99-164">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="6ac99-165">policydetails</span><span class="sxs-lookup"><span data-stu-id="6ac99-165">policyDetails</span></span>|<span data-ttu-id="6ac99-166">[encryptionreportpolicydetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6ac99-166">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="6ac99-167">ポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="6ac99-167">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ac99-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6ac99-168">Relationships</span></span>
<span data-ttu-id="6ac99-169">なし</span><span class="sxs-lookup"><span data-stu-id="6ac99-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ac99-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ac99-170">JSON Representation</span></span>
<span data-ttu-id="6ac99-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ac99-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "deviceType": "String",
  "osVersion": "String",
  "tpmSpecificationVersion": "String",
  "deviceName": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```





