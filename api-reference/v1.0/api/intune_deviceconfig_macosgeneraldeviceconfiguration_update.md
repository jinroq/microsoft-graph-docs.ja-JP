# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="cfe1f-101">macOSGeneralDeviceConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="cfe1f-101">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="cfe1f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfe1f-103">[macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-103">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cfe1f-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="cfe1f-104">Prerequisites</span></span>
<span data-ttu-id="cfe1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cfe1f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfe1f-107">Permission type</span></span>|<span data-ttu-id="cfe1f-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfe1f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfe1f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe1f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cfe1f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe1f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cfe1f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe1f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfe1f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-112">Not supported.</span></span>|
|<span data-ttu-id="cfe1f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfe1f-113">Application</span></span>|<span data-ttu-id="cfe1f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfe1f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfe1f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cfe1f-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe1f-116">Request headers</span></span>
|<span data-ttu-id="cfe1f-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe1f-117">Header</span></span>|<span data-ttu-id="cfe1f-118">値</span><span class="sxs-lookup"><span data-stu-id="cfe1f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfe1f-119">承認</span><span class="sxs-lookup"><span data-stu-id="cfe1f-119">Authorization</span></span>|<span data-ttu-id="cfe1f-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfe1f-121">承諾</span><span class="sxs-lookup"><span data-stu-id="cfe1f-121">Accept</span></span>|<span data-ttu-id="cfe1f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cfe1f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfe1f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cfe1f-123">Request body</span></span>
<span data-ttu-id="cfe1f-124">要求本文で、[macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-124">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="cfe1f-125">次の表に、[macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-125">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="cfe1f-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfe1f-126">Property</span></span>|<span data-ttu-id="cfe1f-127">型</span><span class="sxs-lookup"><span data-stu-id="cfe1f-127">Type</span></span>|<span data-ttu-id="cfe1f-128">説明</span><span class="sxs-lookup"><span data-stu-id="cfe1f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe1f-129">id</span><span class="sxs-lookup"><span data-stu-id="cfe1f-129">id</span></span>|<span data-ttu-id="cfe1f-130">String</span><span class="sxs-lookup"><span data-stu-id="cfe1f-130">String</span></span>|<span data-ttu-id="cfe1f-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-131">Key of the entity.</span></span> <span data-ttu-id="cfe1f-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe1f-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe1f-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe1f-133">lastModifiedDateTime</span></span>|<span data-ttu-id="cfe1f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe1f-134">DateTimeOffset</span></span>|<span data-ttu-id="cfe1f-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-135">DateTime the object was last modified.</span></span> <span data-ttu-id="cfe1f-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe1f-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe1f-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe1f-137">createdDateTime</span></span>|<span data-ttu-id="cfe1f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe1f-138">DateTimeOffset</span></span>|<span data-ttu-id="cfe1f-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-139">DateTime the object was created.</span></span> <span data-ttu-id="cfe1f-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe1f-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe1f-141">description</span><span class="sxs-lookup"><span data-stu-id="cfe1f-141">description</span></span>|<span data-ttu-id="cfe1f-142">String</span><span class="sxs-lookup"><span data-stu-id="cfe1f-142">String</span></span>|<span data-ttu-id="cfe1f-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cfe1f-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe1f-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe1f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="cfe1f-145">displayName</span></span>|<span data-ttu-id="cfe1f-146">String</span><span class="sxs-lookup"><span data-stu-id="cfe1f-146">String</span></span>|<span data-ttu-id="cfe1f-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cfe1f-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe1f-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe1f-149">version</span><span class="sxs-lookup"><span data-stu-id="cfe1f-149">version</span></span>|<span data-ttu-id="cfe1f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe1f-150">Int32</span></span>|<span data-ttu-id="cfe1f-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-151">Version of the device configuration.</span></span> <span data-ttu-id="cfe1f-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cfe1f-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cfe1f-153">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="cfe1f-153">compliantAppsList</span></span>|<span data-ttu-id="cfe1f-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cfe1f-154">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="cfe1f-155">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-155">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="cfe1f-156">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-156">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="cfe1f-157">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="cfe1f-157">compliantAppListType</span></span>|[<span data-ttu-id="cfe1f-158">appListType</span><span class="sxs-lookup"><span data-stu-id="cfe1f-158">appListType</span></span>](../resources/intune_deviceconfig_applisttype.md)|<span data-ttu-id="cfe1f-159">CompliantAppsList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-159">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="cfe1f-160">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-160">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="cfe1f-161">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="cfe1f-161">emailInDomainSuffixes</span></span>|<span data-ttu-id="cfe1f-162">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cfe1f-162">String collection</span></span>|<span data-ttu-id="cfe1f-163">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-163">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="cfe1f-164">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cfe1f-164">passwordBlockSimple</span></span>|<span data-ttu-id="cfe1f-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfe1f-165">Boolean</span></span>|<span data-ttu-id="cfe1f-166">単純なパスワードを禁止します。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-166">Block simple passwords.</span></span>|
|<span data-ttu-id="cfe1f-167">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cfe1f-167">passwordExpirationDays</span></span>|<span data-ttu-id="cfe1f-168">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe1f-168">Int32</span></span>|<span data-ttu-id="cfe1f-169">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-169">Number of days before the password expires.</span></span>|
|<span data-ttu-id="cfe1f-170">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cfe1f-170">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="cfe1f-171">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe1f-171">Int32</span></span>|<span data-ttu-id="cfe1f-172">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-172">Number of character sets a password must contain.</span></span> <span data-ttu-id="cfe1f-173">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="cfe1f-173">Valid values 0 to 4</span></span>|
|<span data-ttu-id="cfe1f-174">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cfe1f-174">passwordMinimumLength</span></span>|<span data-ttu-id="cfe1f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe1f-175">Int32</span></span>|<span data-ttu-id="cfe1f-176">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-176">Minimum length of passwords.</span></span>|
|<span data-ttu-id="cfe1f-177">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cfe1f-177">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cfe1f-178">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe1f-178">Int32</span></span>|<span data-ttu-id="cfe1f-179">パスワードが要求されるまでに必要な非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-179">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="cfe1f-180">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="cfe1f-180">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="cfe1f-181">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe1f-181">Int32</span></span>|<span data-ttu-id="cfe1f-182">画面がタイムアウトになるまでに必要な非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-182">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="cfe1f-183">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cfe1f-183">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cfe1f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cfe1f-184">Int32</span></span>|<span data-ttu-id="cfe1f-185">禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-185">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="cfe1f-186">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cfe1f-186">passwordRequiredType</span></span>|[<span data-ttu-id="cfe1f-187">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cfe1f-187">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="cfe1f-188">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-188">Type of password that is required.</span></span> <span data-ttu-id="cfe1f-189">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-189">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cfe1f-190">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cfe1f-190">passwordRequired</span></span>|<span data-ttu-id="cfe1f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfe1f-191">Boolean</span></span>|<span data-ttu-id="cfe1f-192">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-192">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="cfe1f-193">応答</span><span class="sxs-lookup"><span data-stu-id="cfe1f-193">Response</span></span>
<span data-ttu-id="cfe1f-194">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-194">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune_deviceconfig_macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe1f-195">例</span><span class="sxs-lookup"><span data-stu-id="cfe1f-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="cfe1f-196">要求</span><span class="sxs-lookup"><span data-stu-id="cfe1f-196">Request</span></span>
<span data-ttu-id="cfe1f-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="cfe1f-198">応答</span><span class="sxs-lookup"><span data-stu-id="cfe1f-198">Response</span></span>
<span data-ttu-id="cfe1f-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cfe1f-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```



