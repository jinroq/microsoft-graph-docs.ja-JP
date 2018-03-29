# <a name="create-ioscompliancepolicy"></a><span data-ttu-id="4a347-101">Create iosCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4a347-101">Create iosCompliancePolicy</span></span>

> <span data-ttu-id="4a347-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a347-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a347-103">新しい [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4a347-103">Create a new [plannerBucket](../resources/intune_deviceconfig_ioscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a347-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="4a347-104">Prerequisites</span></span>
<span data-ttu-id="4a347-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a347-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a347-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a347-107">Permission type</span></span>|<span data-ttu-id="4a347-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a347-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a347-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a347-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4a347-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a347-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a347-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a347-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a347-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a347-112">Not supported.</span></span>|
|<span data-ttu-id="4a347-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a347-113">Application</span></span>|<span data-ttu-id="4a347-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a347-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a347-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a347-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4a347-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a347-116">Request headers</span></span>
|<span data-ttu-id="4a347-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a347-117">Header</span></span>|<span data-ttu-id="4a347-118">値</span><span class="sxs-lookup"><span data-stu-id="4a347-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a347-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a347-119">Authorization</span></span>|<span data-ttu-id="4a347-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4a347-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4a347-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4a347-121">Accept</span></span>|<span data-ttu-id="4a347-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4a347-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a347-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a347-123">Request body</span></span>
<span data-ttu-id="4a347-124">要求本文で、iosCompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a347-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="4a347-125">次の表に、iosCompliancePolicy 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4a347-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="4a347-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a347-126">Property</span></span>|<span data-ttu-id="4a347-127">型</span><span class="sxs-lookup"><span data-stu-id="4a347-127">Type</span></span>|<span data-ttu-id="4a347-128">説明</span><span class="sxs-lookup"><span data-stu-id="4a347-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a347-129">id</span><span class="sxs-lookup"><span data-stu-id="4a347-129">id</span></span>|<span data-ttu-id="4a347-130">String</span><span class="sxs-lookup"><span data-stu-id="4a347-130">String</span></span>|<span data-ttu-id="4a347-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4a347-131">Name of the entity.</span></span> <span data-ttu-id="4a347-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4a347-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4a347-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a347-133">createdDateTime</span></span>|<span data-ttu-id="4a347-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a347-134">DateTimeOffset</span></span>|<span data-ttu-id="4a347-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4a347-135">DateTime the object was created.</span></span> <span data-ttu-id="4a347-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4a347-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4a347-137">description</span><span class="sxs-lookup"><span data-stu-id="4a347-137">description</span></span>|<span data-ttu-id="4a347-138">String</span><span class="sxs-lookup"><span data-stu-id="4a347-138">String</span></span>|<span data-ttu-id="4a347-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="4a347-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a347-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4a347-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4a347-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a347-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4a347-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a347-142">DateTimeOffset</span></span>|<span data-ttu-id="4a347-143">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4a347-143">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="4a347-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4a347-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4a347-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4a347-145">displayName</span></span>|<span data-ttu-id="4a347-146">String</span><span class="sxs-lookup"><span data-stu-id="4a347-146">String</span></span>|<span data-ttu-id="4a347-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="4a347-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a347-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4a347-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4a347-149">version</span><span class="sxs-lookup"><span data-stu-id="4a347-149">version</span></span>|<span data-ttu-id="4a347-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4a347-150">Int32</span></span>|<span data-ttu-id="4a347-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4a347-151">Version of the device configuration.</span></span> <span data-ttu-id="4a347-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4a347-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="4a347-153">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4a347-153">passcodeBlockSimple</span></span>|<span data-ttu-id="4a347-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a347-154">Boolean</span></span>|<span data-ttu-id="4a347-155">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4a347-155">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="4a347-156">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4a347-156">passcodeExpirationDays</span></span>|<span data-ttu-id="4a347-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4a347-157">Int32</span></span>|<span data-ttu-id="4a347-158">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="4a347-158">Number of days before the passcode expires.</span></span> <span data-ttu-id="4a347-159">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="4a347-159">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="4a347-160">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4a347-160">passcodeMinimumLength</span></span>|<span data-ttu-id="4a347-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4a347-161">Int32</span></span>|<span data-ttu-id="4a347-162">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="4a347-162">Minimum length of passcode.</span></span> <span data-ttu-id="4a347-163">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="4a347-163">Valid values 4 to 14</span></span>|
|<span data-ttu-id="4a347-164">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4a347-164">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4a347-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4a347-165">Int32</span></span>|<span data-ttu-id="4a347-166">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="4a347-166">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="4a347-167">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="4a347-167">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="4a347-168">Int32</span><span class="sxs-lookup"><span data-stu-id="4a347-168">Int32</span></span>|<span data-ttu-id="4a347-169">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="4a347-169">Number of previous passcodes to block.</span></span> <span data-ttu-id="4a347-170">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="4a347-170">Valid values 1 to 24</span></span>|
|<span data-ttu-id="4a347-171">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4a347-171">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="4a347-172">Int32</span><span class="sxs-lookup"><span data-stu-id="4a347-172">Int32</span></span>|<span data-ttu-id="4a347-173">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="4a347-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4a347-174">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="4a347-174">passcodeRequiredType</span></span>|<span data-ttu-id="4a347-175">String</span><span class="sxs-lookup"><span data-stu-id="4a347-175">String</span></span>|<span data-ttu-id="4a347-176">要求されるパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="4a347-176">The required passcode type.</span></span> <span data-ttu-id="4a347-177">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="4a347-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4a347-178">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="4a347-178">passcodeRequired</span></span>|<span data-ttu-id="4a347-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a347-179">Boolean</span></span>|<span data-ttu-id="4a347-180">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4a347-180">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="4a347-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="4a347-181">osMinimumVersion</span></span>|<span data-ttu-id="4a347-182">String</span><span class="sxs-lookup"><span data-stu-id="4a347-182">String</span></span>|<span data-ttu-id="4a347-183">最低限必要な iOS のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4a347-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="4a347-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="4a347-184">osMaximumVersion</span></span>|<span data-ttu-id="4a347-185">String</span><span class="sxs-lookup"><span data-stu-id="4a347-185">String</span></span>|<span data-ttu-id="4a347-186">iOS の最高バージョン。</span><span class="sxs-lookup"><span data-stu-id="4a347-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="4a347-187">securityBlockJailbrokenDevices</span><span class="sxs-lookup"><span data-stu-id="4a347-187">securityBlockJailbrokenDevices</span></span>|<span data-ttu-id="4a347-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a347-188">Boolean</span></span>|<span data-ttu-id="4a347-189">デバイスの脱獄またはルート化を認めません。</span><span class="sxs-lookup"><span data-stu-id="4a347-189">Devices must not be jailbroken or rooted.</span></span>|
|<span data-ttu-id="4a347-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4a347-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="4a347-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a347-191">Boolean</span></span>|<span data-ttu-id="4a347-192">デバイスへの脅威に対する保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a347-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="4a347-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4a347-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="4a347-194">String</span><span class="sxs-lookup"><span data-stu-id="4a347-194">String</span></span>|<span data-ttu-id="4a347-195">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="4a347-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="4a347-196">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="4a347-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="4a347-197">managedEmailProfileRequired</span><span class="sxs-lookup"><span data-stu-id="4a347-197">managedEmailProfileRequired</span></span>|<span data-ttu-id="4a347-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a347-198">Boolean</span></span>|<span data-ttu-id="4a347-199">管理された電子メール プロファイルを必要とするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4a347-199">Indicates whether or not to require a managed email profile.</span></span>|



## <a name="response"></a><span data-ttu-id="4a347-200">応答</span><span class="sxs-lookup"><span data-stu-id="4a347-200">Response</span></span>
<span data-ttu-id="4a347-201">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosCompliancePolicy](../resources/intune_deviceconfig_ioscompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4a347-201">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_ioscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a347-202">例</span><span class="sxs-lookup"><span data-stu-id="4a347-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a347-203">要求</span><span class="sxs-lookup"><span data-stu-id="4a347-203">Request</span></span>
<span data-ttu-id="4a347-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4a347-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 809

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```

### <a name="response"></a><span data-ttu-id="4a347-205">応答</span><span class="sxs-lookup"><span data-stu-id="4a347-205">Response</span></span>
<span data-ttu-id="4a347-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a347-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true
}
```



