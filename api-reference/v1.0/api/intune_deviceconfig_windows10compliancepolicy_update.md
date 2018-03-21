# <a name="update-windows10compliancepolicy"></a><span data-ttu-id="bfdb5-101">windows10CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="bfdb5-101">Update windows10CompliancePolicy</span></span>

> <span data-ttu-id="bfdb5-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfdb5-103">[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bfdb5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="bfdb5-104">Prerequisites</span></span>
<span data-ttu-id="bfdb5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bfdb5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bfdb5-107">Permission type</span></span>|<span data-ttu-id="bfdb5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bfdb5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfdb5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bfdb5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bfdb5-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfdb5-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bfdb5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bfdb5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfdb5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-112">Not supported.</span></span>|
|<span data-ttu-id="bfdb5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bfdb5-113">Application</span></span>|<span data-ttu-id="bfdb5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfdb5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bfdb5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="bfdb5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bfdb5-116">Request headers</span></span>
|<span data-ttu-id="bfdb5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bfdb5-117">Header</span></span>|<span data-ttu-id="bfdb5-118">値</span><span class="sxs-lookup"><span data-stu-id="bfdb5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfdb5-119">承認</span><span class="sxs-lookup"><span data-stu-id="bfdb5-119">Authorization</span></span>|<span data-ttu-id="bfdb5-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bfdb5-121">承諾</span><span class="sxs-lookup"><span data-stu-id="bfdb5-121">Accept</span></span>|<span data-ttu-id="bfdb5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bfdb5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfdb5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="bfdb5-123">Request body</span></span>
<span data-ttu-id="bfdb5-124">要求本文で、[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>

<span data-ttu-id="bfdb5-125">次の表に、[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="bfdb5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfdb5-126">Property</span></span>|<span data-ttu-id="bfdb5-127">型</span><span class="sxs-lookup"><span data-stu-id="bfdb5-127">Type</span></span>|<span data-ttu-id="bfdb5-128">説明</span><span class="sxs-lookup"><span data-stu-id="bfdb5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfdb5-129">id</span><span class="sxs-lookup"><span data-stu-id="bfdb5-129">id</span></span>|<span data-ttu-id="bfdb5-130">String</span><span class="sxs-lookup"><span data-stu-id="bfdb5-130">String</span></span>|<span data-ttu-id="bfdb5-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-131">Name of the entity.</span></span> <span data-ttu-id="bfdb5-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bfdb5-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bfdb5-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfdb5-133">createdDateTime</span></span>|<span data-ttu-id="bfdb5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfdb5-134">DateTimeOffset</span></span>|<span data-ttu-id="bfdb5-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-135">DateTime the object was created.</span></span> <span data-ttu-id="bfdb5-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bfdb5-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bfdb5-137">description</span><span class="sxs-lookup"><span data-stu-id="bfdb5-137">description</span></span>|<span data-ttu-id="bfdb5-138">String</span><span class="sxs-lookup"><span data-stu-id="bfdb5-138">String</span></span>|<span data-ttu-id="bfdb5-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bfdb5-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bfdb5-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bfdb5-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfdb5-141">lastModifiedDateTime</span></span>|<span data-ttu-id="bfdb5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfdb5-142">DateTimeOffset</span></span>|<span data-ttu-id="bfdb5-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-143">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="bfdb5-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bfdb5-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bfdb5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bfdb5-145">displayName</span></span>|<span data-ttu-id="bfdb5-146">String</span><span class="sxs-lookup"><span data-stu-id="bfdb5-146">String</span></span>|<span data-ttu-id="bfdb5-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bfdb5-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bfdb5-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bfdb5-149">version</span><span class="sxs-lookup"><span data-stu-id="bfdb5-149">version</span></span>|<span data-ttu-id="bfdb5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdb5-150">Int32</span></span>|<span data-ttu-id="bfdb5-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-151">Version of the device configuration.</span></span> <span data-ttu-id="bfdb5-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bfdb5-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="bfdb5-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="bfdb5-153">passwordRequired</span></span>|<span data-ttu-id="bfdb5-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-154">Boolean</span></span>|<span data-ttu-id="bfdb5-155">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="bfdb5-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bfdb5-156">passwordBlockSimple</span></span>|<span data-ttu-id="bfdb5-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-157">Boolean</span></span>|<span data-ttu-id="bfdb5-158">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="bfdb5-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="bfdb5-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="bfdb5-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-160">Boolean</span></span>|<span data-ttu-id="bfdb5-161">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="bfdb5-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bfdb5-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bfdb5-163">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdb5-163">Int32</span></span>|<span data-ttu-id="bfdb5-164">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="bfdb5-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bfdb5-165">passwordExpirationDays</span></span>|<span data-ttu-id="bfdb5-166">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdb5-166">Int32</span></span>|<span data-ttu-id="bfdb5-167">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-167">The password expiration in days.</span></span>|
|<span data-ttu-id="bfdb5-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bfdb5-168">passwordMinimumLength</span></span>|<span data-ttu-id="bfdb5-169">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdb5-169">Int32</span></span>|<span data-ttu-id="bfdb5-170">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-170">The minimum password length.</span></span>|
|<span data-ttu-id="bfdb5-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bfdb5-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="bfdb5-172">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdb5-172">Int32</span></span>|<span data-ttu-id="bfdb5-173">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="bfdb5-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="bfdb5-174">passwordRequiredType</span></span>|<span data-ttu-id="bfdb5-175">String</span><span class="sxs-lookup"><span data-stu-id="bfdb5-175">String</span></span>|<span data-ttu-id="bfdb5-176">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-176">The required password type.</span></span> <span data-ttu-id="bfdb5-177">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bfdb5-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="bfdb5-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="bfdb5-179">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdb5-179">Int32</span></span>|<span data-ttu-id="bfdb5-180">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="bfdb5-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="bfdb5-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="bfdb5-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-182">Boolean</span></span>|<span data-ttu-id="bfdb5-183">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="bfdb5-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bfdb5-184">osMinimumVersion</span></span>|<span data-ttu-id="bfdb5-185">String</span><span class="sxs-lookup"><span data-stu-id="bfdb5-185">String</span></span>|<span data-ttu-id="bfdb5-186">Windows 10 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="bfdb5-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bfdb5-187">osMaximumVersion</span></span>|<span data-ttu-id="bfdb5-188">String</span><span class="sxs-lookup"><span data-stu-id="bfdb5-188">String</span></span>|<span data-ttu-id="bfdb5-189">Windows 10 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="bfdb5-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="bfdb5-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="bfdb5-191">String</span><span class="sxs-lookup"><span data-stu-id="bfdb5-191">String</span></span>|<span data-ttu-id="bfdb5-192">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="bfdb5-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="bfdb5-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="bfdb5-194">String</span><span class="sxs-lookup"><span data-stu-id="bfdb5-194">String</span></span>|<span data-ttu-id="bfdb5-195">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="bfdb5-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="bfdb5-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="bfdb5-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-197">Boolean</span></span>|<span data-ttu-id="bfdb5-198">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="bfdb5-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="bfdb5-199">bitLockerEnabled</span></span>|<span data-ttu-id="bfdb5-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-200">Boolean</span></span>|<span data-ttu-id="bfdb5-201">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="bfdb5-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="bfdb5-202">secureBootEnabled</span></span>|<span data-ttu-id="bfdb5-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-203">Boolean</span></span>|<span data-ttu-id="bfdb5-204">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="bfdb5-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="bfdb5-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="bfdb5-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-206">Boolean</span></span>|<span data-ttu-id="bfdb5-207">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="bfdb5-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="bfdb5-208">storageRequireEncryption</span></span>|<span data-ttu-id="bfdb5-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdb5-209">Boolean</span></span>|<span data-ttu-id="bfdb5-210">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="bfdb5-211">応答</span><span class="sxs-lookup"><span data-stu-id="bfdb5-211">Response</span></span>
<span data-ttu-id="bfdb5-212">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-212">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfdb5-213">例</span><span class="sxs-lookup"><span data-stu-id="bfdb5-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="bfdb5-214">要求</span><span class="sxs-lookup"><span data-stu-id="bfdb5-214">Request</span></span>
<span data-ttu-id="bfdb5-215">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 954

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="bfdb5-216">応答</span><span class="sxs-lookup"><span data-stu-id="bfdb5-216">Response</span></span>
<span data-ttu-id="bfdb5-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bfdb5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



