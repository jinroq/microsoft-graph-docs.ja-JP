# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="0daf1-101">deviceEnrollmentWindowsHelloForBusinessConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="0daf1-101">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="0daf1-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0daf1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0daf1-103">新しい [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0daf1-103">Create a new [plannerBucket](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0daf1-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0daf1-104">Prerequisites</span></span>
<span data-ttu-id="0daf1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0daf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0daf1-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0daf1-107">Permission type</span></span>|<span data-ttu-id="0daf1-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0daf1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0daf1-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0daf1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0daf1-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0daf1-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0daf1-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0daf1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0daf1-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0daf1-112">Not supported.</span></span>|
|<span data-ttu-id="0daf1-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0daf1-113">Application</span></span>|<span data-ttu-id="0daf1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0daf1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0daf1-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0daf1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0daf1-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0daf1-116">Request headers</span></span>
|<span data-ttu-id="0daf1-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0daf1-117">Header</span></span>|<span data-ttu-id="0daf1-118">値</span><span class="sxs-lookup"><span data-stu-id="0daf1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0daf1-119">承認</span><span class="sxs-lookup"><span data-stu-id="0daf1-119">Authorization</span></span>|<span data-ttu-id="0daf1-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="0daf1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0daf1-121">承諾</span><span class="sxs-lookup"><span data-stu-id="0daf1-121">Accept</span></span>|<span data-ttu-id="0daf1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0daf1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0daf1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0daf1-123">Request body</span></span>
<span data-ttu-id="0daf1-124">要求本文で、deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0daf1-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="0daf1-125">次の表に、deviceEnrollmentWindowsHelloForBusinessConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0daf1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0daf1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0daf1-126">Property</span></span>|<span data-ttu-id="0daf1-127">型</span><span class="sxs-lookup"><span data-stu-id="0daf1-127">Type</span></span>|<span data-ttu-id="0daf1-128">説明</span><span class="sxs-lookup"><span data-stu-id="0daf1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0daf1-129">id</span><span class="sxs-lookup"><span data-stu-id="0daf1-129">id</span></span>|<span data-ttu-id="0daf1-130">String</span><span class="sxs-lookup"><span data-stu-id="0daf1-130">String</span></span>|<span data-ttu-id="0daf1-131">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0daf1-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0daf1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0daf1-132">displayName</span></span>|<span data-ttu-id="0daf1-133">String</span><span class="sxs-lookup"><span data-stu-id="0daf1-133">String</span></span>|<span data-ttu-id="0daf1-134">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0daf1-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0daf1-135">description</span><span class="sxs-lookup"><span data-stu-id="0daf1-135">description</span></span>|<span data-ttu-id="0daf1-136">String</span><span class="sxs-lookup"><span data-stu-id="0daf1-136">String</span></span>|<span data-ttu-id="0daf1-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0daf1-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0daf1-138">priority</span><span class="sxs-lookup"><span data-stu-id="0daf1-138">priority</span></span>|<span data-ttu-id="0daf1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0daf1-139">Int32</span></span>|<span data-ttu-id="0daf1-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0daf1-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0daf1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0daf1-141">createdDateTime</span></span>|<span data-ttu-id="0daf1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0daf1-142">DateTimeOffset</span></span>|<span data-ttu-id="0daf1-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0daf1-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0daf1-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0daf1-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0daf1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0daf1-145">DateTimeOffset</span></span>|<span data-ttu-id="0daf1-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0daf1-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0daf1-147">version</span><span class="sxs-lookup"><span data-stu-id="0daf1-147">version</span></span>|<span data-ttu-id="0daf1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0daf1-148">Int32</span></span>|<span data-ttu-id="0daf1-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0daf1-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0daf1-150">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0daf1-150">pinMinimumLength</span></span>|<span data-ttu-id="0daf1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0daf1-151">Int32</span></span>|<span data-ttu-id="0daf1-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0daf1-152">Not yet documented</span></span>|
|<span data-ttu-id="0daf1-153">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="0daf1-153">pinMaximumLength</span></span>|<span data-ttu-id="0daf1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="0daf1-154">Int32</span></span>|<span data-ttu-id="0daf1-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0daf1-155">Not yet documented</span></span>|
|<span data-ttu-id="0daf1-156">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0daf1-156">pinUppercaseCharactersUsage</span></span>|<span data-ttu-id="0daf1-157">String</span><span class="sxs-lookup"><span data-stu-id="0daf1-157">String</span></span>|<span data-ttu-id="0daf1-158">まだ文書化されていません。可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="0daf1-158">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0daf1-159">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0daf1-159">pinLowercaseCharactersUsage</span></span>|<span data-ttu-id="0daf1-160">String</span><span class="sxs-lookup"><span data-stu-id="0daf1-160">String</span></span>|<span data-ttu-id="0daf1-161">まだ文書化されていません。可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="0daf1-161">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0daf1-162">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="0daf1-162">pinSpecialCharactersUsage</span></span>|<span data-ttu-id="0daf1-163">String</span><span class="sxs-lookup"><span data-stu-id="0daf1-163">String</span></span>|<span data-ttu-id="0daf1-164">まだ文書化されていません。可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="0daf1-164">Not yet documented Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="0daf1-165">state</span><span class="sxs-lookup"><span data-stu-id="0daf1-165">state</span></span>|<span data-ttu-id="0daf1-166">String</span><span class="sxs-lookup"><span data-stu-id="0daf1-166">String</span></span>|<span data-ttu-id="0daf1-167">まだ文書化されていません。可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="0daf1-167">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0daf1-168">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="0daf1-168">securityDeviceRequired</span></span>|<span data-ttu-id="0daf1-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="0daf1-169">Boolean</span></span>|<span data-ttu-id="0daf1-170">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0daf1-170">Not yet documented</span></span>|
|<span data-ttu-id="0daf1-171">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="0daf1-171">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="0daf1-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0daf1-172">Boolean</span></span>|<span data-ttu-id="0daf1-173">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0daf1-173">Not yet documented</span></span>|
|<span data-ttu-id="0daf1-174">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="0daf1-174">remotePassportEnabled</span></span>|<span data-ttu-id="0daf1-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="0daf1-175">Boolean</span></span>|<span data-ttu-id="0daf1-176">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0daf1-176">Not yet documented</span></span>|
|<span data-ttu-id="0daf1-177">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="0daf1-177">pinPreviousBlockCount</span></span>|<span data-ttu-id="0daf1-178">Int32</span><span class="sxs-lookup"><span data-stu-id="0daf1-178">Int32</span></span>|<span data-ttu-id="0daf1-179">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0daf1-179">Not yet documented</span></span>|
|<span data-ttu-id="0daf1-180">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="0daf1-180">pinExpirationInDays</span></span>|<span data-ttu-id="0daf1-181">Int32</span><span class="sxs-lookup"><span data-stu-id="0daf1-181">Int32</span></span>|<span data-ttu-id="0daf1-182">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0daf1-182">Not yet documented</span></span>|
|<span data-ttu-id="0daf1-183">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="0daf1-183">enhancedBiometricsState</span></span>|<span data-ttu-id="0daf1-184">String</span><span class="sxs-lookup"><span data-stu-id="0daf1-184">String</span></span>|<span data-ttu-id="0daf1-185">まだ文書化されていません。可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="0daf1-185">Not yet documented Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="0daf1-186">応答</span><span class="sxs-lookup"><span data-stu-id="0daf1-186">Response</span></span>
<span data-ttu-id="0daf1-187">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0daf1-187">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0daf1-188">例</span><span class="sxs-lookup"><span data-stu-id="0daf1-188">Example</span></span>
### <a name="request"></a><span data-ttu-id="0daf1-189">要求</span><span class="sxs-lookup"><span data-stu-id="0daf1-189">Request</span></span>
<span data-ttu-id="0daf1-190">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0daf1-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0daf1-191">応答</span><span class="sxs-lookup"><span data-stu-id="0daf1-191">Response</span></span>
<span data-ttu-id="0daf1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0daf1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



