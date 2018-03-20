# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="cf33e-101">deviceEnrollmentPlatformRestrictionsConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="cf33e-101">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="cf33e-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf33e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf33e-103">新しい [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cf33e-103">Create a new [plannerBucket](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf33e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="cf33e-104">Prerequisites</span></span>
<span data-ttu-id="cf33e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf33e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf33e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf33e-107">Permission type</span></span>|<span data-ttu-id="cf33e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf33e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf33e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf33e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cf33e-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf33e-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cf33e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf33e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf33e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf33e-112">Not supported.</span></span>|
|<span data-ttu-id="cf33e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf33e-113">Application</span></span>|<span data-ttu-id="cf33e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf33e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf33e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf33e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cf33e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf33e-116">Request headers</span></span>
|<span data-ttu-id="cf33e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf33e-117">Header</span></span>|<span data-ttu-id="cf33e-118">値</span><span class="sxs-lookup"><span data-stu-id="cf33e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf33e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf33e-119">Authorization</span></span>|<span data-ttu-id="cf33e-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf33e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cf33e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="cf33e-121">Accept</span></span>|<span data-ttu-id="cf33e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cf33e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf33e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf33e-123">Request body</span></span>
<span data-ttu-id="cf33e-124">要求本文で、deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf33e-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="cf33e-125">次の表に、deviceEnrollmentPlatformRestrictionsConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cf33e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="cf33e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf33e-126">Property</span></span>|<span data-ttu-id="cf33e-127">型</span><span class="sxs-lookup"><span data-stu-id="cf33e-127">Type</span></span>|<span data-ttu-id="cf33e-128">説明</span><span class="sxs-lookup"><span data-stu-id="cf33e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf33e-129">id</span><span class="sxs-lookup"><span data-stu-id="cf33e-129">id</span></span>|<span data-ttu-id="cf33e-130">String</span><span class="sxs-lookup"><span data-stu-id="cf33e-130">String</span></span>|<span data-ttu-id="cf33e-131">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf33e-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf33e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="cf33e-132">displayName</span></span>|<span data-ttu-id="cf33e-133">String</span><span class="sxs-lookup"><span data-stu-id="cf33e-133">String</span></span>|<span data-ttu-id="cf33e-134">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf33e-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf33e-135">description</span><span class="sxs-lookup"><span data-stu-id="cf33e-135">description</span></span>|<span data-ttu-id="cf33e-136">String</span><span class="sxs-lookup"><span data-stu-id="cf33e-136">String</span></span>|<span data-ttu-id="cf33e-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf33e-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf33e-138">priority</span><span class="sxs-lookup"><span data-stu-id="cf33e-138">priority</span></span>|<span data-ttu-id="cf33e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cf33e-139">Int32</span></span>|<span data-ttu-id="cf33e-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf33e-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf33e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf33e-141">createdDateTime</span></span>|<span data-ttu-id="cf33e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf33e-142">DateTimeOffset</span></span>|<span data-ttu-id="cf33e-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf33e-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf33e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf33e-144">lastModifiedDateTime</span></span>|<span data-ttu-id="cf33e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf33e-145">DateTimeOffset</span></span>|<span data-ttu-id="cf33e-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf33e-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf33e-147">version</span><span class="sxs-lookup"><span data-stu-id="cf33e-147">version</span></span>|<span data-ttu-id="cf33e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="cf33e-148">Int32</span></span>|<span data-ttu-id="cf33e-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cf33e-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cf33e-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-150">iosRestriction</span></span>|[<span data-ttu-id="cf33e-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf33e-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cf33e-152">Not yet documented</span></span>|
|<span data-ttu-id="cf33e-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-153">windowsRestriction</span></span>|[<span data-ttu-id="cf33e-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf33e-155">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cf33e-155">Not yet documented</span></span>|
|<span data-ttu-id="cf33e-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="cf33e-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf33e-158">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cf33e-158">Not yet documented</span></span>|
|<span data-ttu-id="cf33e-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-159">androidRestriction</span></span>|[<span data-ttu-id="cf33e-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf33e-161">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cf33e-161">Not yet documented</span></span>|
|<span data-ttu-id="cf33e-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-162">macOSRestriction</span></span>|[<span data-ttu-id="cf33e-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="cf33e-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="cf33e-164">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cf33e-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="cf33e-165">応答</span><span class="sxs-lookup"><span data-stu-id="cf33e-165">Response</span></span>
<span data-ttu-id="cf33e-166">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cf33e-166">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf33e-167">例</span><span class="sxs-lookup"><span data-stu-id="cf33e-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf33e-168">要求</span><span class="sxs-lookup"><span data-stu-id="cf33e-168">Request</span></span>
<span data-ttu-id="cf33e-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf33e-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 1714

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="cf33e-170">応答</span><span class="sxs-lookup"><span data-stu-id="cf33e-170">Response</span></span>
<span data-ttu-id="cf33e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf33e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1822

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```



