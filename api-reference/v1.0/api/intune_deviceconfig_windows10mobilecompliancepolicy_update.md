# <a name="update-windows10mobilecompliancepolicy"></a><span data-ttu-id="1efcc-101">windows10MobileCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="1efcc-101">Update windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="1efcc-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1efcc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1efcc-103">[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-103">Update the properties of a [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1efcc-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1efcc-104">Prerequisites</span></span>
<span data-ttu-id="1efcc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1efcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1efcc-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1efcc-107">Permission type</span></span>|<span data-ttu-id="1efcc-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1efcc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1efcc-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1efcc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1efcc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1efcc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1efcc-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1efcc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1efcc-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1efcc-112">Not supported.</span></span>|
|<span data-ttu-id="1efcc-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1efcc-113">Application</span></span>|<span data-ttu-id="1efcc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1efcc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1efcc-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1efcc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="1efcc-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1efcc-116">Request headers</span></span>
|<span data-ttu-id="1efcc-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1efcc-117">Header</span></span>|<span data-ttu-id="1efcc-118">値</span><span class="sxs-lookup"><span data-stu-id="1efcc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1efcc-119">承認</span><span class="sxs-lookup"><span data-stu-id="1efcc-119">Authorization</span></span>|<span data-ttu-id="1efcc-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="1efcc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1efcc-121">承諾</span><span class="sxs-lookup"><span data-stu-id="1efcc-121">Accept</span></span>|<span data-ttu-id="1efcc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1efcc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1efcc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1efcc-123">Request body</span></span>
<span data-ttu-id="1efcc-124">要求本文で、[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-124">In the request body, supply a JSON representation for the [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object.</span></span>

<span data-ttu-id="1efcc-125">次の表に、[windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-125">The following table shows the properties that are required when you create the [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md).</span></span>

|<span data-ttu-id="1efcc-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1efcc-126">Property</span></span>|<span data-ttu-id="1efcc-127">型</span><span class="sxs-lookup"><span data-stu-id="1efcc-127">Type</span></span>|<span data-ttu-id="1efcc-128">説明</span><span class="sxs-lookup"><span data-stu-id="1efcc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1efcc-129">id</span><span class="sxs-lookup"><span data-stu-id="1efcc-129">id</span></span>|<span data-ttu-id="1efcc-130">String</span><span class="sxs-lookup"><span data-stu-id="1efcc-130">String</span></span>|<span data-ttu-id="1efcc-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1efcc-131">Key of the entity.</span></span> <span data-ttu-id="1efcc-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1efcc-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1efcc-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1efcc-133">createdDateTime</span></span>|<span data-ttu-id="1efcc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1efcc-134">DateTimeOffset</span></span>|<span data-ttu-id="1efcc-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1efcc-135">DateTime the object was created.</span></span> <span data-ttu-id="1efcc-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1efcc-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1efcc-137">description</span><span class="sxs-lookup"><span data-stu-id="1efcc-137">description</span></span>|<span data-ttu-id="1efcc-138">String</span><span class="sxs-lookup"><span data-stu-id="1efcc-138">String</span></span>|<span data-ttu-id="1efcc-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1efcc-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1efcc-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1efcc-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1efcc-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1efcc-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1efcc-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1efcc-142">DateTimeOffset</span></span>|<span data-ttu-id="1efcc-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1efcc-143">DateTime the object was last modified.</span></span> <span data-ttu-id="1efcc-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1efcc-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1efcc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1efcc-145">displayName</span></span>|<span data-ttu-id="1efcc-146">String</span><span class="sxs-lookup"><span data-stu-id="1efcc-146">String</span></span>|<span data-ttu-id="1efcc-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1efcc-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1efcc-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1efcc-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1efcc-149">version</span><span class="sxs-lookup"><span data-stu-id="1efcc-149">version</span></span>|<span data-ttu-id="1efcc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1efcc-150">Int32</span></span>|<span data-ttu-id="1efcc-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1efcc-151">Version of the device configuration.</span></span> <span data-ttu-id="1efcc-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1efcc-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1efcc-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1efcc-153">passwordRequired</span></span>|<span data-ttu-id="1efcc-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efcc-154">Boolean</span></span>|<span data-ttu-id="1efcc-155">Windows Phone デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-155">Require a password to unlock Windows Phone device.</span></span>|
|<span data-ttu-id="1efcc-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1efcc-156">passwordBlockSimple</span></span>|<span data-ttu-id="1efcc-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efcc-157">Boolean</span></span>|<span data-ttu-id="1efcc-158">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-158">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="1efcc-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1efcc-159">passwordMinimumLength</span></span>|<span data-ttu-id="1efcc-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1efcc-160">Int32</span></span>|<span data-ttu-id="1efcc-161">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="1efcc-161">Minimum password length.</span></span> <span data-ttu-id="1efcc-162">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="1efcc-162">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1efcc-163">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1efcc-163">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="1efcc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1efcc-164">Int32</span></span>|<span data-ttu-id="1efcc-165">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="1efcc-165">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="1efcc-166">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1efcc-166">passwordRequiredType</span></span>|[<span data-ttu-id="1efcc-167">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1efcc-167">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="1efcc-168">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="1efcc-168">The required password type.</span></span> <span data-ttu-id="1efcc-169">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="1efcc-169">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1efcc-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1efcc-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1efcc-171">Int32</span><span class="sxs-lookup"><span data-stu-id="1efcc-171">Int32</span></span>|<span data-ttu-id="1efcc-172">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="1efcc-172">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="1efcc-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1efcc-173">passwordExpirationDays</span></span>|<span data-ttu-id="1efcc-174">Int32</span><span class="sxs-lookup"><span data-stu-id="1efcc-174">Int32</span></span>|<span data-ttu-id="1efcc-175">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="1efcc-175">Number of days before password expiration.</span></span> <span data-ttu-id="1efcc-176">有効な値は 1 から 255 までです</span><span class="sxs-lookup"><span data-stu-id="1efcc-176">Valid values 1 to 255</span></span>|
|<span data-ttu-id="1efcc-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1efcc-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1efcc-178">Int32</span><span class="sxs-lookup"><span data-stu-id="1efcc-178">Int32</span></span>|<span data-ttu-id="1efcc-179">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="1efcc-179">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="1efcc-180">passwordRequireToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="1efcc-180">passwordRequireToUnlockFromIdle</span></span>|<span data-ttu-id="1efcc-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efcc-181">Boolean</span></span>|<span data-ttu-id="1efcc-182">アイドル デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-182">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="1efcc-183">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1efcc-183">osMinimumVersion</span></span>|<span data-ttu-id="1efcc-184">String</span><span class="sxs-lookup"><span data-stu-id="1efcc-184">String</span></span>|<span data-ttu-id="1efcc-185">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="1efcc-185">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="1efcc-186">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1efcc-186">osMaximumVersion</span></span>|<span data-ttu-id="1efcc-187">String</span><span class="sxs-lookup"><span data-stu-id="1efcc-187">String</span></span>|<span data-ttu-id="1efcc-188">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="1efcc-188">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="1efcc-189">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="1efcc-189">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="1efcc-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efcc-190">Boolean</span></span>|<span data-ttu-id="1efcc-191">デバイスが Windows デバイス正常性構成証明によって正常と報告される (早期起動マルウェア対策ドライバーが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-191">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="1efcc-192">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="1efcc-192">bitLockerEnabled</span></span>|<span data-ttu-id="1efcc-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efcc-193">Boolean</span></span>|<span data-ttu-id="1efcc-194">デバイスが Windows デバイス正常性構成証明によって正常と報告される (BitLocker が有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-194">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="1efcc-195">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="1efcc-195">secureBootEnabled</span></span>|<span data-ttu-id="1efcc-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efcc-196">Boolean</span></span>|<span data-ttu-id="1efcc-197">デバイスが Windows デバイス正常性構成証明によって正常と報告される (セキュア ブートが有効である) ことを要求します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-197">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="1efcc-198">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="1efcc-198">codeIntegrityEnabled</span></span>|<span data-ttu-id="1efcc-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efcc-199">Boolean</span></span>|<span data-ttu-id="1efcc-200">デバイスが Windows デバイス正常性構成証明によって正常と報告されることを要求します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-200">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="1efcc-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1efcc-201">storageRequireEncryption</span></span>|<span data-ttu-id="1efcc-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="1efcc-202">Boolean</span></span>|<span data-ttu-id="1efcc-203">Windows デバイス上での暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-203">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="1efcc-204">応答</span><span class="sxs-lookup"><span data-stu-id="1efcc-204">Response</span></span>
<span data-ttu-id="1efcc-205">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="1efcc-205">If successful, this method returns a `200 OK` response code and an updated [windows10MobileCompliancePolicy](../resources/intune_deviceconfig_windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1efcc-206">例</span><span class="sxs-lookup"><span data-stu-id="1efcc-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="1efcc-207">要求</span><span class="sxs-lookup"><span data-stu-id="1efcc-207">Request</span></span>
<span data-ttu-id="1efcc-208">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1efcc-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1efcc-209">応答</span><span class="sxs-lookup"><span data-stu-id="1efcc-209">Response</span></span>
<span data-ttu-id="1efcc-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1efcc-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



