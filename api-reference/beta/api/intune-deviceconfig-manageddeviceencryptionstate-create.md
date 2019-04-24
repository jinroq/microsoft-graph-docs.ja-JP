---
title: manageddeviceencryptionstate の作成
description: 新しい manageddeviceencryptionstate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6edba4844d56f1c1f87ff146f547cd4b08699c84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518150"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="0bac1-103">manageddeviceencryptionstate の作成</span><span class="sxs-lookup"><span data-stu-id="0bac1-103">Create managedDeviceEncryptionState</span></span>

> <span data-ttu-id="0bac1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bac1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bac1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0bac1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bac1-106">新しい[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0bac1-106">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bac1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0bac1-107">Prerequisites</span></span>
<span data-ttu-id="0bac1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bac1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bac1-110">Permission type</span></span>|<span data-ttu-id="0bac1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bac1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bac1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bac1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0bac1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bac1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bac1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bac1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bac1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bac1-115">Not supported.</span></span>|
|<span data-ttu-id="0bac1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bac1-116">Application</span></span>|<span data-ttu-id="0bac1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bac1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bac1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bac1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="0bac1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bac1-119">Request headers</span></span>
|<span data-ttu-id="0bac1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bac1-120">Header</span></span>|<span data-ttu-id="0bac1-121">値</span><span class="sxs-lookup"><span data-stu-id="0bac1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bac1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bac1-122">Authorization</span></span>|<span data-ttu-id="0bac1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0bac1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bac1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0bac1-124">Accept</span></span>|<span data-ttu-id="0bac1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0bac1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bac1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bac1-126">Request body</span></span>
<span data-ttu-id="0bac1-127">要求本文で、manageddeviceencryptionstate オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0bac1-127">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="0bac1-128">次の表に、manageddeviceencryptionstate の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0bac1-128">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="0bac1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bac1-129">Property</span></span>|<span data-ttu-id="0bac1-130">型</span><span class="sxs-lookup"><span data-stu-id="0bac1-130">Type</span></span>|<span data-ttu-id="0bac1-131">説明</span><span class="sxs-lookup"><span data-stu-id="0bac1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bac1-132">id</span><span class="sxs-lookup"><span data-stu-id="0bac1-132">id</span></span>|<span data-ttu-id="0bac1-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0bac1-133">String</span></span>|<span data-ttu-id="0bac1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0bac1-134">Key of the entity.</span></span>|
|<span data-ttu-id="0bac1-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0bac1-135">userPrincipalName</span></span>|<span data-ttu-id="0bac1-136">String</span><span class="sxs-lookup"><span data-stu-id="0bac1-136">String</span></span>|<span data-ttu-id="0bac1-137">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="0bac1-137">User name</span></span>|
|<span data-ttu-id="0bac1-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="0bac1-138">deviceType</span></span>|[<span data-ttu-id="0bac1-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="0bac1-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="0bac1-140">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="0bac1-140">Platform of the device.</span></span> <span data-ttu-id="0bac1-141">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0bac1-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="0bac1-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="0bac1-142">osVersion</span></span>|<span data-ttu-id="0bac1-143">String</span><span class="sxs-lookup"><span data-stu-id="0bac1-143">String</span></span>|<span data-ttu-id="0bac1-144">デバイスのオペレーティングシステムのバージョン</span><span class="sxs-lookup"><span data-stu-id="0bac1-144">Operating system version of the device</span></span>|
|<span data-ttu-id="0bac1-145">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="0bac1-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="0bac1-146">String</span><span class="sxs-lookup"><span data-stu-id="0bac1-146">String</span></span>|<span data-ttu-id="0bac1-147">デバイス TPM のバージョン</span><span class="sxs-lookup"><span data-stu-id="0bac1-147">Device TPM Version</span></span>|
|<span data-ttu-id="0bac1-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="0bac1-148">deviceName</span></span>|<span data-ttu-id="0bac1-149">String</span><span class="sxs-lookup"><span data-stu-id="0bac1-149">String</span></span>|<span data-ttu-id="0bac1-150">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="0bac1-150">Device name</span></span>|
|<span data-ttu-id="0bac1-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="0bac1-151">encryptionReadinessState</span></span>|[<span data-ttu-id="0bac1-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="0bac1-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="0bac1-153">暗号化の準備状態。</span><span class="sxs-lookup"><span data-stu-id="0bac1-153">Encryption readiness state.</span></span> <span data-ttu-id="0bac1-154">可能な値は、`notReady`、`ready` です。</span><span class="sxs-lookup"><span data-stu-id="0bac1-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="0bac1-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="0bac1-155">encryptionState</span></span>|[<span data-ttu-id="0bac1-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="0bac1-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="0bac1-157">デバイスの暗号化の状態。</span><span class="sxs-lookup"><span data-stu-id="0bac1-157">Device encryption state.</span></span> <span data-ttu-id="0bac1-158">可能な値は、`notEncrypted`、`encrypted` です。</span><span class="sxs-lookup"><span data-stu-id="0bac1-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="0bac1-159">encryptionpolicysettingstate</span><span class="sxs-lookup"><span data-stu-id="0bac1-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="0bac1-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0bac1-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0bac1-161">暗号化ポリシーの設定状態。</span><span class="sxs-lookup"><span data-stu-id="0bac1-161">Encryption policy setting state.</span></span> <span data-ttu-id="0bac1-162">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="0bac1-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0bac1-163">advanced bitlockerstates</span><span class="sxs-lookup"><span data-stu-id="0bac1-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="0bac1-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="0bac1-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="0bac1-165">高度な BitLocker 状態。</span><span class="sxs-lookup"><span data-stu-id="0bac1-165">Advanced BitLocker State.</span></span> <span data-ttu-id="0bac1-166">可能な値は`success`、 `noUserConsent`、 `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `networkError`、、 `fixedDriveNotEncrypted`、、、、、、、、です。 `recoveryKeyBackupFailed` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady`</span><span class="sxs-lookup"><span data-stu-id="0bac1-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="0bac1-167">policydetails</span><span class="sxs-lookup"><span data-stu-id="0bac1-167">policyDetails</span></span>|<span data-ttu-id="0bac1-168">[encryptionreportpolicydetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0bac1-168">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="0bac1-169">ポリシーの詳細</span><span class="sxs-lookup"><span data-stu-id="0bac1-169">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="0bac1-170">応答</span><span class="sxs-lookup"><span data-stu-id="0bac1-170">Response</span></span>
<span data-ttu-id="0bac1-171">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0bac1-171">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bac1-172">例</span><span class="sxs-lookup"><span data-stu-id="0bac1-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bac1-173">要求</span><span class="sxs-lookup"><span data-stu-id="0bac1-173">Request</span></span>
<span data-ttu-id="0bac1-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0bac1-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
Content-type: application/json
Content-length: 658

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
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="0bac1-175">応答</span><span class="sxs-lookup"><span data-stu-id="0bac1-175">Response</span></span>
<span data-ttu-id="0bac1-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0bac1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 707

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
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```





