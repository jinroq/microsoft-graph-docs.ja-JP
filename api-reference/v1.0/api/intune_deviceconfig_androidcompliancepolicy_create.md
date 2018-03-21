# <a name="create-androidcompliancepolicy"></a><span data-ttu-id="1e5a4-101">androidCompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="1e5a4-101">Create androidCompliancePolicy</span></span>

> <span data-ttu-id="1e5a4-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e5a4-103">新しい [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-103">Create a new [plannerBucket](../resources/intune_deviceconfig_androidcompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1e5a4-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1e5a4-104">Prerequisites</span></span>
<span data-ttu-id="1e5a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1e5a4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e5a4-107">Permission type</span></span>|<span data-ttu-id="1e5a4-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e5a4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e5a4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e5a4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1e5a4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e5a4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e5a4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e5a4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e5a4-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-112">Not supported.</span></span>|
|<span data-ttu-id="1e5a4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e5a4-113">Application</span></span>|<span data-ttu-id="1e5a4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e5a4-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e5a4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="1e5a4-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e5a4-116">Request headers</span></span>
|<span data-ttu-id="1e5a4-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e5a4-117">Header</span></span>|<span data-ttu-id="1e5a4-118">値</span><span class="sxs-lookup"><span data-stu-id="1e5a4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e5a4-119">承認</span><span class="sxs-lookup"><span data-stu-id="1e5a4-119">Authorization</span></span>|<span data-ttu-id="1e5a4-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1e5a4-121">承諾</span><span class="sxs-lookup"><span data-stu-id="1e5a4-121">Accept</span></span>|<span data-ttu-id="1e5a4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1e5a4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e5a4-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e5a4-123">Request body</span></span>
<span data-ttu-id="1e5a4-124">要求本文において、androidCompliancePolicy オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="1e5a4-125">次の表に、androidCompliancePolicy 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1e5a4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e5a4-126">Property</span></span>|<span data-ttu-id="1e5a4-127">型</span><span class="sxs-lookup"><span data-stu-id="1e5a4-127">Type</span></span>|<span data-ttu-id="1e5a4-128">説明</span><span class="sxs-lookup"><span data-stu-id="1e5a4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e5a4-129">id</span><span class="sxs-lookup"><span data-stu-id="1e5a4-129">id</span></span>|<span data-ttu-id="1e5a4-130">String</span><span class="sxs-lookup"><span data-stu-id="1e5a4-130">String</span></span>|<span data-ttu-id="1e5a4-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-131">Name of the entity.</span></span> <span data-ttu-id="1e5a4-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e5a4-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1e5a4-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e5a4-133">createdDateTime</span></span>|<span data-ttu-id="1e5a4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e5a4-134">DateTimeOffset</span></span>|<span data-ttu-id="1e5a4-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-135">DateTime the object was created.</span></span> <span data-ttu-id="1e5a4-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e5a4-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1e5a4-137">description</span><span class="sxs-lookup"><span data-stu-id="1e5a4-137">description</span></span>|<span data-ttu-id="1e5a4-138">String</span><span class="sxs-lookup"><span data-stu-id="1e5a4-138">String</span></span>|<span data-ttu-id="1e5a4-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1e5a4-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e5a4-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1e5a4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e5a4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="1e5a4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e5a4-142">DateTimeOffset</span></span>|<span data-ttu-id="1e5a4-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-143">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="1e5a4-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e5a4-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1e5a4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="1e5a4-145">displayName</span></span>|<span data-ttu-id="1e5a4-146">String</span><span class="sxs-lookup"><span data-stu-id="1e5a4-146">String</span></span>|<span data-ttu-id="1e5a4-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1e5a4-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e5a4-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1e5a4-149">version</span><span class="sxs-lookup"><span data-stu-id="1e5a4-149">version</span></span>|<span data-ttu-id="1e5a4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1e5a4-150">Int32</span></span>|<span data-ttu-id="1e5a4-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-151">Version of the device configuration.</span></span> <span data-ttu-id="1e5a4-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e5a4-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="1e5a4-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="1e5a4-153">passwordRequired</span></span>|<span data-ttu-id="1e5a4-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-154">Boolean</span></span>|<span data-ttu-id="1e5a4-155">デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-155">Require a password to unlock device.</span></span>|
|<span data-ttu-id="1e5a4-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1e5a4-156">passwordMinimumLength</span></span>|<span data-ttu-id="1e5a4-157">Int32</span><span class="sxs-lookup"><span data-stu-id="1e5a4-157">Int32</span></span>|<span data-ttu-id="1e5a4-158">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-158">Minimum password length.</span></span> <span data-ttu-id="1e5a4-159">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="1e5a4-159">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1e5a4-160">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1e5a4-160">passwordRequiredType</span></span>|<span data-ttu-id="1e5a4-161">String</span><span class="sxs-lookup"><span data-stu-id="1e5a4-161">String</span></span>|<span data-ttu-id="1e5a4-162">パスワードの文字の種類。可能な値は、`deviceDefault`、`alphabetic`、`alphanumeric`、`alphanumericWithSymbols`、`lowSecurityBiometric`、`numeric`、`numericComplex`、`any` です。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-162">Type of characters in password Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="1e5a4-163">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1e5a4-163">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1e5a4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1e5a4-164">Int32</span></span>|<span data-ttu-id="1e5a4-165">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-165">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="1e5a4-166">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1e5a4-166">passwordExpirationDays</span></span>|<span data-ttu-id="1e5a4-167">Int32</span><span class="sxs-lookup"><span data-stu-id="1e5a4-167">Int32</span></span>|<span data-ttu-id="1e5a4-168">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-168">Number of days before the password expires.</span></span> <span data-ttu-id="1e5a4-169">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="1e5a4-169">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1e5a4-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1e5a4-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1e5a4-171">Int32</span><span class="sxs-lookup"><span data-stu-id="1e5a4-171">Int32</span></span>|<span data-ttu-id="1e5a4-172">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-172">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="1e5a4-173">securityPreventInstallAppsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="1e5a4-173">securityPreventInstallAppsFromUnknownSources</span></span>|<span data-ttu-id="1e5a4-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-174">Boolean</span></span>|<span data-ttu-id="1e5a4-175">デバイスが不明なソースからのアプリのインストールを許可しないことを要求します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-175">Require that devices disallow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="1e5a4-176">securityDisableUsbDebugging</span><span class="sxs-lookup"><span data-stu-id="1e5a4-176">securityDisableUsbDebugging</span></span>|<span data-ttu-id="1e5a4-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-177">Boolean</span></span>|<span data-ttu-id="1e5a4-178">Android デバイスでの USB デバッグを無効にします。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-178">Disable USB debugging on Android devices.</span></span>|
|<span data-ttu-id="1e5a4-179">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1e5a4-179">securityRequireVerifyApps</span></span>|<span data-ttu-id="1e5a4-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-180">Boolean</span></span>|<span data-ttu-id="1e5a4-181">Android の検証アプリ機能がオンになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-181">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="1e5a4-182">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1e5a4-182">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="1e5a4-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-183">Boolean</span></span>|<span data-ttu-id="1e5a4-184">デバイス脅威保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-184">Require that devices have enabled device threat protection.</span></span>|
|<span data-ttu-id="1e5a4-185">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="1e5a4-185">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="1e5a4-186">String</span><span class="sxs-lookup"><span data-stu-id="1e5a4-186">String</span></span>|<span data-ttu-id="1e5a4-187">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-187">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="1e5a4-188">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-188">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="1e5a4-189">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="1e5a4-189">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="1e5a4-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-190">Boolean</span></span>|<span data-ttu-id="1e5a4-191">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-191">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="1e5a4-192">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="1e5a4-192">osMinimumVersion</span></span>|<span data-ttu-id="1e5a4-193">String</span><span class="sxs-lookup"><span data-stu-id="1e5a4-193">String</span></span>|<span data-ttu-id="1e5a4-194">Android の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-194">Minimum Android version.</span></span>|
|<span data-ttu-id="1e5a4-195">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="1e5a4-195">osMaximumVersion</span></span>|<span data-ttu-id="1e5a4-196">String</span><span class="sxs-lookup"><span data-stu-id="1e5a4-196">String</span></span>|<span data-ttu-id="1e5a4-197">Android の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-197">Maximum Android version.</span></span>|
|<span data-ttu-id="1e5a4-198">minAndroidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="1e5a4-198">minAndroidSecurityPatchLevel</span></span>|<span data-ttu-id="1e5a4-199">String</span><span class="sxs-lookup"><span data-stu-id="1e5a4-199">String</span></span>|<span data-ttu-id="1e5a4-200">Android セキュリティ パッチの最小レベル。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-200">Minimum Android security patch level.</span></span>|
|<span data-ttu-id="1e5a4-201">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="1e5a4-201">storageRequireEncryption</span></span>|<span data-ttu-id="1e5a4-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-202">Boolean</span></span>|<span data-ttu-id="1e5a4-203">Android デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-203">Require encryption on Android devices.</span></span>|
|<span data-ttu-id="1e5a4-204">securityRequireSafetyNetAttestationBasicIntegrity</span><span class="sxs-lookup"><span data-stu-id="1e5a4-204">securityRequireSafetyNetAttestationBasicIntegrity</span></span>|<span data-ttu-id="1e5a4-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-205">Boolean</span></span>|<span data-ttu-id="1e5a4-206">デバイスが SafetyNet の基本整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-206">Require the device to pass the SafetyNet basic integrity check.</span></span>|
|<span data-ttu-id="1e5a4-207">securityRequireSafetyNetAttestationCertifiedDevice</span><span class="sxs-lookup"><span data-stu-id="1e5a4-207">securityRequireSafetyNetAttestationCertifiedDevice</span></span>|<span data-ttu-id="1e5a4-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-208">Boolean</span></span>|<span data-ttu-id="1e5a4-209">デバイスが SafetyNet の認定デバイス チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-209">Require the device to pass the SafetyNet certified device check.</span></span>|
|<span data-ttu-id="1e5a4-210">securityRequireGooglePlayServices</span><span class="sxs-lookup"><span data-stu-id="1e5a4-210">securityRequireGooglePlayServices</span></span>|<span data-ttu-id="1e5a4-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-211">Boolean</span></span>|<span data-ttu-id="1e5a4-212">Google Play サービスがデバイスにインストールされて有効になっていることを要求します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-212">Require Google Play Services to be installed and enabled on the device.</span></span>|
|<span data-ttu-id="1e5a4-213">securityRequireUpToDateSecurityProviders</span><span class="sxs-lookup"><span data-stu-id="1e5a4-213">securityRequireUpToDateSecurityProviders</span></span>|<span data-ttu-id="1e5a4-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-214">Boolean</span></span>|<span data-ttu-id="1e5a4-215">デバイスに最新のセキュリティ プロバイダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-215">Require the device to have up to date security providers.</span></span> <span data-ttu-id="1e5a4-216">デバイスで Google Play 開発者サービスが有効かつ最新の状態になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-216">The device will require Google Play Services to be enabled and up to date.</span></span>|
|<span data-ttu-id="1e5a4-217">securityRequireCompanyPortalAppIntegrity</span><span class="sxs-lookup"><span data-stu-id="1e5a4-217">securityRequireCompanyPortalAppIntegrity</span></span>|<span data-ttu-id="1e5a4-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e5a4-218">Boolean</span></span>|<span data-ttu-id="1e5a4-219">デバイスが会社のポータル クライアント アプリのランタイム整合性チェックに合格することを要求します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-219">Require the device to pass the Company Portal client app runtime integrity check.</span></span>|



## <a name="response"></a><span data-ttu-id="1e5a4-220">応答</span><span class="sxs-lookup"><span data-stu-id="1e5a4-220">Response</span></span>
<span data-ttu-id="1e5a4-221">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-221">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_deviceconfig_androidcompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e5a4-222">例</span><span class="sxs-lookup"><span data-stu-id="1e5a4-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="1e5a4-223">要求</span><span class="sxs-lookup"><span data-stu-id="1e5a4-223">Request</span></span>
<span data-ttu-id="1e5a4-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1223

{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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

### <a name="response"></a><span data-ttu-id="1e5a4-225">応答</span><span class="sxs-lookup"><span data-stu-id="1e5a4-225">Response</span></span>
<span data-ttu-id="1e5a4-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e5a4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



