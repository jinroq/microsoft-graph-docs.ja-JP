# <a name="create-macoscompliancepolicy"></a><span data-ttu-id="d563a-101">macOSCompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="d563a-101">Create macOSCompliancePolicy</span></span>

> <span data-ttu-id="d563a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d563a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d563a-103">新しい [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d563a-103">Create a new [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d563a-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d563a-104">Prerequisites</span></span>
<span data-ttu-id="d563a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d563a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d563a-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d563a-107">Permission type</span></span>|<span data-ttu-id="d563a-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d563a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d563a-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d563a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d563a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d563a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d563a-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d563a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d563a-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d563a-112">Not supported.</span></span>|
|<span data-ttu-id="d563a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d563a-113">Application</span></span>|<span data-ttu-id="d563a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d563a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d563a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d563a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="d563a-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d563a-116">Request headers</span></span>
|<span data-ttu-id="d563a-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d563a-117">Header</span></span>|<span data-ttu-id="d563a-118">値</span><span class="sxs-lookup"><span data-stu-id="d563a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d563a-119">承認</span><span class="sxs-lookup"><span data-stu-id="d563a-119">Authorization</span></span>|<span data-ttu-id="d563a-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="d563a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d563a-121">承諾</span><span class="sxs-lookup"><span data-stu-id="d563a-121">Accept</span></span>|<span data-ttu-id="d563a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d563a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d563a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d563a-123">Request body</span></span>
<span data-ttu-id="d563a-124">要求本文で、macOSCompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d563a-124">In the request body, supply a JSON representation for the macOSCompliancePolicy object.</span></span>

<span data-ttu-id="d563a-125">次の表に、macOSCompliancePolicy 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d563a-125">The following table shows the properties that are required when you create the macOSCompliancePolicy.</span></span>

|<span data-ttu-id="d563a-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d563a-126">Property</span></span>|<span data-ttu-id="d563a-127">型</span><span class="sxs-lookup"><span data-stu-id="d563a-127">Type</span></span>|<span data-ttu-id="d563a-128">説明</span><span class="sxs-lookup"><span data-stu-id="d563a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d563a-129">id</span><span class="sxs-lookup"><span data-stu-id="d563a-129">id</span></span>|<span data-ttu-id="d563a-130">String</span><span class="sxs-lookup"><span data-stu-id="d563a-130">String</span></span>|<span data-ttu-id="d563a-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d563a-131">Key of the entity.</span></span> <span data-ttu-id="d563a-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d563a-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d563a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d563a-133">createdDateTime</span></span>|<span data-ttu-id="d563a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d563a-134">DateTimeOffset</span></span>|<span data-ttu-id="d563a-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d563a-135">DateTime the object was created.</span></span> <span data-ttu-id="d563a-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d563a-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d563a-137">description</span><span class="sxs-lookup"><span data-stu-id="d563a-137">description</span></span>|<span data-ttu-id="d563a-138">String</span><span class="sxs-lookup"><span data-stu-id="d563a-138">String</span></span>|<span data-ttu-id="d563a-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d563a-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d563a-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d563a-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d563a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d563a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d563a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d563a-142">DateTimeOffset</span></span>|<span data-ttu-id="d563a-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d563a-143">DateTime the object was last modified.</span></span> <span data-ttu-id="d563a-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d563a-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d563a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d563a-145">displayName</span></span>|<span data-ttu-id="d563a-146">String</span><span class="sxs-lookup"><span data-stu-id="d563a-146">String</span></span>|<span data-ttu-id="d563a-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d563a-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d563a-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d563a-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d563a-149">version</span><span class="sxs-lookup"><span data-stu-id="d563a-149">version</span></span>|<span data-ttu-id="d563a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d563a-150">Int32</span></span>|<span data-ttu-id="d563a-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d563a-151">Version of the device configuration.</span></span> <span data-ttu-id="d563a-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d563a-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="d563a-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d563a-153">passwordRequired</span></span>|<span data-ttu-id="d563a-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="d563a-154">Boolean</span></span>|<span data-ttu-id="d563a-155">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d563a-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="d563a-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d563a-156">passwordBlockSimple</span></span>|<span data-ttu-id="d563a-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="d563a-157">Boolean</span></span>|<span data-ttu-id="d563a-158">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d563a-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="d563a-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d563a-159">passwordExpirationDays</span></span>|<span data-ttu-id="d563a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d563a-160">Int32</span></span>|<span data-ttu-id="d563a-161">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="d563a-161">Number of days before the password expires.</span></span> <span data-ttu-id="d563a-162">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="d563a-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="d563a-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d563a-163">passwordMinimumLength</span></span>|<span data-ttu-id="d563a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d563a-164">Int32</span></span>|<span data-ttu-id="d563a-165">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="d563a-165">Minimum length of password.</span></span> <span data-ttu-id="d563a-166">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="d563a-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="d563a-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d563a-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d563a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="d563a-168">Int32</span></span>|<span data-ttu-id="d563a-169">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="d563a-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="d563a-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d563a-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d563a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="d563a-171">Int32</span></span>|<span data-ttu-id="d563a-172">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="d563a-172">Number of previous passwords to block.</span></span> <span data-ttu-id="d563a-173">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="d563a-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d563a-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d563a-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d563a-175">Int32</span><span class="sxs-lookup"><span data-stu-id="d563a-175">Int32</span></span>|<span data-ttu-id="d563a-176">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="d563a-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="d563a-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d563a-177">passwordRequiredType</span></span>|[<span data-ttu-id="d563a-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d563a-178">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="d563a-179">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="d563a-179">The required password type.</span></span> <span data-ttu-id="d563a-180">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="d563a-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d563a-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d563a-181">osMinimumVersion</span></span>|<span data-ttu-id="d563a-182">String</span><span class="sxs-lookup"><span data-stu-id="d563a-182">String</span></span>|<span data-ttu-id="d563a-183">最小の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="d563a-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="d563a-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d563a-184">osMaximumVersion</span></span>|<span data-ttu-id="d563a-185">String</span><span class="sxs-lookup"><span data-stu-id="d563a-185">String</span></span>|<span data-ttu-id="d563a-186">最大の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="d563a-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="d563a-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="d563a-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="d563a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d563a-188">Boolean</span></span>|<span data-ttu-id="d563a-189">デバイスでシステム整合性の保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d563a-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="d563a-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="d563a-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="d563a-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d563a-191">Boolean</span></span>|<span data-ttu-id="d563a-192">デバイスの脅威保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d563a-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="d563a-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="d563a-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="d563a-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="d563a-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="d563a-195">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="d563a-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="d563a-196">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="d563a-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="d563a-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="d563a-197">storageRequireEncryption</span></span>|<span data-ttu-id="d563a-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="d563a-198">Boolean</span></span>|<span data-ttu-id="d563a-199">Mac OS デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="d563a-199">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="d563a-200">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="d563a-200">firewallEnabled</span></span>|<span data-ttu-id="d563a-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="d563a-201">Boolean</span></span>|<span data-ttu-id="d563a-202">かどうか、か、これらのファイアウォールは有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d563a-202">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="d563a-203">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="d563a-203">firewallBlockAllIncoming</span></span>|<span data-ttu-id="d563a-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="d563a-204">Boolean</span></span>|<span data-ttu-id="d563a-205">「すべての着信接続をブロックする] オプションに対応します。</span><span class="sxs-lookup"><span data-stu-id="d563a-205">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="d563a-206">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="d563a-206">firewallEnableStealthMode</span></span>|<span data-ttu-id="d563a-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="d563a-207">Boolean</span></span>|<span data-ttu-id="d563a-208">「有効にするステルス モード」に対応</span><span class="sxs-lookup"><span data-stu-id="d563a-208">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="d563a-209">応答</span><span class="sxs-lookup"><span data-stu-id="d563a-209">Response</span></span>
<span data-ttu-id="d563a-210">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d563a-210">If successful, this method returns a `201 Created` response code and a [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d563a-211">例</span><span class="sxs-lookup"><span data-stu-id="d563a-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="d563a-212">要求</span><span class="sxs-lookup"><span data-stu-id="d563a-212">Request</span></span>
<span data-ttu-id="d563a-213">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d563a-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 849

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="d563a-214">応答</span><span class="sxs-lookup"><span data-stu-id="d563a-214">Response</span></span>
<span data-ttu-id="d563a-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d563a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



