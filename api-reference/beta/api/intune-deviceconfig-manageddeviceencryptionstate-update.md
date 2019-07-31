---
title: ManagedDeviceEncryptionState の更新
description: ManagedDeviceEncryptionState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: def987033cc6a1ea34159f5de9038d0f2c0ceefb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946614"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="07607-103">ManagedDeviceEncryptionState の更新</span><span class="sxs-lookup"><span data-stu-id="07607-103">Update managedDeviceEncryptionState</span></span>

> <span data-ttu-id="07607-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07607-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07607-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="07607-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07607-106">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="07607-106">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07607-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="07607-107">Prerequisites</span></span>
<span data-ttu-id="07607-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07607-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07607-110">Permission type</span></span>|<span data-ttu-id="07607-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="07607-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07607-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07607-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07607-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07607-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07607-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07607-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07607-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07607-115">Not supported.</span></span>|
|<span data-ttu-id="07607-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07607-116">Application</span></span>|<span data-ttu-id="07607-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07607-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07607-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07607-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="07607-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07607-119">Request headers</span></span>
|<span data-ttu-id="07607-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07607-120">Header</span></span>|<span data-ttu-id="07607-121">値</span><span class="sxs-lookup"><span data-stu-id="07607-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07607-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07607-122">Authorization</span></span>|<span data-ttu-id="07607-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="07607-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07607-124">承諾</span><span class="sxs-lookup"><span data-stu-id="07607-124">Accept</span></span>|<span data-ttu-id="07607-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07607-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07607-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="07607-126">Request body</span></span>
<span data-ttu-id="07607-127">要求本文で、 [Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="07607-127">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="07607-128">次の表に、 [Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="07607-128">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="07607-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07607-129">Property</span></span>|<span data-ttu-id="07607-130">型</span><span class="sxs-lookup"><span data-stu-id="07607-130">Type</span></span>|<span data-ttu-id="07607-131">説明</span><span class="sxs-lookup"><span data-stu-id="07607-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07607-132">id</span><span class="sxs-lookup"><span data-stu-id="07607-132">id</span></span>|<span data-ttu-id="07607-133">文字列</span><span class="sxs-lookup"><span data-stu-id="07607-133">String</span></span>|<span data-ttu-id="07607-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="07607-134">Key of the entity.</span></span>|
|<span data-ttu-id="07607-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="07607-135">userPrincipalName</span></span>|<span data-ttu-id="07607-136">String</span><span class="sxs-lookup"><span data-stu-id="07607-136">String</span></span>|<span data-ttu-id="07607-137">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="07607-137">User name</span></span>|
|<span data-ttu-id="07607-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="07607-138">deviceType</span></span>|[<span data-ttu-id="07607-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="07607-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="07607-140">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="07607-140">Platform of the device.</span></span> <span data-ttu-id="07607-141">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="07607-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="07607-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="07607-142">osVersion</span></span>|<span data-ttu-id="07607-143">String</span><span class="sxs-lookup"><span data-stu-id="07607-143">String</span></span>|<span data-ttu-id="07607-144">デバイスのオペレーティングシステムのバージョン</span><span class="sxs-lookup"><span data-stu-id="07607-144">Operating system version of the device</span></span>|
|<span data-ttu-id="07607-145">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="07607-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="07607-146">String</span><span class="sxs-lookup"><span data-stu-id="07607-146">String</span></span>|<span data-ttu-id="07607-147">デバイス TPM のバージョン</span><span class="sxs-lookup"><span data-stu-id="07607-147">Device TPM Version</span></span>|
|<span data-ttu-id="07607-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="07607-148">deviceName</span></span>|<span data-ttu-id="07607-149">String</span><span class="sxs-lookup"><span data-stu-id="07607-149">String</span></span>|<span data-ttu-id="07607-150">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="07607-150">Device name</span></span>|
|<span data-ttu-id="07607-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="07607-151">encryptionReadinessState</span></span>|[<span data-ttu-id="07607-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="07607-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="07607-153">暗号化の準備状態。</span><span class="sxs-lookup"><span data-stu-id="07607-153">Encryption readiness state.</span></span> <span data-ttu-id="07607-154">可能な値は、`notReady`、`ready` です。</span><span class="sxs-lookup"><span data-stu-id="07607-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="07607-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="07607-155">encryptionState</span></span>|[<span data-ttu-id="07607-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="07607-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="07607-157">デバイスの暗号化の状態。</span><span class="sxs-lookup"><span data-stu-id="07607-157">Device encryption state.</span></span> <span data-ttu-id="07607-158">可能な値は、`notEncrypted`、`encrypted` です。</span><span class="sxs-lookup"><span data-stu-id="07607-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="07607-159">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="07607-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="07607-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="07607-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="07607-161">暗号化ポリシーの設定状態。</span><span class="sxs-lookup"><span data-stu-id="07607-161">Encryption policy setting state.</span></span> <span data-ttu-id="07607-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="07607-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="07607-163">Advanced Bitlockerstates</span><span class="sxs-lookup"><span data-stu-id="07607-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="07607-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="07607-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="07607-165">高度な BitLocker 状態。</span><span class="sxs-lookup"><span data-stu-id="07607-165">Advanced BitLocker State.</span></span> <span data-ttu-id="07607-166">可能な値は`success`、 `noUserConsent`、 `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、です。 `recoveryKeyBackupFailed` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="07607-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="07607-167">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="07607-167">fileVaultStates</span></span>|[<span data-ttu-id="07607-168">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="07607-168">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="07607-169">FileVault の状態です。</span><span class="sxs-lookup"><span data-stu-id="07607-169">FileVault State.</span></span> <span data-ttu-id="07607-170">使用可能な値は、`success`、`driveEncryptedByUser`、`userDeferredEncryption`、`escrowNotEnabled` です。</span><span class="sxs-lookup"><span data-stu-id="07607-170">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="07607-171">policyDetails</span><span class="sxs-lookup"><span data-stu-id="07607-171">policyDetails</span></span>|<span data-ttu-id="07607-172">[Encryptionreportpolicydetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="07607-172">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="07607-173">ポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="07607-173">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="07607-174">応答</span><span class="sxs-lookup"><span data-stu-id="07607-174">Response</span></span>
<span data-ttu-id="07607-175">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="07607-175">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07607-176">例</span><span class="sxs-lookup"><span data-stu-id="07607-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="07607-177">要求</span><span class="sxs-lookup"><span data-stu-id="07607-177">Request</span></span>
<span data-ttu-id="07607-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07607-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
Content-type: application/json
Content-length: 704

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="07607-179">応答</span><span class="sxs-lookup"><span data-stu-id="07607-179">Response</span></span>
<span data-ttu-id="07607-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07607-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```





