# <a name="create-androidworkprofilecompliancepolicy"></a><span data-ttu-id="71ba8-101">AndroidWorkProfileCompliancePolicy を作成します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-101">Create androidWorkProfileCompliancePolicy</span></span>

> <span data-ttu-id="71ba8-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="71ba8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71ba8-103">新しい[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-103">Create a new [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71ba8-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="71ba8-104">Prerequisites</span></span>
<span data-ttu-id="71ba8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71ba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71ba8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71ba8-107">Permission type</span></span>|<span data-ttu-id="71ba8-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="71ba8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71ba8-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71ba8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="71ba8-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ba8-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71ba8-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71ba8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71ba8-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71ba8-112">Not supported.</span></span>|
|<span data-ttu-id="71ba8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71ba8-113">Application</span></span>|<span data-ttu-id="71ba8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71ba8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71ba8-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71ba8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="71ba8-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71ba8-116">Request headers</span></span>
|<span data-ttu-id="71ba8-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71ba8-117">Header</span></span>|<span data-ttu-id="71ba8-118">値</span><span class="sxs-lookup"><span data-stu-id="71ba8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71ba8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="71ba8-119">Authorization</span></span>|<span data-ttu-id="71ba8-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="71ba8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71ba8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="71ba8-121">Accept</span></span>|<span data-ttu-id="71ba8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="71ba8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71ba8-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="71ba8-123">Request body</span></span>
<span data-ttu-id="71ba8-124">要求の本文に androidWorkProfileCompliancePolicy オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-124">In the request body, supply a JSON representation for the androidWorkProfileCompliancePolicy object.</span></span>

<span data-ttu-id="71ba8-125">次の表は、androidWorkProfileCompliancePolicy を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-125">The following table shows the properties that are required when you create the androidWorkProfileCompliancePolicy.</span></span>

|<span data-ttu-id="71ba8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71ba8-126">Property</span></span>|<span data-ttu-id="71ba8-127">型</span><span class="sxs-lookup"><span data-stu-id="71ba8-127">Type</span></span>|<span data-ttu-id="71ba8-128">説明</span><span class="sxs-lookup"><span data-stu-id="71ba8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71ba8-129">id</span><span class="sxs-lookup"><span data-stu-id="71ba8-129">id</span></span>|<span data-ttu-id="71ba8-130">String</span><span class="sxs-lookup"><span data-stu-id="71ba8-130">String</span></span>|<span data-ttu-id="71ba8-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="71ba8-131">Key of the entity.</span></span> <span data-ttu-id="71ba8-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71ba8-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71ba8-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71ba8-133">createdDateTime</span></span>|<span data-ttu-id="71ba8-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71ba8-134">DateTimeOffset</span></span>|<span data-ttu-id="71ba8-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="71ba8-135">DateTime the object was created.</span></span> <span data-ttu-id="71ba8-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71ba8-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71ba8-137">説明</span><span class="sxs-lookup"><span data-stu-id="71ba8-137">description</span></span>|<span data-ttu-id="71ba8-138">String</span><span class="sxs-lookup"><span data-stu-id="71ba8-138">String</span></span>|<span data-ttu-id="71ba8-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="71ba8-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71ba8-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71ba8-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71ba8-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71ba8-141">lastModifiedDateTime</span></span>|<span data-ttu-id="71ba8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71ba8-142">DateTimeOffset</span></span>|<span data-ttu-id="71ba8-143">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="71ba8-143">DateTime the object was last modified.</span></span> <span data-ttu-id="71ba8-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71ba8-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71ba8-145">displayName</span><span class="sxs-lookup"><span data-stu-id="71ba8-145">displayName</span></span>|<span data-ttu-id="71ba8-146">String</span><span class="sxs-lookup"><span data-stu-id="71ba8-146">String</span></span>|<span data-ttu-id="71ba8-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="71ba8-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71ba8-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71ba8-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71ba8-149">version</span><span class="sxs-lookup"><span data-stu-id="71ba8-149">version</span></span>|<span data-ttu-id="71ba8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="71ba8-150">Int32</span></span>|<span data-ttu-id="71ba8-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="71ba8-151">Version of the device configuration.</span></span> <span data-ttu-id="71ba8-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="71ba8-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="71ba8-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="71ba8-153">passwordRequired</span></span>|<span data-ttu-id="71ba8-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-154">Boolean</span></span>|<span data-ttu-id="71ba8-155">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="71ba8-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="71ba8-156">passwordMinimumLength</span></span>|<span data-ttu-id="71ba8-157">Int32</span><span class="sxs-lookup"><span data-stu-id="71ba8-157">Int32</span></span>|<span data-ttu-id="71ba8-158">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="71ba8-158">Minimum password length.</span></span> <span data-ttu-id="71ba8-159">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="71ba8-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="71ba8-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="71ba8-160">passwordRequiredType</span></span>|[<span data-ttu-id="71ba8-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="71ba8-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="71ba8-162">パスワード内の文字の種類です。</span><span class="sxs-lookup"><span data-stu-id="71ba8-162">Type of characters in password.</span></span> <span data-ttu-id="71ba8-163">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="71ba8-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="71ba8-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="71ba8-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="71ba8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="71ba8-165">Int32</span></span>|<span data-ttu-id="71ba8-166">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="71ba8-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="71ba8-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="71ba8-167">passwordExpirationDays</span></span>|<span data-ttu-id="71ba8-168">Int32</span><span class="sxs-lookup"><span data-stu-id="71ba8-168">Int32</span></span>|<span data-ttu-id="71ba8-169">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="71ba8-169">Number of days before the password expires.</span></span> <span data-ttu-id="71ba8-170">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="71ba8-170">Valid values 1 to 365</span></span>|
|<span data-ttu-id="71ba8-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="71ba8-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="71ba8-172">Int32</span><span class="sxs-lookup"><span data-stu-id="71ba8-172">Int32</span></span>|<span data-ttu-id="71ba8-173">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="71ba8-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="71ba8-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="71ba8-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="71ba8-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-175">Boolean</span></span>|<span data-ttu-id="71ba8-176">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="71ba8-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="71ba8-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="71ba8-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-178">Boolean</span></span>|<span data-ttu-id="71ba8-179">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="71ba8-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="71ba8-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="71ba8-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="71ba8-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-181">Boolean</span></span>|<span data-ttu-id="71ba8-182">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="71ba8-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="71ba8-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="71ba8-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-184">Boolean</span></span>|<span data-ttu-id="71ba8-185">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="71ba8-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="71ba8-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="71ba8-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="71ba8-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="71ba8-188">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="71ba8-189">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="71ba8-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="71ba8-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="71ba8-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="71ba8-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-191">Boolean</span></span>|<span data-ttu-id="71ba8-192">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="71ba8-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="71ba8-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="71ba8-193">osMinimumVersion</span></span>|<span data-ttu-id="71ba8-194">String</span><span class="sxs-lookup"><span data-stu-id="71ba8-194">String</span></span>|<span data-ttu-id="71ba8-195">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="71ba8-195">Minimum Android version.</span></span>|
|<span data-ttu-id="71ba8-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="71ba8-196">osMaximumVersion</span></span>|<span data-ttu-id="71ba8-197">String</span><span class="sxs-lookup"><span data-stu-id="71ba8-197">String</span></span>|<span data-ttu-id="71ba8-198">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="71ba8-198">Maximum Android version.</span></span>|
|<span data-ttu-id="71ba8-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="71ba8-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="71ba8-200">String</span><span class="sxs-lookup"><span data-stu-id="71ba8-200">String</span></span>|<span data-ttu-id="71ba8-201">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="71ba8-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="71ba8-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="71ba8-202">storageRequireEncryption</span></span>|<span data-ttu-id="71ba8-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-203">Boolean</span></span>|<span data-ttu-id="71ba8-204">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="71ba8-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="71ba8-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="71ba8-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-206">Boolean</span></span>|<span data-ttu-id="71ba8-207">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="71ba8-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="71ba8-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="71ba8-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-209">Boolean</span></span>|<span data-ttu-id="71ba8-210">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="71ba8-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="71ba8-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="71ba8-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-212">Boolean</span></span>|<span data-ttu-id="71ba8-213">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="71ba8-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="71ba8-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="71ba8-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-215">Boolean</span></span>|<span data-ttu-id="71ba8-216">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="71ba8-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="71ba8-217">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="71ba8-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="71ba8-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="71ba8-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="71ba8-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="71ba8-219">Boolean</span></span>|<span data-ttu-id="71ba8-220">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="71ba8-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="71ba8-221">応答</span><span class="sxs-lookup"><span data-stu-id="71ba8-221">Response</span></span>
<span data-ttu-id="71ba8-222">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="71ba8-222">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71ba8-223">例</span><span class="sxs-lookup"><span data-stu-id="71ba8-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="71ba8-224">要求</span><span class="sxs-lookup"><span data-stu-id="71ba8-224">Request</span></span>
<span data-ttu-id="71ba8-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71ba8-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="71ba8-226">応答</span><span class="sxs-lookup"><span data-stu-id="71ba8-226">Response</span></span>
<span data-ttu-id="71ba8-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71ba8-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "4e385271-5271-4e38-7152-384e7152384e",
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



