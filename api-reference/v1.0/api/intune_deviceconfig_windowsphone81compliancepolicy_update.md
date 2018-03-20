# <a name="update-windowsphone81compliancepolicy"></a><span data-ttu-id="7f099-101">windowsPhone81CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="7f099-101">Update windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="7f099-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f099-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f099-103">[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f099-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f099-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f099-104">Prerequisites</span></span>
<span data-ttu-id="7f099-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f099-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f099-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f099-107">Permission type</span></span>|<span data-ttu-id="7f099-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f099-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f099-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f099-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7f099-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f099-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f099-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f099-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f099-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f099-112">Not supported.</span></span>|
|<span data-ttu-id="7f099-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f099-113">Application</span></span>|<span data-ttu-id="7f099-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f099-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f099-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f099-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="7f099-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f099-116">Request headers</span></span>
|<span data-ttu-id="7f099-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f099-117">Header</span></span>|<span data-ttu-id="7f099-118">値</span><span class="sxs-lookup"><span data-stu-id="7f099-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f099-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f099-119">Authorization</span></span>|<span data-ttu-id="7f099-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f099-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7f099-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7f099-121">Accept</span></span>|<span data-ttu-id="7f099-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7f099-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f099-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f099-123">Request body</span></span>
<span data-ttu-id="7f099-124">要求本文で、[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f099-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>

<span data-ttu-id="7f099-125">次の表に、[windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f099-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="7f099-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f099-126">Property</span></span>|<span data-ttu-id="7f099-127">型</span><span class="sxs-lookup"><span data-stu-id="7f099-127">Type</span></span>|<span data-ttu-id="7f099-128">説明</span><span class="sxs-lookup"><span data-stu-id="7f099-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f099-129">id</span><span class="sxs-lookup"><span data-stu-id="7f099-129">id</span></span>|<span data-ttu-id="7f099-130">String</span><span class="sxs-lookup"><span data-stu-id="7f099-130">String</span></span>|<span data-ttu-id="7f099-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f099-131">Name of the entity.</span></span> <span data-ttu-id="7f099-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f099-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f099-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f099-133">createdDateTime</span></span>|<span data-ttu-id="7f099-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f099-134">DateTimeOffset</span></span>|<span data-ttu-id="7f099-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f099-135">DateTime the object was created.</span></span> <span data-ttu-id="7f099-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f099-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f099-137">description</span><span class="sxs-lookup"><span data-stu-id="7f099-137">description</span></span>|<span data-ttu-id="7f099-138">String</span><span class="sxs-lookup"><span data-stu-id="7f099-138">String</span></span>|<span data-ttu-id="7f099-139">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="7f099-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7f099-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f099-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f099-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f099-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7f099-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f099-142">DateTimeOffset</span></span>|<span data-ttu-id="7f099-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f099-143">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="7f099-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f099-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f099-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7f099-145">displayName</span></span>|<span data-ttu-id="7f099-146">String</span><span class="sxs-lookup"><span data-stu-id="7f099-146">String</span></span>|<span data-ttu-id="7f099-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="7f099-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7f099-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f099-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f099-149">version</span><span class="sxs-lookup"><span data-stu-id="7f099-149">version</span></span>|<span data-ttu-id="7f099-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7f099-150">Int32</span></span>|<span data-ttu-id="7f099-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7f099-151">Version of the device configuration.</span></span> <span data-ttu-id="7f099-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f099-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7f099-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7f099-153">passwordBlockSimple</span></span>|<span data-ttu-id="7f099-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f099-154">Boolean</span></span>|<span data-ttu-id="7f099-155">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f099-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="7f099-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7f099-156">passwordExpirationDays</span></span>|<span data-ttu-id="7f099-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7f099-157">Int32</span></span>|<span data-ttu-id="7f099-158">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="7f099-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="7f099-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7f099-159">passwordMinimumLength</span></span>|<span data-ttu-id="7f099-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7f099-160">Int32</span></span>|<span data-ttu-id="7f099-161">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="7f099-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="7f099-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7f099-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7f099-163">Int32</span><span class="sxs-lookup"><span data-stu-id="7f099-163">Int32</span></span>|<span data-ttu-id="7f099-164">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="7f099-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7f099-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7f099-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7f099-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7f099-166">Int32</span></span>|<span data-ttu-id="7f099-167">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="7f099-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7f099-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7f099-168">passwordRequiredType</span></span>|<span data-ttu-id="7f099-169">String</span><span class="sxs-lookup"><span data-stu-id="7f099-169">String</span></span>|<span data-ttu-id="7f099-170">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="7f099-170">The required password type.</span></span> <span data-ttu-id="7f099-171">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="7f099-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7f099-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7f099-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7f099-173">Int32</span><span class="sxs-lookup"><span data-stu-id="7f099-173">Int32</span></span>|<span data-ttu-id="7f099-174">禁止する、以前のパスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="7f099-174">Number of previous passwords to block.</span></span> <span data-ttu-id="7f099-175">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="7f099-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7f099-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7f099-176">passwordRequired</span></span>|<span data-ttu-id="7f099-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f099-177">Boolean</span></span>|<span data-ttu-id="7f099-178">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f099-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="7f099-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7f099-179">osMinimumVersion</span></span>|<span data-ttu-id="7f099-180">String</span><span class="sxs-lookup"><span data-stu-id="7f099-180">String</span></span>|<span data-ttu-id="7f099-181">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="7f099-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="7f099-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7f099-182">osMaximumVersion</span></span>|<span data-ttu-id="7f099-183">String</span><span class="sxs-lookup"><span data-stu-id="7f099-183">String</span></span>|<span data-ttu-id="7f099-184">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="7f099-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="7f099-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7f099-185">storageRequireEncryption</span></span>|<span data-ttu-id="7f099-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f099-186">Boolean</span></span>|<span data-ttu-id="7f099-187">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="7f099-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="7f099-188">応答</span><span class="sxs-lookup"><span data-stu-id="7f099-188">Response</span></span>
<span data-ttu-id="7f099-189">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f099-189">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f099-190">例</span><span class="sxs-lookup"><span data-stu-id="7f099-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f099-191">要求</span><span class="sxs-lookup"><span data-stu-id="7f099-191">Request</span></span>
<span data-ttu-id="7f099-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f099-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="7f099-193">応答</span><span class="sxs-lookup"><span data-stu-id="7f099-193">Response</span></span>
<span data-ttu-id="7f099-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f099-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



