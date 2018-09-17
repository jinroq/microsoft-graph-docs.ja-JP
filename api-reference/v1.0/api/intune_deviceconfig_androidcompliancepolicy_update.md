# <a name="update-androidcompliancepolicy"></a><span data-ttu-id="a2941-101">androidCompliancePolicy を更新する</span><span class="sxs-lookup"><span data-stu-id="a2941-101">Update androidCompliancePolicy</span></span>

> <span data-ttu-id="a2941-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2941-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2941-103">[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a2941-103">Update the properties of a [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2941-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2941-104">Prerequisites</span></span>
<span data-ttu-id="a2941-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2941-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2941-107">Permission type</span></span>|<span data-ttu-id="a2941-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2941-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2941-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2941-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a2941-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2941-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2941-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2941-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2941-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2941-112">Not supported.</span></span>|
|<span data-ttu-id="a2941-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2941-113">Application</span></span>|<span data-ttu-id="a2941-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2941-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2941-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2941-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a2941-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2941-116">Request headers</span></span>
|<span data-ttu-id="a2941-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2941-117">Header</span></span>|<span data-ttu-id="a2941-118">値</span><span class="sxs-lookup"><span data-stu-id="a2941-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2941-119">承認</span><span class="sxs-lookup"><span data-stu-id="a2941-119">Authorization</span></span>|<span data-ttu-id="a2941-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a2941-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2941-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="a2941-121">Accept</span></span>|<span data-ttu-id="a2941-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="a2941-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2941-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2941-123">Request body</span></span>
<span data-ttu-id="a2941-124">要求本文において、[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクト用の JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="a2941-124">In the request body, supply a JSON representation for the [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>

<span data-ttu-id="a2941-125">次の表に、[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a2941-125">The following table shows the properties that are required when you create the [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).</span></span>

|<span data-ttu-id="a2941-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2941-126">Property</span></span>|<span data-ttu-id="a2941-127">型</span><span class="sxs-lookup"><span data-stu-id="a2941-127">Type</span></span>|<span data-ttu-id="a2941-128">説明</span><span class="sxs-lookup"><span data-stu-id="a2941-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2941-129">ID</span><span class="sxs-lookup"><span data-stu-id="a2941-129">id</span></span>|<span data-ttu-id="a2941-130">文字列</span><span class="sxs-lookup"><span data-stu-id="a2941-130">String</span></span>|<span data-ttu-id="a2941-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a2941-131">Key of the entity.</span></span> <span data-ttu-id="a2941-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2941-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2941-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2941-133">createdDateTime</span></span>|<span data-ttu-id="a2941-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2941-134">DateTimeOffset</span></span>|<span data-ttu-id="a2941-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a2941-135">DateTime the object was created.</span></span> <span data-ttu-id="a2941-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2941-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2941-137">説明</span><span class="sxs-lookup"><span data-stu-id="a2941-137">description</span></span>|<span data-ttu-id="a2941-138">文字列</span><span class="sxs-lookup"><span data-stu-id="a2941-138">String</span></span>|<span data-ttu-id="a2941-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="a2941-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2941-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2941-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2941-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2941-141">lastModifiedDateTime</span></span>|<span data-ttu-id="a2941-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2941-142">DateTimeOffset</span></span>|<span data-ttu-id="a2941-143">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a2941-143">DateTime the object was last modified.</span></span> <span data-ttu-id="a2941-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2941-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2941-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a2941-145">displayName</span></span>|<span data-ttu-id="a2941-146">文字列</span><span class="sxs-lookup"><span data-stu-id="a2941-146">String</span></span>|<span data-ttu-id="a2941-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="a2941-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2941-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2941-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2941-149">バージョン</span><span class="sxs-lookup"><span data-stu-id="a2941-149">version</span></span>|<span data-ttu-id="a2941-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a2941-150">Int32</span></span>|<span data-ttu-id="a2941-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a2941-151">Version of the device configuration.</span></span> <span data-ttu-id="a2941-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a2941-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="a2941-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a2941-153">passwordRequired</span></span>|<span data-ttu-id="a2941-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-154">Boolean</span></span>|<span data-ttu-id="a2941-155">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="a2941-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a2941-156">passwordMinimumLength</span></span>|<span data-ttu-id="a2941-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a2941-157">Int32</span></span>|<span data-ttu-id="a2941-158">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="a2941-158">Minimum password length.</span></span> <span data-ttu-id="a2941-159">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="a2941-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a2941-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a2941-160">passwordRequiredType</span></span>|[<span data-ttu-id="a2941-161">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a2941-161">androidRequiredPasswordType</span></span>](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|<span data-ttu-id="a2941-162">パスワード内の文字の種類。</span><span class="sxs-lookup"><span data-stu-id="a2941-162">Type of characters in password Possible values are: , , , , , , , .</span></span> <span data-ttu-id="a2941-163">可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="a2941-163">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="a2941-164">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a2941-164">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a2941-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a2941-165">Int32</span></span>|<span data-ttu-id="a2941-166">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="a2941-166">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="a2941-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a2941-167">passwordExpirationDays</span></span>|<span data-ttu-id="a2941-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a2941-168">Int32</span></span>|<span data-ttu-id="a2941-169">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="a2941-169">Number of days before the password expires.</span></span> <span data-ttu-id="a2941-170">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="a2941-170">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="a2941-171">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a2941-171">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a2941-172">Int32</span><span class="sxs-lookup"><span data-stu-id="a2941-172">Int32</span></span>|<span data-ttu-id="a2941-173">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="a2941-173">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="a2941-174">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="a2941-174">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="a2941-175">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-175">Boolean</span></span>|<span data-ttu-id="a2941-176">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-176">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="a2941-177">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="a2941-177">securityDisableUsbDebugging</span></span>|<span data-ttu-id="a2941-178">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-178">Boolean</span></span>|<span data-ttu-id="a2941-179">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="a2941-179">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="a2941-180">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a2941-180">securityRequireVerifyApps</span></span>|<span data-ttu-id="a2941-181">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-181">Boolean</span></span>|<span data-ttu-id="a2941-182">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-182">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="a2941-183">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a2941-183">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="a2941-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-184">Boolean</span></span>|<span data-ttu-id="a2941-185">デバイスの脅威保護が有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-185">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="a2941-186">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="a2941-186">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="a2941-187">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="a2941-187">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="a2941-188">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-188">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="a2941-189">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="a2941-189">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="a2941-190">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="a2941-190">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="a2941-191">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-191">Boolean</span></span>|<span data-ttu-id="a2941-192">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="a2941-192">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="a2941-193">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="a2941-193">osMinimumVersion</span></span>|<span data-ttu-id="a2941-194">文字列</span><span class="sxs-lookup"><span data-stu-id="a2941-194">String</span></span>|<span data-ttu-id="a2941-195">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="a2941-195">Minimum Android version.</span></span>|
|<span data-ttu-id="a2941-196">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="a2941-196">osMaximumVersion</span></span>|<span data-ttu-id="a2941-197">文字列</span><span class="sxs-lookup"><span data-stu-id="a2941-197">String</span></span>|<span data-ttu-id="a2941-198">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="a2941-198">Maximum Android version.</span></span>|
|<span data-ttu-id="a2941-199">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a2941-199">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="a2941-200">文字列</span><span class="sxs-lookup"><span data-stu-id="a2941-200">String</span></span>|<span data-ttu-id="a2941-201">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="a2941-201">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="a2941-202">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="a2941-202">storageRequireEncryption</span></span>|<span data-ttu-id="a2941-203">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-203">Boolean</span></span>|<span data-ttu-id="a2941-204">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-204">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="a2941-205">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="a2941-205">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="a2941-206">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-206">Boolean</span></span>|<span data-ttu-id="a2941-207">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-207">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="a2941-208">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="a2941-208">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="a2941-209">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-209">Boolean</span></span>|<span data-ttu-id="a2941-210">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-210">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="a2941-211">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="a2941-211">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="a2941-212">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-212">Boolean</span></span>|<span data-ttu-id="a2941-213">Google Play 開発者サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-213">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="a2941-214">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="a2941-214">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="a2941-215">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-215">Boolean</span></span>|<span data-ttu-id="a2941-216">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="a2941-216">Require the device to have up to date security providers.</span></span> <span data-ttu-id="a2941-217">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2941-217">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="a2941-218">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="a2941-218">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="a2941-219">ブール値</span><span class="sxs-lookup"><span data-stu-id="a2941-219">Boolean</span></span>|<span data-ttu-id="a2941-220">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="a2941-220">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="a2941-221">応答</span><span class="sxs-lookup"><span data-stu-id="a2941-221">Response</span></span>
<span data-ttu-id="a2941-222">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a2941-222">If successful, this method returns a `200 OK` response code and an updated [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2941-223">例</span><span class="sxs-lookup"><span data-stu-id="a2941-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2941-224">要求</span><span class="sxs-lookup"><span data-stu-id="a2941-224">Request</span></span>
<span data-ttu-id="a2941-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2941-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1161

{
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

### <a name="response"></a><span data-ttu-id="a2941-226">応答</span><span class="sxs-lookup"><span data-stu-id="a2941-226">Response</span></span>
<span data-ttu-id="a2941-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2941-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








