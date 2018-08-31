# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="75f49-101">enrollmentTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="75f49-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="75f49-102">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75f49-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75f49-103">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75f49-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75f49-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="75f49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="75f49-105">[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="75f49-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="75f49-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="75f49-106">Prerequisites</span></span>
<span data-ttu-id="75f49-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75f49-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75f49-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75f49-109">Permission type</span></span>|<span data-ttu-id="75f49-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="75f49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75f49-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75f49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75f49-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f49-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="75f49-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75f49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75f49-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75f49-114">Not supported.</span></span>|
|<span data-ttu-id="75f49-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75f49-115">Application</span></span>|<span data-ttu-id="75f49-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75f49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75f49-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75f49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="75f49-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75f49-118">Request headers</span></span>
|<span data-ttu-id="75f49-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75f49-119">Header</span></span>|<span data-ttu-id="75f49-120">値</span><span class="sxs-lookup"><span data-stu-id="75f49-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75f49-121">承認</span><span class="sxs-lookup"><span data-stu-id="75f49-121">Authorization</span></span>|<span data-ttu-id="75f49-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="75f49-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75f49-123">承諾</span><span class="sxs-lookup"><span data-stu-id="75f49-123">Accept</span></span>|<span data-ttu-id="75f49-124">application/json</span><span class="sxs-lookup"><span data-stu-id="75f49-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75f49-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="75f49-125">Request body</span></span>
<span data-ttu-id="75f49-126">要求本文で、[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="75f49-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="75f49-127">次の表に、[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="75f49-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="75f49-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75f49-128">Property</span></span>|<span data-ttu-id="75f49-129">タイプ</span><span class="sxs-lookup"><span data-stu-id="75f49-129">Type</span></span>|<span data-ttu-id="75f49-130">説明</span><span class="sxs-lookup"><span data-stu-id="75f49-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75f49-131">ID</span><span class="sxs-lookup"><span data-stu-id="75f49-131">id</span></span>|<span data-ttu-id="75f49-132">文字列</span><span class="sxs-lookup"><span data-stu-id="75f49-132">String</span></span>|<span data-ttu-id="75f49-133">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="75f49-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="75f49-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="75f49-134">eventDateTime</span></span>|<span data-ttu-id="75f49-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75f49-135">DateTimeOffset</span></span>|<span data-ttu-id="75f49-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="75f49-136">Time when the event occurred .</span></span> <span data-ttu-id="75f49-137">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75f49-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="75f49-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="75f49-138">correlationId</span></span>|<span data-ttu-id="75f49-139">文字列</span><span class="sxs-lookup"><span data-stu-id="75f49-139">String</span></span>|<span data-ttu-id="75f49-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="75f49-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="75f49-141">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75f49-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="75f49-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="75f49-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="75f49-143">文字列</span><span class="sxs-lookup"><span data-stu-id="75f49-143">String</span></span>|<span data-ttu-id="75f49-144">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="75f49-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="75f49-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="75f49-145">operatingSystem</span></span>|<span data-ttu-id="75f49-146">文字列</span><span class="sxs-lookup"><span data-stu-id="75f49-146">String</span></span>|<span data-ttu-id="75f49-147">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="75f49-147">Operating System.</span></span>|
|<span data-ttu-id="75f49-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="75f49-148">osVersion</span></span>|<span data-ttu-id="75f49-149">文字列</span><span class="sxs-lookup"><span data-stu-id="75f49-149">String</span></span>|<span data-ttu-id="75f49-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="75f49-150">OS Version.</span></span>|
|<span data-ttu-id="75f49-151">userId</span><span class="sxs-lookup"><span data-stu-id="75f49-151">userId</span></span>|<span data-ttu-id="75f49-152">文字列</span><span class="sxs-lookup"><span data-stu-id="75f49-152">String</span></span>|<span data-ttu-id="75f49-153">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="75f49-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="75f49-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="75f49-154">deviceId</span></span>|<span data-ttu-id="75f49-155">文字列</span><span class="sxs-lookup"><span data-stu-id="75f49-155">String</span></span>|<span data-ttu-id="75f49-156">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="75f49-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="75f49-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="75f49-157">enrollmentType</span></span>|[<span data-ttu-id="75f49-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="75f49-158">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="75f49-159">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="75f49-159">Type of the enrollment.</span></span> <span data-ttu-id="75f49-160">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`です。</span><span class="sxs-lookup"><span data-stu-id="75f49-160">The possible values are `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, , or .</span></span>|
|<span data-ttu-id="75f49-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="75f49-161">failureCategory</span></span>|[<span data-ttu-id="75f49-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="75f49-162">deviceEnrollmentFailureReason values</span></span>](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|<span data-ttu-id="75f49-163">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="75f49-163">Highlevel failure category.</span></span> <span data-ttu-id="75f49-164">可能な値は、`unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected` です。</span><span class="sxs-lookup"><span data-stu-id="75f49-164">The possible values are `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, or .</span></span>|
|<span data-ttu-id="75f49-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="75f49-165">failureReason</span></span>|<span data-ttu-id="75f49-166">文字列</span><span class="sxs-lookup"><span data-stu-id="75f49-166">String</span></span>|<span data-ttu-id="75f49-167">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="75f49-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="75f49-168">応答</span><span class="sxs-lookup"><span data-stu-id="75f49-168">Response</span></span>
<span data-ttu-id="75f49-169">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="75f49-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75f49-170">例</span><span class="sxs-lookup"><span data-stu-id="75f49-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="75f49-171">要求</span><span class="sxs-lookup"><span data-stu-id="75f49-171">Request</span></span>
<span data-ttu-id="75f49-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="75f49-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 440

{
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="75f49-173">応答</span><span class="sxs-lookup"><span data-stu-id="75f49-173">Response</span></span>
<span data-ttu-id="75f49-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="75f49-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```



