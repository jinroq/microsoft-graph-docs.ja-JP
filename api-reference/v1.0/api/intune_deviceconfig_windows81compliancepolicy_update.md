# <a name="update-windows81compliancepolicy"></a><span data-ttu-id="b6538-101">windows81CompliancePolicy の更新</span><span class="sxs-lookup"><span data-stu-id="b6538-101">Update windows81CompliancePolicy</span></span>

> <span data-ttu-id="b6538-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6538-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6538-103">[windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b6538-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6538-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b6538-104">Prerequisites</span></span>
<span data-ttu-id="b6538-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6538-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b6538-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6538-107">Permission type</span></span>|<span data-ttu-id="b6538-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6538-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6538-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6538-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b6538-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6538-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6538-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6538-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6538-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6538-112">Not supported.</span></span>|
|<span data-ttu-id="b6538-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6538-113">Application</span></span>|<span data-ttu-id="b6538-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6538-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6538-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6538-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="b6538-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6538-116">Request headers</span></span>
|<span data-ttu-id="b6538-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6538-117">Header</span></span>|<span data-ttu-id="b6538-118">値</span><span class="sxs-lookup"><span data-stu-id="b6538-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6538-119">承認</span><span class="sxs-lookup"><span data-stu-id="b6538-119">Authorization</span></span>|<span data-ttu-id="b6538-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="b6538-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b6538-121">承諾</span><span class="sxs-lookup"><span data-stu-id="b6538-121">Accept</span></span>|<span data-ttu-id="b6538-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b6538-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6538-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6538-123">Request body</span></span>
<span data-ttu-id="b6538-124">要求本文で、[windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6538-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows81compliancepolicy.md) object.</span></span>

<span data-ttu-id="b6538-125">次の表に、[windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b6538-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b6538-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6538-126">Property</span></span>|<span data-ttu-id="b6538-127">型</span><span class="sxs-lookup"><span data-stu-id="b6538-127">Type</span></span>|<span data-ttu-id="b6538-128">説明</span><span class="sxs-lookup"><span data-stu-id="b6538-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6538-129">id</span><span class="sxs-lookup"><span data-stu-id="b6538-129">id</span></span>|<span data-ttu-id="b6538-130">String</span><span class="sxs-lookup"><span data-stu-id="b6538-130">String</span></span>|<span data-ttu-id="b6538-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b6538-131">Name of the entity.</span></span> <span data-ttu-id="b6538-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6538-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6538-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6538-133">createdDateTime</span></span>|<span data-ttu-id="b6538-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6538-134">DateTimeOffset</span></span>|<span data-ttu-id="b6538-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b6538-135">DateTime the object was created.</span></span> <span data-ttu-id="b6538-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6538-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6538-137">description</span><span class="sxs-lookup"><span data-stu-id="b6538-137">description</span></span>|<span data-ttu-id="b6538-138">String</span><span class="sxs-lookup"><span data-stu-id="b6538-138">String</span></span>|<span data-ttu-id="b6538-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="b6538-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6538-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6538-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6538-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6538-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b6538-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6538-142">DateTimeOffset</span></span>|<span data-ttu-id="b6538-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b6538-143">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="b6538-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6538-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6538-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b6538-145">displayName</span></span>|<span data-ttu-id="b6538-146">String</span><span class="sxs-lookup"><span data-stu-id="b6538-146">String</span></span>|<span data-ttu-id="b6538-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="b6538-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6538-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6538-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6538-149">version</span><span class="sxs-lookup"><span data-stu-id="b6538-149">version</span></span>|<span data-ttu-id="b6538-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b6538-150">Int32</span></span>|<span data-ttu-id="b6538-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b6538-151">Version of the device configuration.</span></span> <span data-ttu-id="b6538-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b6538-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="b6538-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b6538-153">passwordRequired</span></span>|<span data-ttu-id="b6538-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6538-154">Boolean</span></span>|<span data-ttu-id="b6538-155">Windows デバイスのロックを解除するパスワードを要求します。</span><span class="sxs-lookup"><span data-stu-id="b6538-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="b6538-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b6538-156">passwordBlockSimple</span></span>|<span data-ttu-id="b6538-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6538-157">Boolean</span></span>|<span data-ttu-id="b6538-158">単純なパスワードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6538-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="b6538-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b6538-159">passwordExpirationDays</span></span>|<span data-ttu-id="b6538-160">Int32</span><span class="sxs-lookup"><span data-stu-id="b6538-160">Int32</span></span>|<span data-ttu-id="b6538-161">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="b6538-161">Password expiration in days.</span></span>|
|<span data-ttu-id="b6538-162">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b6538-162">passwordMinimumLength</span></span>|<span data-ttu-id="b6538-163">Int32</span><span class="sxs-lookup"><span data-stu-id="b6538-163">Int32</span></span>|<span data-ttu-id="b6538-164">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="b6538-164">The minimum password length.</span></span>|
|<span data-ttu-id="b6538-165">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b6538-165">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b6538-166">Int32</span><span class="sxs-lookup"><span data-stu-id="b6538-166">Int32</span></span>|<span data-ttu-id="b6538-167">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="b6538-167">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="b6538-168">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b6538-168">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b6538-169">Int32</span><span class="sxs-lookup"><span data-stu-id="b6538-169">Int32</span></span>|<span data-ttu-id="b6538-170">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="b6538-170">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b6538-171">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b6538-171">passwordRequiredType</span></span>|<span data-ttu-id="b6538-172">String</span><span class="sxs-lookup"><span data-stu-id="b6538-172">String</span></span>|<span data-ttu-id="b6538-173">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="b6538-173">The required password type.</span></span> <span data-ttu-id="b6538-174">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="b6538-174">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b6538-175">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b6538-175">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b6538-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b6538-176">Int32</span></span>|<span data-ttu-id="b6538-177">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="b6538-177">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="b6538-178">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="b6538-178">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b6538-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b6538-179">osMinimumVersion</span></span>|<span data-ttu-id="b6538-180">String</span><span class="sxs-lookup"><span data-stu-id="b6538-180">String</span></span>|<span data-ttu-id="b6538-181">Windows 8.1 の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="b6538-181">Minimum Windows 8.1 version.</span></span>|
|<span data-ttu-id="b6538-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b6538-182">osMaximumVersion</span></span>|<span data-ttu-id="b6538-183">String</span><span class="sxs-lookup"><span data-stu-id="b6538-183">String</span></span>|<span data-ttu-id="b6538-184">Windows 8.1 の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="b6538-184">Maximum Windows 8.1 version.</span></span>|
|<span data-ttu-id="b6538-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b6538-185">storageRequireEncryption</span></span>|<span data-ttu-id="b6538-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6538-186">Boolean</span></span>|<span data-ttu-id="b6538-187">Windows 8.1 のデバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b6538-187">Indicates whether or not to require encryption on a windows 8.1 device.</span></span>|



## <a name="response"></a><span data-ttu-id="b6538-188">応答</span><span class="sxs-lookup"><span data-stu-id="b6538-188">Response</span></span>
<span data-ttu-id="b6538-189">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows81CompliancePolicy](../resources/intune_deviceconfig_windows81compliancepolicy.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="b6538-189">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6538-190">例</span><span class="sxs-lookup"><span data-stu-id="b6538-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6538-191">要求</span><span class="sxs-lookup"><span data-stu-id="b6538-191">Request</span></span>
<span data-ttu-id="b6538-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6538-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

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
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="b6538-193">応答</span><span class="sxs-lookup"><span data-stu-id="b6538-193">Response</span></span>
<span data-ttu-id="b6538-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6538-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



