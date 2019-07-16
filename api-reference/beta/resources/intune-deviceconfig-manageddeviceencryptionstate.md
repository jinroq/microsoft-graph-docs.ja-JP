---
title: managedDeviceEncryptionState リソースの種類
description: デバイスごとの暗号化レポート
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c2c86a843c4573d4c00ae4650d857c3f01ec08d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737497"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="47445-103">managedDeviceEncryptionState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47445-103">managedDeviceEncryptionState resource type</span></span>

> <span data-ttu-id="47445-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47445-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47445-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47445-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47445-106">デバイスごとの暗号化レポート</span><span class="sxs-lookup"><span data-stu-id="47445-106">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="47445-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="47445-107">Methods</span></span>
|<span data-ttu-id="47445-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="47445-108">Method</span></span>|<span data-ttu-id="47445-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="47445-109">Return Type</span></span>|<span data-ttu-id="47445-110">説明</span><span class="sxs-lookup"><span data-stu-id="47445-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47445-111">ManagedDeviceEncryptionStates のリスト</span><span class="sxs-lookup"><span data-stu-id="47445-111">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="47445-112">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="47445-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="47445-113">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="47445-113">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="47445-114">ManagedDeviceEncryptionState の取得</span><span class="sxs-lookup"><span data-stu-id="47445-114">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="47445-115">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="47445-115">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="47445-116">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="47445-116">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="47445-117">ManagedDeviceEncryptionState の作成</span><span class="sxs-lookup"><span data-stu-id="47445-117">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="47445-118">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="47445-118">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="47445-119">新しい[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="47445-119">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="47445-120">ManagedDeviceEncryptionState の削除</span><span class="sxs-lookup"><span data-stu-id="47445-120">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="47445-121">None</span><span class="sxs-lookup"><span data-stu-id="47445-121">None</span></span>|<span data-ttu-id="47445-122">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="47445-122">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="47445-123">ManagedDeviceEncryptionState の更新</span><span class="sxs-lookup"><span data-stu-id="47445-123">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="47445-124">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="47445-124">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="47445-125">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="47445-125">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47445-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47445-126">Properties</span></span>
|<span data-ttu-id="47445-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47445-127">Property</span></span>|<span data-ttu-id="47445-128">型</span><span class="sxs-lookup"><span data-stu-id="47445-128">Type</span></span>|<span data-ttu-id="47445-129">説明</span><span class="sxs-lookup"><span data-stu-id="47445-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47445-130">id</span><span class="sxs-lookup"><span data-stu-id="47445-130">id</span></span>|<span data-ttu-id="47445-131">文字列</span><span class="sxs-lookup"><span data-stu-id="47445-131">String</span></span>|<span data-ttu-id="47445-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="47445-132">Key of the entity.</span></span>|
|<span data-ttu-id="47445-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="47445-133">userPrincipalName</span></span>|<span data-ttu-id="47445-134">String</span><span class="sxs-lookup"><span data-stu-id="47445-134">String</span></span>|<span data-ttu-id="47445-135">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="47445-135">User name</span></span>|
|<span data-ttu-id="47445-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="47445-136">deviceType</span></span>|[<span data-ttu-id="47445-137">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="47445-137">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="47445-138">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="47445-138">Platform of the device.</span></span> <span data-ttu-id="47445-139">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="47445-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="47445-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="47445-140">osVersion</span></span>|<span data-ttu-id="47445-141">String</span><span class="sxs-lookup"><span data-stu-id="47445-141">String</span></span>|<span data-ttu-id="47445-142">デバイスのオペレーティングシステムのバージョン</span><span class="sxs-lookup"><span data-stu-id="47445-142">Operating system version of the device</span></span>|
|<span data-ttu-id="47445-143">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="47445-143">tpmSpecificationVersion</span></span>|<span data-ttu-id="47445-144">String</span><span class="sxs-lookup"><span data-stu-id="47445-144">String</span></span>|<span data-ttu-id="47445-145">デバイス TPM のバージョン</span><span class="sxs-lookup"><span data-stu-id="47445-145">Device TPM Version</span></span>|
|<span data-ttu-id="47445-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="47445-146">deviceName</span></span>|<span data-ttu-id="47445-147">String</span><span class="sxs-lookup"><span data-stu-id="47445-147">String</span></span>|<span data-ttu-id="47445-148">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="47445-148">Device name</span></span>|
|<span data-ttu-id="47445-149">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="47445-149">encryptionReadinessState</span></span>|[<span data-ttu-id="47445-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="47445-150">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="47445-151">暗号化の準備状態。</span><span class="sxs-lookup"><span data-stu-id="47445-151">Encryption readiness state.</span></span> <span data-ttu-id="47445-152">可能な値は、`notReady`、`ready` です。</span><span class="sxs-lookup"><span data-stu-id="47445-152">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="47445-153">encryptionState</span><span class="sxs-lookup"><span data-stu-id="47445-153">encryptionState</span></span>|[<span data-ttu-id="47445-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="47445-154">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="47445-155">デバイスの暗号化の状態。</span><span class="sxs-lookup"><span data-stu-id="47445-155">Device encryption state.</span></span> <span data-ttu-id="47445-156">可能な値は、`notEncrypted`、`encrypted` です。</span><span class="sxs-lookup"><span data-stu-id="47445-156">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="47445-157">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="47445-157">encryptionPolicySettingState</span></span>|[<span data-ttu-id="47445-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="47445-158">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="47445-159">暗号化ポリシーの設定状態。</span><span class="sxs-lookup"><span data-stu-id="47445-159">Encryption policy setting state.</span></span> <span data-ttu-id="47445-160">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="47445-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="47445-161">Advanced Bitlockerstates</span><span class="sxs-lookup"><span data-stu-id="47445-161">advancedBitLockerStates</span></span>|[<span data-ttu-id="47445-162">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="47445-162">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="47445-163">高度な BitLocker 状態。</span><span class="sxs-lookup"><span data-stu-id="47445-163">Advanced BitLocker State.</span></span> <span data-ttu-id="47445-164">可能な値は`success`、 `noUserConsent`、 `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、です。 `recoveryKeyBackupFailed` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="47445-164">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="47445-165">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="47445-165">fileVaultStates</span></span>|[<span data-ttu-id="47445-166">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="47445-166">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="47445-167">FileVault の状態です。</span><span class="sxs-lookup"><span data-stu-id="47445-167">FileVault State.</span></span> <span data-ttu-id="47445-168">使用可能な値は、`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled` です。</span><span class="sxs-lookup"><span data-stu-id="47445-168">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="47445-169">policyDetails</span><span class="sxs-lookup"><span data-stu-id="47445-169">policyDetails</span></span>|<span data-ttu-id="47445-170">[Encryptionreportpolicydetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="47445-170">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="47445-171">ポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="47445-171">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="47445-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47445-172">Relationships</span></span>
<span data-ttu-id="47445-173">なし</span><span class="sxs-lookup"><span data-stu-id="47445-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47445-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47445-174">JSON Representation</span></span>
<span data-ttu-id="47445-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47445-175">Here is a JSON representation of the resource.</span></span>
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
  "fileVaultStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```





