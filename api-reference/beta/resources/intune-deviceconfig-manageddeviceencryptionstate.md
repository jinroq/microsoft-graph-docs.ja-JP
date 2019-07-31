---
title: managedDeviceEncryptionState リソースの種類
description: デバイスごとの暗号化レポート
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb212599c56410b7f66d6f8baa8db1d06d36ba60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000882"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="62087-103">managedDeviceEncryptionState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62087-103">managedDeviceEncryptionState resource type</span></span>

> <span data-ttu-id="62087-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62087-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62087-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62087-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62087-106">デバイスごとの暗号化レポート</span><span class="sxs-lookup"><span data-stu-id="62087-106">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="62087-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="62087-107">Methods</span></span>
|<span data-ttu-id="62087-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="62087-108">Method</span></span>|<span data-ttu-id="62087-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="62087-109">Return Type</span></span>|<span data-ttu-id="62087-110">説明</span><span class="sxs-lookup"><span data-stu-id="62087-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62087-111">ManagedDeviceEncryptionStates のリスト</span><span class="sxs-lookup"><span data-stu-id="62087-111">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="62087-112">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62087-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="62087-113">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="62087-113">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="62087-114">ManagedDeviceEncryptionState の取得</span><span class="sxs-lookup"><span data-stu-id="62087-114">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="62087-115">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="62087-115">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="62087-116">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="62087-116">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="62087-117">ManagedDeviceEncryptionState の作成</span><span class="sxs-lookup"><span data-stu-id="62087-117">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="62087-118">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="62087-118">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="62087-119">新しい[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="62087-119">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="62087-120">ManagedDeviceEncryptionState の削除</span><span class="sxs-lookup"><span data-stu-id="62087-120">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="62087-121">None</span><span class="sxs-lookup"><span data-stu-id="62087-121">None</span></span>|<span data-ttu-id="62087-122">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="62087-122">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="62087-123">ManagedDeviceEncryptionState の更新</span><span class="sxs-lookup"><span data-stu-id="62087-123">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="62087-124">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="62087-124">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="62087-125">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="62087-125">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="62087-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62087-126">Properties</span></span>
|<span data-ttu-id="62087-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62087-127">Property</span></span>|<span data-ttu-id="62087-128">型</span><span class="sxs-lookup"><span data-stu-id="62087-128">Type</span></span>|<span data-ttu-id="62087-129">説明</span><span class="sxs-lookup"><span data-stu-id="62087-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62087-130">id</span><span class="sxs-lookup"><span data-stu-id="62087-130">id</span></span>|<span data-ttu-id="62087-131">文字列</span><span class="sxs-lookup"><span data-stu-id="62087-131">String</span></span>|<span data-ttu-id="62087-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="62087-132">Key of the entity.</span></span>|
|<span data-ttu-id="62087-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62087-133">userPrincipalName</span></span>|<span data-ttu-id="62087-134">String</span><span class="sxs-lookup"><span data-stu-id="62087-134">String</span></span>|<span data-ttu-id="62087-135">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="62087-135">User name</span></span>|
|<span data-ttu-id="62087-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="62087-136">deviceType</span></span>|[<span data-ttu-id="62087-137">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="62087-137">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="62087-138">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="62087-138">Platform of the device.</span></span> <span data-ttu-id="62087-139">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="62087-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="62087-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="62087-140">osVersion</span></span>|<span data-ttu-id="62087-141">String</span><span class="sxs-lookup"><span data-stu-id="62087-141">String</span></span>|<span data-ttu-id="62087-142">デバイスのオペレーティングシステムのバージョン</span><span class="sxs-lookup"><span data-stu-id="62087-142">Operating system version of the device</span></span>|
|<span data-ttu-id="62087-143">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="62087-143">tpmSpecificationVersion</span></span>|<span data-ttu-id="62087-144">String</span><span class="sxs-lookup"><span data-stu-id="62087-144">String</span></span>|<span data-ttu-id="62087-145">デバイス TPM のバージョン</span><span class="sxs-lookup"><span data-stu-id="62087-145">Device TPM Version</span></span>|
|<span data-ttu-id="62087-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="62087-146">deviceName</span></span>|<span data-ttu-id="62087-147">String</span><span class="sxs-lookup"><span data-stu-id="62087-147">String</span></span>|<span data-ttu-id="62087-148">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="62087-148">Device name</span></span>|
|<span data-ttu-id="62087-149">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="62087-149">encryptionReadinessState</span></span>|[<span data-ttu-id="62087-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="62087-150">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="62087-151">暗号化の準備状態。</span><span class="sxs-lookup"><span data-stu-id="62087-151">Encryption readiness state.</span></span> <span data-ttu-id="62087-152">可能な値は、`notReady`、`ready` です。</span><span class="sxs-lookup"><span data-stu-id="62087-152">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="62087-153">encryptionState</span><span class="sxs-lookup"><span data-stu-id="62087-153">encryptionState</span></span>|[<span data-ttu-id="62087-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="62087-154">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="62087-155">デバイスの暗号化の状態。</span><span class="sxs-lookup"><span data-stu-id="62087-155">Device encryption state.</span></span> <span data-ttu-id="62087-156">可能な値は、`notEncrypted`、`encrypted` です。</span><span class="sxs-lookup"><span data-stu-id="62087-156">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="62087-157">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="62087-157">encryptionPolicySettingState</span></span>|[<span data-ttu-id="62087-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="62087-158">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="62087-159">暗号化ポリシーの設定状態。</span><span class="sxs-lookup"><span data-stu-id="62087-159">Encryption policy setting state.</span></span> <span data-ttu-id="62087-160">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="62087-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="62087-161">Advanced Bitlockerstates</span><span class="sxs-lookup"><span data-stu-id="62087-161">advancedBitLockerStates</span></span>|[<span data-ttu-id="62087-162">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="62087-162">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="62087-163">高度な BitLocker 状態。</span><span class="sxs-lookup"><span data-stu-id="62087-163">Advanced BitLocker State.</span></span> <span data-ttu-id="62087-164">可能な値は`success`、 `noUserConsent`、 `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、です。 `recoveryKeyBackupFailed` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="62087-164">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="62087-165">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="62087-165">fileVaultStates</span></span>|[<span data-ttu-id="62087-166">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="62087-166">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="62087-167">FileVault の状態です。</span><span class="sxs-lookup"><span data-stu-id="62087-167">FileVault State.</span></span> <span data-ttu-id="62087-168">使用可能な値は、`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled` です。</span><span class="sxs-lookup"><span data-stu-id="62087-168">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="62087-169">policyDetails</span><span class="sxs-lookup"><span data-stu-id="62087-169">policyDetails</span></span>|<span data-ttu-id="62087-170">[Encryptionreportpolicydetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62087-170">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="62087-171">ポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="62087-171">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="62087-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="62087-172">Relationships</span></span>
<span data-ttu-id="62087-173">なし</span><span class="sxs-lookup"><span data-stu-id="62087-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62087-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62087-174">JSON Representation</span></span>
<span data-ttu-id="62087-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="62087-175">Here is a JSON representation of the resource.</span></span>
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





