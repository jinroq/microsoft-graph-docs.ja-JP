# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="b23dd-101">Update androidCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b23dd-101">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="b23dd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b23dd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b23dd-103">[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-103">Update the properties of a [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b23dd-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b23dd-104">Prerequisites</span></span>
<span data-ttu-id="b23dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b23dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b23dd-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b23dd-107">Permission type</span></span>|<span data-ttu-id="b23dd-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b23dd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b23dd-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="b23dd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b23dd-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23dd-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b23dd-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b23dd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b23dd-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b23dd-112">Not supported.</span></span>|
|<span data-ttu-id="b23dd-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b23dd-113">Application</span></span>|<span data-ttu-id="b23dd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b23dd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b23dd-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b23dd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b23dd-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b23dd-116">Request headers</span></span>
|<span data-ttu-id="b23dd-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b23dd-117">Header</span></span>|<span data-ttu-id="b23dd-118">値</span><span class="sxs-lookup"><span data-stu-id="b23dd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b23dd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b23dd-119">Authorization</span></span>|<span data-ttu-id="b23dd-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b23dd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b23dd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b23dd-121">Accept</span></span>|<span data-ttu-id="b23dd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b23dd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b23dd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b23dd-123">Request body</span></span>
<span data-ttu-id="b23dd-124">要求本文において、[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクト用の JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-124">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="b23dd-125">次の表に、[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-125">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="b23dd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b23dd-126">Property</span></span>|<span data-ttu-id="b23dd-127">型</span><span class="sxs-lookup"><span data-stu-id="b23dd-127">Type</span></span>|<span data-ttu-id="b23dd-128">説明</span><span class="sxs-lookup"><span data-stu-id="b23dd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b23dd-129">id</span><span class="sxs-lookup"><span data-stu-id="b23dd-129">id</span></span>|<span data-ttu-id="b23dd-130">String</span><span class="sxs-lookup"><span data-stu-id="b23dd-130">String</span></span>|<span data-ttu-id="b23dd-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b23dd-131">Key of the entity.</span></span> <span data-ttu-id="b23dd-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b23dd-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b23dd-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b23dd-133">createdDateTime</span></span>|<span data-ttu-id="b23dd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b23dd-134">DateTimeOffset</span></span>|<span data-ttu-id="b23dd-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b23dd-135">DateTime the object was created.</span></span> <span data-ttu-id="b23dd-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b23dd-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b23dd-137">description</span><span class="sxs-lookup"><span data-stu-id="b23dd-137">description</span></span>|<span data-ttu-id="b23dd-138">String</span><span class="sxs-lookup"><span data-stu-id="b23dd-138">String</span></span>|<span data-ttu-id="b23dd-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="b23dd-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b23dd-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b23dd-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b23dd-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b23dd-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b23dd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b23dd-142">DateTimeOffset</span></span>|<span data-ttu-id="b23dd-143">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b23dd-143">DateTime the object was last modified.</span></span> <span data-ttu-id="b23dd-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b23dd-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b23dd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b23dd-145">displayName</span></span>|<span data-ttu-id="b23dd-146">String</span><span class="sxs-lookup"><span data-stu-id="b23dd-146">String</span></span>|<span data-ttu-id="b23dd-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="b23dd-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b23dd-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b23dd-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b23dd-149">version</span><span class="sxs-lookup"><span data-stu-id="b23dd-149">version</span></span>|<span data-ttu-id="b23dd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b23dd-150">Int32</span></span>|<span data-ttu-id="b23dd-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b23dd-151">Version of the device configuration.</span></span> <span data-ttu-id="b23dd-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b23dd-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b23dd-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b23dd-153">passwordRequired</span></span>|<span data-ttu-id="b23dd-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-154">Boolean</span></span>|<span data-ttu-id="b23dd-155">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="b23dd-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b23dd-156">passwordMinimumLength</span></span>|<span data-ttu-id="b23dd-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b23dd-157">Int32</span></span>|<span data-ttu-id="b23dd-158">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="b23dd-158">Minimum password length.</span></span> <span data-ttu-id="b23dd-159">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="b23dd-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b23dd-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b23dd-160">passwordRequiredType</span></span>|[<span data-ttu-id="b23dd-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b23dd-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="b23dd-162">パスワード内の文字の種類です。</span><span class="sxs-lookup"><span data-stu-id="b23dd-162">Type of characters in password.</span></span> <span data-ttu-id="b23dd-163">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="b23dd-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="b23dd-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b23dd-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b23dd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b23dd-165">Int32</span></span>|<span data-ttu-id="b23dd-166">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="b23dd-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b23dd-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b23dd-167">passwordExpirationDays</span></span>|<span data-ttu-id="b23dd-168">Int32</span><span class="sxs-lookup"><span data-stu-id="b23dd-168">Int32</span></span>|<span data-ttu-id="b23dd-169">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="b23dd-169">Number of days before the password expires.</span></span> <span data-ttu-id="b23dd-170">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="b23dd-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b23dd-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b23dd-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b23dd-172">Int32</span><span class="sxs-lookup"><span data-stu-id="b23dd-172">Int32</span></span>|<span data-ttu-id="b23dd-173">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="b23dd-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="b23dd-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="b23dd-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="b23dd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-175">Boolean</span></span>|<span data-ttu-id="b23dd-176">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="b23dd-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="b23dd-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="b23dd-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-178">Boolean</span></span>|<span data-ttu-id="b23dd-179">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="b23dd-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="b23dd-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="b23dd-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="b23dd-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-181">Boolean</span></span>|<span data-ttu-id="b23dd-182">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="b23dd-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="b23dd-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="b23dd-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-184">Boolean</span></span>|<span data-ttu-id="b23dd-185">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="b23dd-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b23dd-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="b23dd-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="b23dd-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="b23dd-188">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="b23dd-189">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="b23dd-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="b23dd-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="b23dd-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="b23dd-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-191">Boolean</span></span>|<span data-ttu-id="b23dd-192">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="b23dd-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="b23dd-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b23dd-193">osMinimumVersion</span></span>|<span data-ttu-id="b23dd-194">String</span><span class="sxs-lookup"><span data-stu-id="b23dd-194">String</span></span>|<span data-ttu-id="b23dd-195">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="b23dd-195">Minimum Android version.</span></span>|
|<span data-ttu-id="b23dd-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b23dd-196">osMaximumVersion</span></span>|<span data-ttu-id="b23dd-197">String</span><span class="sxs-lookup"><span data-stu-id="b23dd-197">String</span></span>|<span data-ttu-id="b23dd-198">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="b23dd-198">Maximum Android version.</span></span>|
|<span data-ttu-id="b23dd-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="b23dd-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="b23dd-200">String</span><span class="sxs-lookup"><span data-stu-id="b23dd-200">String</span></span>|<span data-ttu-id="b23dd-201">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="b23dd-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="b23dd-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b23dd-202">storageRequireEncryption</span></span>|<span data-ttu-id="b23dd-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-203">Boolean</span></span>|<span data-ttu-id="b23dd-204">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="b23dd-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="b23dd-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="b23dd-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-206">Boolean</span></span>|<span data-ttu-id="b23dd-207">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="b23dd-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="b23dd-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="b23dd-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-209">Boolean</span></span>|<span data-ttu-id="b23dd-210">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="b23dd-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="b23dd-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="b23dd-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-212">Boolean</span></span>|<span data-ttu-id="b23dd-213">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="b23dd-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="b23dd-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="b23dd-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-215">Boolean</span></span>|<span data-ttu-id="b23dd-216">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="b23dd-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="b23dd-217">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b23dd-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="b23dd-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="b23dd-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="b23dd-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="b23dd-219">Boolean</span></span>|<span data-ttu-id="b23dd-220">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="b23dd-221">応答</span><span class="sxs-lookup"><span data-stu-id="b23dd-221">Response</span></span>
<span data-ttu-id="b23dd-222">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b23dd-222">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b23dd-223">例</span><span class="sxs-lookup"><span data-stu-id="b23dd-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="b23dd-224">要求</span><span class="sxs-lookup"><span data-stu-id="b23dd-224">Request</span></span>
<span data-ttu-id="b23dd-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b23dd-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1159

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a><span data-ttu-id="b23dd-226">応答</span><span class="sxs-lookup"><span data-stu-id="b23dd-226">Response</span></span>
<span data-ttu-id="b23dd-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b23dd-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
  "id": "752c820f-820f-752c-0f82-2c750f822c75",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```



