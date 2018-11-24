# <a name="create-windowsphone81compliancepolicy"></a><span data-ttu-id="7a5b4-101">windowsPhone81CompliancePolicy の作成</span><span class="sxs-lookup"><span data-stu-id="7a5b4-101">Create windowsPhone81CompliancePolicy</span></span>

> <span data-ttu-id="7a5b4-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a5b4-103">新しい [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-103">Create a new [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a5b4-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7a5b4-104">Prerequisites</span></span>
<span data-ttu-id="7a5b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7a5b4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7a5b4-107">Permission type</span></span>|<span data-ttu-id="7a5b4-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7a5b4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a5b4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7a5b4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7a5b4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a5b4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a5b4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7a5b4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a5b4-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-112">Not supported.</span></span>|
|<span data-ttu-id="7a5b4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7a5b4-113">Application</span></span>|<span data-ttu-id="7a5b4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a5b4-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7a5b4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="7a5b4-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a5b4-116">Request headers</span></span>
|<span data-ttu-id="7a5b4-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7a5b4-117">Header</span></span>|<span data-ttu-id="7a5b4-118">値</span><span class="sxs-lookup"><span data-stu-id="7a5b4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a5b4-119">承認</span><span class="sxs-lookup"><span data-stu-id="7a5b4-119">Authorization</span></span>|<span data-ttu-id="7a5b4-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a5b4-121">承諾</span><span class="sxs-lookup"><span data-stu-id="7a5b4-121">Accept</span></span>|<span data-ttu-id="7a5b4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7a5b4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a5b4-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7a5b4-123">Request body</span></span>
<span data-ttu-id="7a5b4-124">要求本文で、windowsPhone81CompliancePolicy オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-124">In the request body, supply a JSON representation for the windowsPhone81CompliancePolicy object.</span></span>

<span data-ttu-id="7a5b4-125">次の表に、windowsPhone81CompliancePolicy の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-125">The following table shows the properties that are required when you create the windowsPhone81CompliancePolicy.</span></span>

|<span data-ttu-id="7a5b4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a5b4-126">Property</span></span>|<span data-ttu-id="7a5b4-127">型</span><span class="sxs-lookup"><span data-stu-id="7a5b4-127">Type</span></span>|<span data-ttu-id="7a5b4-128">説明</span><span class="sxs-lookup"><span data-stu-id="7a5b4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a5b4-129">id</span><span class="sxs-lookup"><span data-stu-id="7a5b4-129">id</span></span>|<span data-ttu-id="7a5b4-130">String</span><span class="sxs-lookup"><span data-stu-id="7a5b4-130">String</span></span>|<span data-ttu-id="7a5b4-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-131">Key of the entity.</span></span> <span data-ttu-id="7a5b4-132">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a5b4-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7a5b4-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a5b4-133">createdDateTime</span></span>|<span data-ttu-id="7a5b4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a5b4-134">DateTimeOffset</span></span>|<span data-ttu-id="7a5b4-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-135">DateTime the object was created.</span></span> <span data-ttu-id="7a5b4-136">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a5b4-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7a5b4-137">description</span><span class="sxs-lookup"><span data-stu-id="7a5b4-137">description</span></span>|<span data-ttu-id="7a5b4-138">String</span><span class="sxs-lookup"><span data-stu-id="7a5b4-138">String</span></span>|<span data-ttu-id="7a5b4-139">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7a5b4-140">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a5b4-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7a5b4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a5b4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7a5b4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a5b4-142">DateTimeOffset</span></span>|<span data-ttu-id="7a5b4-143">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-143">DateTime the object was last modified.</span></span> <span data-ttu-id="7a5b4-144">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a5b4-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7a5b4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="7a5b4-145">displayName</span></span>|<span data-ttu-id="7a5b4-146">String</span><span class="sxs-lookup"><span data-stu-id="7a5b4-146">String</span></span>|<span data-ttu-id="7a5b4-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7a5b4-148">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a5b4-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7a5b4-149">version</span><span class="sxs-lookup"><span data-stu-id="7a5b4-149">version</span></span>|<span data-ttu-id="7a5b4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7a5b4-150">Int32</span></span>|<span data-ttu-id="7a5b4-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-151">Version of the device configuration.</span></span> <span data-ttu-id="7a5b4-152">[deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7a5b4-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="7a5b4-153">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7a5b4-153">passwordBlockSimple</span></span>|<span data-ttu-id="7a5b4-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a5b4-154">Boolean</span></span>|<span data-ttu-id="7a5b4-155">カレンダーの同期を禁止するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-155">Whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="7a5b4-156">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7a5b4-156">passwordExpirationDays</span></span>|<span data-ttu-id="7a5b4-157">Int32</span><span class="sxs-lookup"><span data-stu-id="7a5b4-157">Int32</span></span>|<span data-ttu-id="7a5b4-158">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-158">Number of days before the password expires.</span></span>|
|<span data-ttu-id="7a5b4-159">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7a5b4-159">passwordMinimumLength</span></span>|<span data-ttu-id="7a5b4-160">Int32</span><span class="sxs-lookup"><span data-stu-id="7a5b4-160">Int32</span></span>|<span data-ttu-id="7a5b4-161">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-161">Minimum length of passwords.</span></span>|
|<span data-ttu-id="7a5b4-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7a5b4-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7a5b4-163">Int32</span><span class="sxs-lookup"><span data-stu-id="7a5b4-163">Int32</span></span>|<span data-ttu-id="7a5b4-164">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="7a5b4-165">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7a5b4-165">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="7a5b4-166">Int32</span><span class="sxs-lookup"><span data-stu-id="7a5b4-166">Int32</span></span>|<span data-ttu-id="7a5b4-167">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-167">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="7a5b4-168">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="7a5b4-168">passwordRequiredType</span></span>|[<span data-ttu-id="7a5b4-169">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7a5b4-169">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="7a5b4-170">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-170">The required password type.</span></span> <span data-ttu-id="7a5b4-171">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-171">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7a5b4-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="7a5b4-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="7a5b4-173">Int32</span><span class="sxs-lookup"><span data-stu-id="7a5b4-173">Int32</span></span>|<span data-ttu-id="7a5b4-174">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-174">Number of previous passwords to block.</span></span> <span data-ttu-id="7a5b4-175">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="7a5b4-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="7a5b4-176">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="7a5b4-176">passwordRequired</span></span>|<span data-ttu-id="7a5b4-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a5b4-177">Boolean</span></span>|<span data-ttu-id="7a5b4-178">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-178">Whether or not to require a password.</span></span>|
|<span data-ttu-id="7a5b4-179">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="7a5b4-179">osMinimumVersion</span></span>|<span data-ttu-id="7a5b4-180">String</span><span class="sxs-lookup"><span data-stu-id="7a5b4-180">String</span></span>|<span data-ttu-id="7a5b4-181">Windows Phone の最小バージョン。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-181">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="7a5b4-182">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="7a5b4-182">osMaximumVersion</span></span>|<span data-ttu-id="7a5b4-183">String</span><span class="sxs-lookup"><span data-stu-id="7a5b4-183">String</span></span>|<span data-ttu-id="7a5b4-184">Windows Phone の最大バージョン。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-184">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="7a5b4-185">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="7a5b4-185">storageRequireEncryption</span></span>|<span data-ttu-id="7a5b4-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a5b4-186">Boolean</span></span>|<span data-ttu-id="7a5b4-187">Windows Phone デバイスでの暗号化を要求します。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-187">Require encryption on windows phone devices.</span></span>|



## <a name="response"></a><span data-ttu-id="7a5b4-188">応答</span><span class="sxs-lookup"><span data-stu-id="7a5b4-188">Response</span></span>
<span data-ttu-id="7a5b4-189">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-189">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a5b4-190">例</span><span class="sxs-lookup"><span data-stu-id="7a5b4-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a5b4-191">要求</span><span class="sxs-lookup"><span data-stu-id="7a5b4-191">Request</span></span>
<span data-ttu-id="7a5b4-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 607

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="7a5b4-193">応答</span><span class="sxs-lookup"><span data-stu-id="7a5b4-193">Response</span></span>
<span data-ttu-id="7a5b4-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7a5b4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



