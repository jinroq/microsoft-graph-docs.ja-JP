---
title: windows10MobileCompliancePolicy の更新
description: windows10MobileCompliancePolicy オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 696b5c0cb2e51b4f49c656e876940323151e5cba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326237"
---
# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="44a06-103">windows10MobileCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="44a06-103">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="44a06-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="44a06-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44a06-105">[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="44a06-105">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44a06-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="44a06-106">Prerequisites</span></span>
<span data-ttu-id="44a06-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44a06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44a06-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44a06-109">Permission type</span></span>|<span data-ttu-id="44a06-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="44a06-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44a06-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44a06-111">Delegated (work or school account)</span></span>|<span data-ttu-id="44a06-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a06-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44a06-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44a06-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44a06-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44a06-114">Not supported.</span></span>|
|<span data-ttu-id="44a06-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44a06-115">Application</span></span>|<span data-ttu-id="44a06-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44a06-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44a06-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44a06-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="44a06-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44a06-118">Request headers</span></span>
|<span data-ttu-id="44a06-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44a06-119">Header</span></span>|<span data-ttu-id="44a06-120">値</span><span class="sxs-lookup"><span data-stu-id="44a06-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44a06-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44a06-121">Authorization</span></span>|<span data-ttu-id="44a06-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="44a06-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44a06-123">Accept</span><span class="sxs-lookup"><span data-stu-id="44a06-123">Accept</span></span>|<span data-ttu-id="44a06-124">application/json</span><span class="sxs-lookup"><span data-stu-id="44a06-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44a06-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="44a06-125">Request body</span></span>
<span data-ttu-id="44a06-126">要求本文で、[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="44a06-126">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="44a06-127">次の表に、[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="44a06-127">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="44a06-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44a06-128">Property</span></span>|<span data-ttu-id="44a06-129">種類</span><span class="sxs-lookup"><span data-stu-id="44a06-129">Type</span></span>|<span data-ttu-id="44a06-130">説明</span><span class="sxs-lookup"><span data-stu-id="44a06-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44a06-131">ID</span><span class="sxs-lookup"><span data-stu-id="44a06-131">id</span></span>|<span data-ttu-id="44a06-132">String</span><span class="sxs-lookup"><span data-stu-id="44a06-132">String</span></span>|<span data-ttu-id="44a06-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="44a06-133">Key of the entity.</span></span> <span data-ttu-id="44a06-134">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44a06-134">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44a06-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44a06-135">createdDateTime</span></span>|<span data-ttu-id="44a06-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44a06-136">DateTimeOffset</span></span>|<span data-ttu-id="44a06-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="44a06-137">DateTime the object was created.</span></span> <span data-ttu-id="44a06-138">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44a06-138">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44a06-139">説明</span><span class="sxs-lookup"><span data-stu-id="44a06-139">description</span></span>|<span data-ttu-id="44a06-140">String</span><span class="sxs-lookup"><span data-stu-id="44a06-140">String</span></span>|<span data-ttu-id="44a06-141">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="44a06-141">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44a06-142">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44a06-142">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44a06-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44a06-143">lastModifiedDateTime</span></span>|<span data-ttu-id="44a06-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44a06-144">DateTimeOffset</span></span>|<span data-ttu-id="44a06-145">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="44a06-145">DateTime the object was last modified.</span></span> <span data-ttu-id="44a06-146">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44a06-146">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44a06-147">displayName</span><span class="sxs-lookup"><span data-stu-id="44a06-147">displayName</span></span>|<span data-ttu-id="44a06-148">String</span><span class="sxs-lookup"><span data-stu-id="44a06-148">String</span></span>|<span data-ttu-id="44a06-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="44a06-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44a06-150">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44a06-150">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44a06-151">version</span><span class="sxs-lookup"><span data-stu-id="44a06-151">version</span></span>|<span data-ttu-id="44a06-152">Int32</span><span class="sxs-lookup"><span data-stu-id="44a06-152">Int32</span></span>|<span data-ttu-id="44a06-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="44a06-153">Version of the device configuration.</span></span> <span data-ttu-id="44a06-154">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="44a06-154">Inherited from [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="44a06-155">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="44a06-155">passwordRequired</span></span>|<span data-ttu-id="44a06-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="44a06-156">Boolean</span></span>|<span data-ttu-id="44a06-157">Windows Phone デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="44a06-157">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="44a06-158">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="44a06-158">passwordBlockSimple</span></span>|<span data-ttu-id="44a06-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="44a06-159">Boolean</span></span>|<span data-ttu-id="44a06-160">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="44a06-160">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="44a06-161">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="44a06-161">passwordMinimumLength</span></span>|<span data-ttu-id="44a06-162">Int32</span><span class="sxs-lookup"><span data-stu-id="44a06-162">Int32</span></span>|<span data-ttu-id="44a06-163">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="44a06-163">Minimum password length.</span></span> <span data-ttu-id="44a06-164">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="44a06-164">Valid values 4 to 16</span></span>|
|<span data-ttu-id="44a06-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="44a06-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="44a06-166">Int32</span><span class="sxs-lookup"><span data-stu-id="44a06-166">Int32</span></span>|<span data-ttu-id="44a06-167">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="44a06-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="44a06-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="44a06-168">passwordRequiredType</span></span>|[<span data-ttu-id="44a06-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="44a06-169">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="44a06-170">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="44a06-170">The required password type.</span></span> <span data-ttu-id="44a06-171">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="44a06-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="44a06-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="44a06-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="44a06-173">Int32</span><span class="sxs-lookup"><span data-stu-id="44a06-173">Int32</span></span>|<span data-ttu-id="44a06-174">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="44a06-174">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="44a06-175">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="44a06-175">passwordExpirationDays</span></span>|<span data-ttu-id="44a06-176">Int32</span><span class="sxs-lookup"><span data-stu-id="44a06-176">Int32</span></span>|<span data-ttu-id="44a06-177">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="44a06-177">Number of days before password expiration.</span></span> <span data-ttu-id="44a06-178">有効な値は 1 から 255 までです</span><span class="sxs-lookup"><span data-stu-id="44a06-178">Valid values 1 to 255</span></span>|
|<span data-ttu-id="44a06-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="44a06-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="44a06-180">Int32</span><span class="sxs-lookup"><span data-stu-id="44a06-180">Int32</span></span>|<span data-ttu-id="44a06-181">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="44a06-181">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="44a06-182">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="44a06-182">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="44a06-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="44a06-183">Boolean</span></span>|<span data-ttu-id="44a06-184">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="44a06-184">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="44a06-185">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="44a06-185">osMinimumVersion</span></span>|<span data-ttu-id="44a06-186">String</span><span class="sxs-lookup"><span data-stu-id="44a06-186">String</span></span>|<span data-ttu-id="44a06-187">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="44a06-187">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="44a06-188">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="44a06-188">osMaximumVersion</span></span>|<span data-ttu-id="44a06-189">String</span><span class="sxs-lookup"><span data-stu-id="44a06-189">String</span></span>|<span data-ttu-id="44a06-190">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="44a06-190">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="44a06-191">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="44a06-191">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="44a06-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="44a06-192">Boolean</span></span>|<span data-ttu-id="44a06-193">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="44a06-193">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="44a06-194">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="44a06-194">bitLockerEnabled</span></span>|<span data-ttu-id="44a06-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="44a06-195">Boolean</span></span>|<span data-ttu-id="44a06-196">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="44a06-196">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="44a06-197">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="44a06-197">secureBootEnabled</span></span>|<span data-ttu-id="44a06-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="44a06-198">Boolean</span></span>|<span data-ttu-id="44a06-199">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="44a06-199">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="44a06-200">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="44a06-200">codeIntegrityEnabled</span></span>|<span data-ttu-id="44a06-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="44a06-201">Boolean</span></span>|<span data-ttu-id="44a06-202">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="44a06-202">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="44a06-203">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="44a06-203">storageRequireEncryption</span></span>|<span data-ttu-id="44a06-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="44a06-204">Boolean</span></span>|<span data-ttu-id="44a06-205">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="44a06-205">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="44a06-206">応答</span><span class="sxs-lookup"><span data-stu-id="44a06-206">Response</span></span>
<span data-ttu-id="44a06-207">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="44a06-207">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44a06-208">例</span><span class="sxs-lookup"><span data-stu-id="44a06-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="44a06-209">要求</span><span class="sxs-lookup"><span data-stu-id="44a06-209">Request</span></span>
<span data-ttu-id="44a06-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44a06-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="44a06-211">応答</span><span class="sxs-lookup"><span data-stu-id="44a06-211">Response</span></span>
<span data-ttu-id="44a06-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44a06-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
  "id": "3d4237b0-37b0-3d42-b037-423db037423d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordExpirationDays": 6,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordRequireToUnlockFromIdle": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```


