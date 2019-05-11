---
title: managedDeviceEncryptionState リソースの種類
description: デバイスごとの暗号化レポート
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6816e8bc0bb71f4f81b3fc213db622d38ed83816
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944937"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="accfd-103">managedDeviceEncryptionState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="accfd-103">managedDeviceEncryptionState resource type</span></span>

> <span data-ttu-id="accfd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="accfd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="accfd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="accfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="accfd-106">デバイスごとの暗号化レポート</span><span class="sxs-lookup"><span data-stu-id="accfd-106">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="accfd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="accfd-107">Methods</span></span>
|<span data-ttu-id="accfd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="accfd-108">Method</span></span>|<span data-ttu-id="accfd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="accfd-109">Return Type</span></span>|<span data-ttu-id="accfd-110">説明</span><span class="sxs-lookup"><span data-stu-id="accfd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="accfd-111">ManagedDeviceEncryptionStates のリスト</span><span class="sxs-lookup"><span data-stu-id="accfd-111">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="accfd-112">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="accfd-112">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="accfd-113">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="accfd-113">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="accfd-114">ManagedDeviceEncryptionState の取得</span><span class="sxs-lookup"><span data-stu-id="accfd-114">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="accfd-115">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="accfd-115">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="accfd-116">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="accfd-116">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="accfd-117">ManagedDeviceEncryptionState の作成</span><span class="sxs-lookup"><span data-stu-id="accfd-117">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="accfd-118">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="accfd-118">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="accfd-119">新しい[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="accfd-119">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="accfd-120">ManagedDeviceEncryptionState の削除</span><span class="sxs-lookup"><span data-stu-id="accfd-120">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="accfd-121">None</span><span class="sxs-lookup"><span data-stu-id="accfd-121">None</span></span>|<span data-ttu-id="accfd-122">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="accfd-122">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="accfd-123">ManagedDeviceEncryptionState の更新</span><span class="sxs-lookup"><span data-stu-id="accfd-123">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="accfd-124">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="accfd-124">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="accfd-125">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="accfd-125">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="accfd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="accfd-126">Properties</span></span>
|<span data-ttu-id="accfd-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="accfd-127">Property</span></span>|<span data-ttu-id="accfd-128">型</span><span class="sxs-lookup"><span data-stu-id="accfd-128">Type</span></span>|<span data-ttu-id="accfd-129">説明</span><span class="sxs-lookup"><span data-stu-id="accfd-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="accfd-130">id</span><span class="sxs-lookup"><span data-stu-id="accfd-130">id</span></span>|<span data-ttu-id="accfd-131">文字列</span><span class="sxs-lookup"><span data-stu-id="accfd-131">String</span></span>|<span data-ttu-id="accfd-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="accfd-132">Key of the entity.</span></span>|
|<span data-ttu-id="accfd-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="accfd-133">userPrincipalName</span></span>|<span data-ttu-id="accfd-134">String</span><span class="sxs-lookup"><span data-stu-id="accfd-134">String</span></span>|<span data-ttu-id="accfd-135">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="accfd-135">User name</span></span>|
|<span data-ttu-id="accfd-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="accfd-136">deviceType</span></span>|[<span data-ttu-id="accfd-137">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="accfd-137">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="accfd-138">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="accfd-138">Platform of the device.</span></span> <span data-ttu-id="accfd-139">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="accfd-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="accfd-140">osVersion</span><span class="sxs-lookup"><span data-stu-id="accfd-140">osVersion</span></span>|<span data-ttu-id="accfd-141">String</span><span class="sxs-lookup"><span data-stu-id="accfd-141">String</span></span>|<span data-ttu-id="accfd-142">デバイスのオペレーティングシステムのバージョン</span><span class="sxs-lookup"><span data-stu-id="accfd-142">Operating system version of the device</span></span>|
|<span data-ttu-id="accfd-143">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="accfd-143">tpmSpecificationVersion</span></span>|<span data-ttu-id="accfd-144">String</span><span class="sxs-lookup"><span data-stu-id="accfd-144">String</span></span>|<span data-ttu-id="accfd-145">デバイス TPM のバージョン</span><span class="sxs-lookup"><span data-stu-id="accfd-145">Device TPM Version</span></span>|
|<span data-ttu-id="accfd-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="accfd-146">deviceName</span></span>|<span data-ttu-id="accfd-147">String</span><span class="sxs-lookup"><span data-stu-id="accfd-147">String</span></span>|<span data-ttu-id="accfd-148">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="accfd-148">Device name</span></span>|
|<span data-ttu-id="accfd-149">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="accfd-149">encryptionReadinessState</span></span>|[<span data-ttu-id="accfd-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="accfd-150">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="accfd-151">暗号化の準備状態。</span><span class="sxs-lookup"><span data-stu-id="accfd-151">Encryption readiness state.</span></span> <span data-ttu-id="accfd-152">可能な値は、`notReady`、`ready` です。</span><span class="sxs-lookup"><span data-stu-id="accfd-152">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="accfd-153">encryptionState</span><span class="sxs-lookup"><span data-stu-id="accfd-153">encryptionState</span></span>|[<span data-ttu-id="accfd-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="accfd-154">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="accfd-155">デバイスの暗号化の状態。</span><span class="sxs-lookup"><span data-stu-id="accfd-155">Device encryption state.</span></span> <span data-ttu-id="accfd-156">可能な値は、`notEncrypted`、`encrypted` です。</span><span class="sxs-lookup"><span data-stu-id="accfd-156">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="accfd-157">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="accfd-157">encryptionPolicySettingState</span></span>|[<span data-ttu-id="accfd-158">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="accfd-158">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="accfd-159">暗号化ポリシーの設定状態。</span><span class="sxs-lookup"><span data-stu-id="accfd-159">Encryption policy setting state.</span></span> <span data-ttu-id="accfd-160">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="accfd-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="accfd-161">Advanced Bitlockerstates</span><span class="sxs-lookup"><span data-stu-id="accfd-161">advancedBitLockerStates</span></span>|[<span data-ttu-id="accfd-162">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="accfd-162">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="accfd-163">高度な BitLocker 状態。</span><span class="sxs-lookup"><span data-stu-id="accfd-163">Advanced BitLocker State.</span></span> <span data-ttu-id="accfd-164">可能な値は`success`、 `noUserConsent`、 `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、です。 `recoveryKeyBackupFailed` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="accfd-164">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="accfd-165">policyDetails</span><span class="sxs-lookup"><span data-stu-id="accfd-165">policyDetails</span></span>|<span data-ttu-id="accfd-166">[Encryptionreportpolicydetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="accfd-166">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="accfd-167">ポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="accfd-167">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="accfd-168">関係</span><span class="sxs-lookup"><span data-stu-id="accfd-168">Relationships</span></span>
<span data-ttu-id="accfd-169">なし</span><span class="sxs-lookup"><span data-stu-id="accfd-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="accfd-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="accfd-170">JSON Representation</span></span>
<span data-ttu-id="accfd-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="accfd-171">Here is a JSON representation of the resource.</span></span>
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




