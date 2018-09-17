# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="ef71b-101">deviceEnrollmentWindowsHelloForBusinessConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="ef71b-101">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="ef71b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef71b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef71b-103">新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ef71b-103">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef71b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ef71b-104">Prerequisites</span></span>
<span data-ttu-id="ef71b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef71b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ef71b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef71b-107">Permission type</span></span>|<span data-ttu-id="ef71b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef71b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef71b-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef71b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ef71b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef71b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ef71b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef71b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef71b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef71b-112">Not supported.</span></span>|
|<span data-ttu-id="ef71b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef71b-113">Application</span></span>|<span data-ttu-id="ef71b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef71b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef71b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef71b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ef71b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef71b-116">Request headers</span></span>
|<span data-ttu-id="ef71b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef71b-117">Header</span></span>|<span data-ttu-id="ef71b-118">値</span><span class="sxs-lookup"><span data-stu-id="ef71b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef71b-119">承認</span><span class="sxs-lookup"><span data-stu-id="ef71b-119">Authorization</span></span>|<span data-ttu-id="ef71b-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ef71b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef71b-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="ef71b-121">Accept</span></span>|<span data-ttu-id="ef71b-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="ef71b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef71b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ef71b-123">Request body</span></span>
<span data-ttu-id="ef71b-124">要求本文で、deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef71b-124">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="ef71b-125">次の表に、deviceEnrollmentWindowsHelloForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ef71b-125">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="ef71b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef71b-126">Property</span></span>|<span data-ttu-id="ef71b-127">型</span><span class="sxs-lookup"><span data-stu-id="ef71b-127">Type</span></span>|<span data-ttu-id="ef71b-128">説明</span><span class="sxs-lookup"><span data-stu-id="ef71b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef71b-129">ID</span><span class="sxs-lookup"><span data-stu-id="ef71b-129">id</span></span>|<span data-ttu-id="ef71b-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ef71b-130">String</span></span>|<span data-ttu-id="ef71b-131">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef71b-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef71b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ef71b-132">displayName</span></span>|<span data-ttu-id="ef71b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="ef71b-133">String</span></span>|<span data-ttu-id="ef71b-134">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef71b-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef71b-135">説明</span><span class="sxs-lookup"><span data-stu-id="ef71b-135">description</span></span>|<span data-ttu-id="ef71b-136">文字列</span><span class="sxs-lookup"><span data-stu-id="ef71b-136">String</span></span>|<span data-ttu-id="ef71b-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef71b-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef71b-138">重要度</span><span class="sxs-lookup"><span data-stu-id="ef71b-138">priority</span></span>|<span data-ttu-id="ef71b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ef71b-139">Int32</span></span>|<span data-ttu-id="ef71b-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef71b-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef71b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef71b-141">createdDateTime</span></span>|<span data-ttu-id="ef71b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef71b-142">DateTimeOffset</span></span>|<span data-ttu-id="ef71b-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef71b-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef71b-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef71b-144">lastModifiedDateTime</span></span>|<span data-ttu-id="ef71b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef71b-145">DateTimeOffset</span></span>|<span data-ttu-id="ef71b-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef71b-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef71b-147">バージョン</span><span class="sxs-lookup"><span data-stu-id="ef71b-147">version</span></span>|<span data-ttu-id="ef71b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ef71b-148">Int32</span></span>|<span data-ttu-id="ef71b-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef71b-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ef71b-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ef71b-150">pinMinimumLength</span></span>|<span data-ttu-id="ef71b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ef71b-151">Int32</span></span>|<span data-ttu-id="ef71b-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef71b-152">Not yet documented</span></span>|
|<span data-ttu-id="ef71b-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="ef71b-153">pinMaximumLength</span></span>|<span data-ttu-id="ef71b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ef71b-154">Int32</span></span>|<span data-ttu-id="ef71b-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef71b-155">Not yet documented</span></span>|
|<span data-ttu-id="ef71b-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ef71b-156">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="ef71b-157">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="ef71b-157">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="ef71b-158">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="ef71b-158">Not yet documented</span></span> <span data-ttu-id="ef71b-159">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="ef71b-159">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ef71b-160">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ef71b-160">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="ef71b-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="ef71b-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="ef71b-162">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="ef71b-162">Not yet documented</span></span> <span data-ttu-id="ef71b-163">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="ef71b-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ef71b-164">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ef71b-164">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="ef71b-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="ef71b-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune_onboarding_windowshelloforbusinesspinusage.md)|<span data-ttu-id="ef71b-166">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="ef71b-166">Not yet documented</span></span> <span data-ttu-id="ef71b-167">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="ef71b-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ef71b-168">都道府県</span><span class="sxs-lookup"><span data-stu-id="ef71b-168">state</span></span>|[<span data-ttu-id="ef71b-169">有効化</span><span class="sxs-lookup"><span data-stu-id="ef71b-169">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="ef71b-170">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="ef71b-170">Not yet documented</span></span> <span data-ttu-id="ef71b-171">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ef71b-171">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ef71b-172">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="ef71b-172">securityDeviceRequired</span></span>|<span data-ttu-id="ef71b-173">ブール値</span><span class="sxs-lookup"><span data-stu-id="ef71b-173">Boolean</span></span>|<span data-ttu-id="ef71b-174">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef71b-174">Not yet documented</span></span>|
|<span data-ttu-id="ef71b-175">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="ef71b-175">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="ef71b-176">ブール値</span><span class="sxs-lookup"><span data-stu-id="ef71b-176">Boolean</span></span>|<span data-ttu-id="ef71b-177">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef71b-177">Not yet documented</span></span>|
|<span data-ttu-id="ef71b-178">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="ef71b-178">remotePassportEnabled</span></span>|<span data-ttu-id="ef71b-179">ブール値</span><span class="sxs-lookup"><span data-stu-id="ef71b-179">Boolean</span></span>|<span data-ttu-id="ef71b-180">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef71b-180">Not yet documented</span></span>|
|<span data-ttu-id="ef71b-181">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="ef71b-181">pinPreviousBlockCount</span></span>|<span data-ttu-id="ef71b-182">Int32</span><span class="sxs-lookup"><span data-stu-id="ef71b-182">Int32</span></span>|<span data-ttu-id="ef71b-183">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef71b-183">Not yet documented</span></span>|
|<span data-ttu-id="ef71b-184">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="ef71b-184">pinExpirationInDays</span></span>|<span data-ttu-id="ef71b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ef71b-185">Int32</span></span>|<span data-ttu-id="ef71b-186">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef71b-186">Not yet documented</span></span>|
|<span data-ttu-id="ef71b-187">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="ef71b-187">enhancedBiometricsState</span></span>|[<span data-ttu-id="ef71b-188">有効化</span><span class="sxs-lookup"><span data-stu-id="ef71b-188">Enablement</span></span>](../resources/intune_onboarding_enablement.md)|<span data-ttu-id="ef71b-189">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="ef71b-189">Not yet documented</span></span> <span data-ttu-id="ef71b-190">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="ef71b-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef71b-191">応答</span><span class="sxs-lookup"><span data-stu-id="ef71b-191">Response</span></span>
<span data-ttu-id="ef71b-192">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ef71b-192">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef71b-193">例</span><span class="sxs-lookup"><span data-stu-id="ef71b-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef71b-194">要求</span><span class="sxs-lookup"><span data-stu-id="ef71b-194">Request</span></span>
<span data-ttu-id="ef71b-195">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ef71b-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 693

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="ef71b-196">応答</span><span class="sxs-lookup"><span data-stu-id="ef71b-196">Response</span></span>
<span data-ttu-id="ef71b-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ef71b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```








