# <a name="create-windows81compliancepolicy"></a><span data-ttu-id="0fb3d-101">windows81CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="0fb3d-101">Create windows81CompliancePolicy</span></span>

> <span data-ttu-id="0fb3d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fb3d-103">新しい [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-103">Create a new [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0fb3d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0fb3d-104">Prerequisites</span></span>
<span data-ttu-id="0fb3d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0fb3d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0fb3d-107">Permission type</span></span>|<span data-ttu-id="0fb3d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0fb3d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fb3d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0fb3d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0fb3d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb3d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fb3d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0fb3d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fb3d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-112">Not supported.</span></span>|
|<span data-ttu-id="0fb3d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0fb3d-113">Application</span></span>|<span data-ttu-id="0fb3d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fb3d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fb3d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="0fb3d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fb3d-116">Request headers</span></span>
|<span data-ttu-id="0fb3d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fb3d-117">Header</span></span>|<span data-ttu-id="0fb3d-118">値</span><span class="sxs-lookup"><span data-stu-id="0fb3d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fb3d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fb3d-119">Authorization</span></span>|<span data-ttu-id="0fb3d-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fb3d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0fb3d-121">Accept</span></span>|<span data-ttu-id="0fb3d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0fb3d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fb3d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0fb3d-123">Request body</span></span>
<span data-ttu-id="0fb3d-124">要求本文で、windows81CompliancePolicy オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-124">In the request body, supply a JSON representation for the windows81CompliancePolicy object.</span></span>

<span data-ttu-id="0fb3d-125">次の表に、windows81CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-125">The following table shows the properties that are required when you create the windows81CompliancePolicy.</span></span>

|<span data-ttu-id="0fb3d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fb3d-126">Property</span></span>|<span data-ttu-id="0fb3d-127">型</span><span class="sxs-lookup"><span data-stu-id="0fb3d-127">Type</span></span>|<span data-ttu-id="0fb3d-128">説明</span><span class="sxs-lookup"><span data-stu-id="0fb3d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb3d-129">id</span><span class="sxs-lookup"><span data-stu-id="0fb3d-129">id</span></span>|<span data-ttu-id="0fb3d-130">String</span><span class="sxs-lookup"><span data-stu-id="0fb3d-130">String</span></span>|<span data-ttu-id="0fb3d-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-131">Key of the entity.</span></span> <span data-ttu-id="0fb3d-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0fb3d-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb3d-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fb3d-133">createdDateTime</span></span>|<span data-ttu-id="0fb3d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fb3d-134">DateTimeOffset</span></span>|<span data-ttu-id="0fb3d-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-135">DateTime the object was created.</span></span> <span data-ttu-id="0fb3d-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0fb3d-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb3d-137">description</span><span class="sxs-lookup"><span data-stu-id="0fb3d-137">description</span></span>|<span data-ttu-id="0fb3d-138">String</span><span class="sxs-lookup"><span data-stu-id="0fb3d-138">String</span></span>|<span data-ttu-id="0fb3d-139">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0fb3d-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0fb3d-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb3d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fb3d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0fb3d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fb3d-142">DateTimeOffset</span></span>|<span data-ttu-id="0fb3d-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-143">DateTime the object was last modified.</span></span> <span data-ttu-id="0fb3d-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0fb3d-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb3d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0fb3d-145">displayName</span></span>|<span data-ttu-id="0fb3d-146">String</span><span class="sxs-lookup"><span data-stu-id="0fb3d-146">String</span></span>|<span data-ttu-id="0fb3d-147">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0fb3d-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0fb3d-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb3d-149">version</span><span class="sxs-lookup"><span data-stu-id="0fb3d-149">version</span></span>|<span data-ttu-id="0fb3d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb3d-150">Int32</span></span>|<span data-ttu-id="0fb3d-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-151">Version of the device configuration.</span></span> <span data-ttu-id="0fb3d-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0fb3d-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="0fb3d-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0fb3d-153">passwordRequired</span></span>|<span data-ttu-id="0fb3d-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fb3d-154">Boolean</span></span>|<span data-ttu-id="0fb3d-155">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="0fb3d-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0fb3d-156">passwordBlockSimple</span></span>|<span data-ttu-id="0fb3d-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fb3d-157">Boolean</span></span>|<span data-ttu-id="0fb3d-158">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="0fb3d-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0fb3d-159">passwordExpirationDays</span></span>|<span data-ttu-id="0fb3d-160">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb3d-160">Int32</span></span>|<span data-ttu-id="0fb3d-161">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-161">Password expiration in days.</span></span>|
|<span data-ttu-id="0fb3d-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0fb3d-162">passwordMinimumLength</span></span>|<span data-ttu-id="0fb3d-163">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb3d-163">Int32</span></span>|<span data-ttu-id="0fb3d-164">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-164">The minimum password length.</span></span>|
|<span data-ttu-id="0fb3d-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0fb3d-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0fb3d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb3d-166">Int32</span></span>|<span data-ttu-id="0fb3d-167">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="0fb3d-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0fb3d-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0fb3d-169">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb3d-169">Int32</span></span>|<span data-ttu-id="0fb3d-170">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="0fb3d-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0fb3d-171">passwordRequiredType</span></span>|[<span data-ttu-id="0fb3d-172">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0fb3d-172">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="0fb3d-173">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-173">The required password type.</span></span> <span data-ttu-id="0fb3d-174">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0fb3d-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0fb3d-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0fb3d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0fb3d-176">Int32</span></span>|<span data-ttu-id="0fb3d-177">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="0fb3d-178">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="0fb3d-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="0fb3d-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="0fb3d-179">osMinimumVersion</span></span>|<span data-ttu-id="0fb3d-180">String</span><span class="sxs-lookup"><span data-stu-id="0fb3d-180">String</span></span>|<span data-ttu-id="0fb3d-181">Windows 8.1 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="0fb3d-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="0fb3d-182">osMaximumVersion</span></span>|<span data-ttu-id="0fb3d-183">String</span><span class="sxs-lookup"><span data-stu-id="0fb3d-183">String</span></span>|<span data-ttu-id="0fb3d-184">Windows 8.1 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="0fb3d-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="0fb3d-185">storageRequireEncryption</span></span>|<span data-ttu-id="0fb3d-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fb3d-186">Boolean</span></span>|<span data-ttu-id="0fb3d-187">Windows 8.1 のデバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="0fb3d-188">応答</span><span class="sxs-lookup"><span data-stu-id="0fb3d-188">Response</span></span>
<span data-ttu-id="0fb3d-189">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-189">If successful, this method returns a `201 Created` response code and a [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fb3d-190">例</span><span class="sxs-lookup"><span data-stu-id="0fb3d-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="0fb3d-191">要求</span><span class="sxs-lookup"><span data-stu-id="0fb3d-191">Request</span></span>
<span data-ttu-id="0fb3d-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="0fb3d-193">応答</span><span class="sxs-lookup"><span data-stu-id="0fb3d-193">Response</span></span>
<span data-ttu-id="0fb3d-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0fb3d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 774

{
  "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
  "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



