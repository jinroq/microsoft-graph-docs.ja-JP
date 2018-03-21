# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="6b401-101">macOSCompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="6b401-101">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="6b401-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b401-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b401-103">[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6b401-103">Update the properties of a [calendar](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b401-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="6b401-104">Prerequisites</span></span>
<span data-ttu-id="6b401-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b401-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b401-107">Permission type</span></span>|<span data-ttu-id="6b401-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b401-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b401-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b401-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6b401-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b401-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b401-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b401-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b401-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b401-112">Not supported.</span></span>|
|<span data-ttu-id="6b401-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b401-113">Application</span></span>|<span data-ttu-id="6b401-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b401-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b401-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b401-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="6b401-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b401-116">Request headers</span></span>
|<span data-ttu-id="6b401-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b401-117">Header</span></span>|<span data-ttu-id="6b401-118">値</span><span class="sxs-lookup"><span data-stu-id="6b401-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b401-119">承認</span><span class="sxs-lookup"><span data-stu-id="6b401-119">Authorization</span></span>|<span data-ttu-id="6b401-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="6b401-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6b401-121">承諾</span><span class="sxs-lookup"><span data-stu-id="6b401-121">Accept</span></span>|<span data-ttu-id="6b401-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6b401-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b401-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b401-123">Request body</span></span>
<span data-ttu-id="6b401-124">要求本文で、[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b401-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="6b401-125">次の表に、[macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6b401-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="6b401-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b401-126">Property</span></span>|<span data-ttu-id="6b401-127">型</span><span class="sxs-lookup"><span data-stu-id="6b401-127">Type</span></span>|<span data-ttu-id="6b401-128">説明</span><span class="sxs-lookup"><span data-stu-id="6b401-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b401-129">id</span><span class="sxs-lookup"><span data-stu-id="6b401-129">id</span></span>|<span data-ttu-id="6b401-130">String</span><span class="sxs-lookup"><span data-stu-id="6b401-130">String</span></span>|<span data-ttu-id="6b401-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6b401-131">Name of the entity.</span></span> <span data-ttu-id="6b401-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b401-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b401-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b401-133">createdDateTime</span></span>|<span data-ttu-id="6b401-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b401-134">DateTimeOffset</span></span>|<span data-ttu-id="6b401-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6b401-135">DateTime the object was created.</span></span> <span data-ttu-id="6b401-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b401-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b401-137">description</span><span class="sxs-lookup"><span data-stu-id="6b401-137">description</span></span>|<span data-ttu-id="6b401-138">String</span><span class="sxs-lookup"><span data-stu-id="6b401-138">String</span></span>|<span data-ttu-id="6b401-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="6b401-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b401-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b401-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b401-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b401-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6b401-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b401-142">DateTimeOffset</span></span>|<span data-ttu-id="6b401-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="6b401-143">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="6b401-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b401-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b401-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6b401-145">displayName</span></span>|<span data-ttu-id="6b401-146">String</span><span class="sxs-lookup"><span data-stu-id="6b401-146">String</span></span>|<span data-ttu-id="6b401-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="6b401-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b401-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b401-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b401-149">version</span><span class="sxs-lookup"><span data-stu-id="6b401-149">version</span></span>|<span data-ttu-id="6b401-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6b401-150">Int32</span></span>|<span data-ttu-id="6b401-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6b401-151">Version of the device configuration.</span></span> <span data-ttu-id="6b401-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b401-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="6b401-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="6b401-153">passwordRequired</span></span>|<span data-ttu-id="6b401-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b401-154">Boolean</span></span>|<span data-ttu-id="6b401-155">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b401-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="6b401-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6b401-156">passwordBlockSimple</span></span>|<span data-ttu-id="6b401-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b401-157">Boolean</span></span>|<span data-ttu-id="6b401-158">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b401-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="6b401-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6b401-159">passwordExpirationDays</span></span>|<span data-ttu-id="6b401-160">Int32</span><span class="sxs-lookup"><span data-stu-id="6b401-160">Int32</span></span>|<span data-ttu-id="6b401-161">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="6b401-161">Number of days before the password expires.</span></span> <span data-ttu-id="6b401-162">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="6b401-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b401-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6b401-163">passwordMinimumLength</span></span>|<span data-ttu-id="6b401-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6b401-164">Int32</span></span>|<span data-ttu-id="6b401-165">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="6b401-165">Minimum length of password.</span></span> <span data-ttu-id="6b401-166">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="6b401-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6b401-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6b401-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6b401-168">Int32</span><span class="sxs-lookup"><span data-stu-id="6b401-168">Int32</span></span>|<span data-ttu-id="6b401-169">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="6b401-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="6b401-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="6b401-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="6b401-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6b401-171">Int32</span></span>|<span data-ttu-id="6b401-172">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="6b401-172">Number of previous passwords to block.</span></span> <span data-ttu-id="6b401-173">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="6b401-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6b401-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6b401-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="6b401-175">Int32</span><span class="sxs-lookup"><span data-stu-id="6b401-175">Int32</span></span>|<span data-ttu-id="6b401-176">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="6b401-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="6b401-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="6b401-177">passwordRequiredType</span></span>|<span data-ttu-id="6b401-178">String</span><span class="sxs-lookup"><span data-stu-id="6b401-178">String</span></span>|<span data-ttu-id="6b401-179">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="6b401-179">The required password type.</span></span> <span data-ttu-id="6b401-180">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="6b401-180">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6b401-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="6b401-181">osMinimumVersion</span></span>|<span data-ttu-id="6b401-182">String</span><span class="sxs-lookup"><span data-stu-id="6b401-182">String</span></span>|<span data-ttu-id="6b401-183">最小の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="6b401-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="6b401-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="6b401-184">osMaximumVersion</span></span>|<span data-ttu-id="6b401-185">String</span><span class="sxs-lookup"><span data-stu-id="6b401-185">String</span></span>|<span data-ttu-id="6b401-186">最大の iOS バージョン。</span><span class="sxs-lookup"><span data-stu-id="6b401-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="6b401-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6b401-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="6b401-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b401-188">Boolean</span></span>|<span data-ttu-id="6b401-189">デバイスでシステム整合性の保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b401-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="6b401-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="6b401-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="6b401-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b401-191">Boolean</span></span>|<span data-ttu-id="6b401-192">デバイスの脅威保護が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b401-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="6b401-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="6b401-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|<span data-ttu-id="6b401-194">String</span><span class="sxs-lookup"><span data-stu-id="6b401-194">String</span></span>|<span data-ttu-id="6b401-195">Mobile Threat Protection に、コンプライアンス違反をレポートするための最小のリスク レベルを要求します。</span><span class="sxs-lookup"><span data-stu-id="6b401-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="6b401-196">可能な値は、`unavailable`、`secured`、`low`、`medium`、`high`、`notSet` です。</span><span class="sxs-lookup"><span data-stu-id="6b401-196">Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.</span></span>|
|<span data-ttu-id="6b401-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="6b401-197">storageRequireEncryption</span></span>|<span data-ttu-id="6b401-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b401-198">Boolean</span></span>|<span data-ttu-id="6b401-199">Mac OS デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="6b401-199">Require encryption on Mac OS devices.</span></span>|



## <a name="response"></a><span data-ttu-id="6b401-200">応答</span><span class="sxs-lookup"><span data-stu-id="6b401-200">Response</span></span>
<span data-ttu-id="6b401-201">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="6b401-201">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b401-202">例</span><span class="sxs-lookup"><span data-stu-id="6b401-202">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b401-203">要求</span><span class="sxs-lookup"><span data-stu-id="6b401-203">Request</span></span>
<span data-ttu-id="6b401-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b401-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 750

{
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
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="6b401-205">応答</span><span class="sxs-lookup"><span data-stu-id="6b401-205">Response</span></span>
<span data-ttu-id="6b401-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6b401-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

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
  "storageRequireEncryption": true
}
```



