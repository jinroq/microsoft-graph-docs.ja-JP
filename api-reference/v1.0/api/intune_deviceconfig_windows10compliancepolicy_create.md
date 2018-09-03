# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="79cb1-101">windows10CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="79cb1-101">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="79cb1-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79cb1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79cb1-103">新しい [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-103">Create a new [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79cb1-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="79cb1-104">Prerequisites</span></span>
<span data-ttu-id="79cb1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79cb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79cb1-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79cb1-107">Permission type</span></span>|<span data-ttu-id="79cb1-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79cb1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79cb1-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79cb1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="79cb1-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79cb1-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79cb1-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79cb1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79cb1-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79cb1-112">Not supported.</span></span>|
|<span data-ttu-id="79cb1-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79cb1-113">Application</span></span>|<span data-ttu-id="79cb1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79cb1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79cb1-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79cb1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="79cb1-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79cb1-116">Request headers</span></span>
|<span data-ttu-id="79cb1-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79cb1-117">Header</span></span>|<span data-ttu-id="79cb1-118">値</span><span class="sxs-lookup"><span data-stu-id="79cb1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79cb1-119">承認</span><span class="sxs-lookup"><span data-stu-id="79cb1-119">Authorization</span></span>|<span data-ttu-id="79cb1-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="79cb1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79cb1-121">承諾</span><span class="sxs-lookup"><span data-stu-id="79cb1-121">Accept</span></span>|<span data-ttu-id="79cb1-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="79cb1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79cb1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="79cb1-123">Request body</span></span>
<span data-ttu-id="79cb1-124">要求本文で、windows10CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-124">In the request body, supply a JSON representation for the windows10CompliancePolicy object.</span></span>

<span data-ttu-id="79cb1-125">次の表に、windows10CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-125">The following table shows the properties that are required when you create the windows10CompliancePolicy.</span></span>

|<span data-ttu-id="79cb1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79cb1-126">Property</span></span>|<span data-ttu-id="79cb1-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="79cb1-127">Type</span></span>|<span data-ttu-id="79cb1-128">説明</span><span class="sxs-lookup"><span data-stu-id="79cb1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79cb1-129">ID</span><span class="sxs-lookup"><span data-stu-id="79cb1-129">id</span></span>|<span data-ttu-id="79cb1-130">文字列</span><span class="sxs-lookup"><span data-stu-id="79cb1-130">String</span></span>|<span data-ttu-id="79cb1-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="79cb1-131">Key of the entity.</span></span> <span data-ttu-id="79cb1-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79cb1-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79cb1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79cb1-133">createdDateTime</span></span>|<span data-ttu-id="79cb1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79cb1-134">DateTimeOffset</span></span>|<span data-ttu-id="79cb1-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="79cb1-135">DateTime the object was created.</span></span> <span data-ttu-id="79cb1-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79cb1-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79cb1-137">説明</span><span class="sxs-lookup"><span data-stu-id="79cb1-137">description</span></span>|<span data-ttu-id="79cb1-138">文字列</span><span class="sxs-lookup"><span data-stu-id="79cb1-138">String</span></span>|<span data-ttu-id="79cb1-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="79cb1-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79cb1-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79cb1-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79cb1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79cb1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="79cb1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79cb1-142">DateTimeOffset</span></span>|<span data-ttu-id="79cb1-143">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="79cb1-143">DateTime the object was last modified.</span></span> <span data-ttu-id="79cb1-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79cb1-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79cb1-145">displayName</span><span class="sxs-lookup"><span data-stu-id="79cb1-145">displayName</span></span>|<span data-ttu-id="79cb1-146">文字列</span><span class="sxs-lookup"><span data-stu-id="79cb1-146">String</span></span>|<span data-ttu-id="79cb1-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="79cb1-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79cb1-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79cb1-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79cb1-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="79cb1-149">version</span></span>|<span data-ttu-id="79cb1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="79cb1-150">Int32</span></span>|<span data-ttu-id="79cb1-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="79cb1-151">Version of the device configuration.</span></span> <span data-ttu-id="79cb1-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79cb1-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="79cb1-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="79cb1-153">passwordRequired</span></span>|<span data-ttu-id="79cb1-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-154">Boolean</span></span>|<span data-ttu-id="79cb1-155">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="79cb1-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="79cb1-156">passwordBlockSimple</span></span>|<span data-ttu-id="79cb1-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-157">Boolean</span></span>|<span data-ttu-id="79cb1-158">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="79cb1-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="79cb1-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="79cb1-160">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-160">Boolean</span></span>|<span data-ttu-id="79cb1-161">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="79cb1-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="79cb1-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="79cb1-163">Int32</span><span class="sxs-lookup"><span data-stu-id="79cb1-163">Int32</span></span>|<span data-ttu-id="79cb1-164">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="79cb1-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="79cb1-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="79cb1-165">passwordExpirationDays</span></span>|<span data-ttu-id="79cb1-166">Int32</span><span class="sxs-lookup"><span data-stu-id="79cb1-166">Int32</span></span>|<span data-ttu-id="79cb1-167">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="79cb1-167">The password expiration in days.</span></span>|
|<span data-ttu-id="79cb1-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="79cb1-168">passwordMinimumLength</span></span>|<span data-ttu-id="79cb1-169">Int32</span><span class="sxs-lookup"><span data-stu-id="79cb1-169">Int32</span></span>|<span data-ttu-id="79cb1-170">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="79cb1-170">The minimum password length.</span></span>|
|<span data-ttu-id="79cb1-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="79cb1-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="79cb1-172">Int32</span><span class="sxs-lookup"><span data-stu-id="79cb1-172">Int32</span></span>|<span data-ttu-id="79cb1-173">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="79cb1-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="79cb1-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="79cb1-174">passwordRequiredType</span></span>|[<span data-ttu-id="79cb1-175">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="79cb1-175">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="79cb1-176">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="79cb1-176">The required password type.</span></span> <span data-ttu-id="79cb1-177">可能な値は、 `deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="79cb1-177">The possible values are `deviceDefault`, `alphanumeric`, or `numeric`.</span></span>|
|<span data-ttu-id="79cb1-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="79cb1-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="79cb1-179">Int32</span><span class="sxs-lookup"><span data-stu-id="79cb1-179">Int32</span></span>|<span data-ttu-id="79cb1-180">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="79cb1-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="79cb1-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="79cb1-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="79cb1-182">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-182">Boolean</span></span>|<span data-ttu-id="79cb1-183">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="79cb1-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="79cb1-184">osMinimumVersion</span></span>|<span data-ttu-id="79cb1-185">文字列</span><span class="sxs-lookup"><span data-stu-id="79cb1-185">String</span></span>|<span data-ttu-id="79cb1-186">Windows 10 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="79cb1-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="79cb1-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="79cb1-187">osMaximumVersion</span></span>|<span data-ttu-id="79cb1-188">文字列</span><span class="sxs-lookup"><span data-stu-id="79cb1-188">String</span></span>|<span data-ttu-id="79cb1-189">Windows 10 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="79cb1-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="79cb1-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="79cb1-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="79cb1-191">文字列</span><span class="sxs-lookup"><span data-stu-id="79cb1-191">String</span></span>|<span data-ttu-id="79cb1-192">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="79cb1-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="79cb1-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="79cb1-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="79cb1-194">文字列</span><span class="sxs-lookup"><span data-stu-id="79cb1-194">String</span></span>|<span data-ttu-id="79cb1-195">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="79cb1-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="79cb1-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="79cb1-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="79cb1-197">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-197">Boolean</span></span>|<span data-ttu-id="79cb1-198">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="79cb1-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="79cb1-199">bitLockerEnabled</span></span>|<span data-ttu-id="79cb1-200">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-200">Boolean</span></span>|<span data-ttu-id="79cb1-201">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="79cb1-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="79cb1-202">secureBootEnabled</span></span>|<span data-ttu-id="79cb1-203">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-203">Boolean</span></span>|<span data-ttu-id="79cb1-204">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="79cb1-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="79cb1-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="79cb1-206">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-206">Boolean</span></span>|<span data-ttu-id="79cb1-207">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="79cb1-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="79cb1-208">storageRequireEncryption</span></span>|<span data-ttu-id="79cb1-209">ブール値</span><span class="sxs-lookup"><span data-stu-id="79cb1-209">Boolean</span></span>|<span data-ttu-id="79cb1-210">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="79cb1-211">応答</span><span class="sxs-lookup"><span data-stu-id="79cb1-211">Response</span></span>
<span data-ttu-id="79cb1-212">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79cb1-212">If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79cb1-213">例</span><span class="sxs-lookup"><span data-stu-id="79cb1-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="79cb1-214">要求</span><span class="sxs-lookup"><span data-stu-id="79cb1-214">Request</span></span>
<span data-ttu-id="79cb1-215">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79cb1-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1018

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="79cb1-216">応答</span><span class="sxs-lookup"><span data-stu-id="79cb1-216">Response</span></span>
<span data-ttu-id="79cb1-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79cb1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



