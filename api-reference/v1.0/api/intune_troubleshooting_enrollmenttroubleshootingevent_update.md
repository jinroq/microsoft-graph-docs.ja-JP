# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="27431-101">enrollmentTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="27431-101">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="27431-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="27431-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27431-103">[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="27431-103">Update the properties of a [calendar](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27431-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="27431-104">Prerequisites</span></span>
<span data-ttu-id="27431-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27431-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27431-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27431-107">Permission type</span></span>|<span data-ttu-id="27431-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27431-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27431-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27431-109">Delegated (work or school account)</span></span>|<span data-ttu-id="27431-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27431-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="27431-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27431-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27431-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27431-112">Not supported.</span></span>|
|<span data-ttu-id="27431-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27431-113">Application</span></span>|<span data-ttu-id="27431-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27431-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27431-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27431-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="27431-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27431-116">Request headers</span></span>
|<span data-ttu-id="27431-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27431-117">Header</span></span>|<span data-ttu-id="27431-118">値</span><span class="sxs-lookup"><span data-stu-id="27431-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27431-119">承認</span><span class="sxs-lookup"><span data-stu-id="27431-119">Authorization</span></span>|<span data-ttu-id="27431-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="27431-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="27431-121">承諾</span><span class="sxs-lookup"><span data-stu-id="27431-121">Accept</span></span>|<span data-ttu-id="27431-122">application/json</span><span class="sxs-lookup"><span data-stu-id="27431-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27431-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="27431-123">Request body</span></span>
<span data-ttu-id="27431-124">要求本文で、[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="27431-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="27431-125">次の表に、[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="27431-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="27431-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27431-126">Property</span></span>|<span data-ttu-id="27431-127">型</span><span class="sxs-lookup"><span data-stu-id="27431-127">Type</span></span>|<span data-ttu-id="27431-128">説明</span><span class="sxs-lookup"><span data-stu-id="27431-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27431-129">id</span><span class="sxs-lookup"><span data-stu-id="27431-129">id</span></span>|<span data-ttu-id="27431-130">String</span><span class="sxs-lookup"><span data-stu-id="27431-130">String</span></span>|<span data-ttu-id="27431-131">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="27431-131">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="27431-132">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="27431-132">eventDateTime</span></span>|<span data-ttu-id="27431-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27431-133">DateTimeOffset</span></span>|<span data-ttu-id="27431-134">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="27431-134">Time when the event occurred .</span></span> <span data-ttu-id="27431-135">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27431-135">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="27431-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="27431-136">correlation_id</span></span>|<span data-ttu-id="27431-137">String</span><span class="sxs-lookup"><span data-stu-id="27431-137">String</span></span>|<span data-ttu-id="27431-138">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="27431-138">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="27431-139">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27431-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="27431-140">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="27431-140">managedDeviceIdentifier</span></span>|<span data-ttu-id="27431-141">String</span><span class="sxs-lookup"><span data-stu-id="27431-141">String</span></span>|<span data-ttu-id="27431-142">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="27431-142">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="27431-143">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="27431-143">operatingSystem</span></span>|<span data-ttu-id="27431-144">String</span><span class="sxs-lookup"><span data-stu-id="27431-144">String</span></span>|<span data-ttu-id="27431-145">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="27431-145">Operating system</span></span>|
|<span data-ttu-id="27431-146">osVersion</span><span class="sxs-lookup"><span data-stu-id="27431-146">osVersion</span></span>|<span data-ttu-id="27431-147">String</span><span class="sxs-lookup"><span data-stu-id="27431-147">String</span></span>|<span data-ttu-id="27431-148">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="27431-148">OS Version.</span></span>|
|<span data-ttu-id="27431-149">userId</span><span class="sxs-lookup"><span data-stu-id="27431-149">userId</span></span>|<span data-ttu-id="27431-150">String</span><span class="sxs-lookup"><span data-stu-id="27431-150">String</span></span>|<span data-ttu-id="27431-151">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="27431-151">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="27431-152">deviceId</span><span class="sxs-lookup"><span data-stu-id="27431-152">deviceId</span></span>|<span data-ttu-id="27431-153">String</span><span class="sxs-lookup"><span data-stu-id="27431-153">String</span></span>|<span data-ttu-id="27431-154">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="27431-154">Azure AD device identifier.</span></span>|
|<span data-ttu-id="27431-155">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="27431-155">enrollmentType</span></span>|<span data-ttu-id="27431-156">String</span><span class="sxs-lookup"><span data-stu-id="27431-156">String</span></span>|<span data-ttu-id="27431-157">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="27431-157">Type of the enrollment.</span></span> <span data-ttu-id="27431-158">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="27431-158">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="27431-159">failureCategory</span><span class="sxs-lookup"><span data-stu-id="27431-159">failureCategory</span></span>|<span data-ttu-id="27431-160">String</span><span class="sxs-lookup"><span data-stu-id="27431-160">String</span></span>|<span data-ttu-id="27431-161">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="27431-161">Highlevel failure category.</span></span> <span data-ttu-id="27431-162">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected` です。</span><span class="sxs-lookup"><span data-stu-id="27431-162">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.</span></span>|
|<span data-ttu-id="27431-163">failureReason</span><span class="sxs-lookup"><span data-stu-id="27431-163">failureReason</span></span>|<span data-ttu-id="27431-164">String</span><span class="sxs-lookup"><span data-stu-id="27431-164">String</span></span>|<span data-ttu-id="27431-165">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="27431-165">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="27431-166">応答</span><span class="sxs-lookup"><span data-stu-id="27431-166">Response</span></span>
<span data-ttu-id="27431-167">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="27431-167">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27431-168">例</span><span class="sxs-lookup"><span data-stu-id="27431-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="27431-169">要求</span><span class="sxs-lookup"><span data-stu-id="27431-169">Request</span></span>
<span data-ttu-id="27431-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27431-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="27431-171">応答</span><span class="sxs-lookup"><span data-stu-id="27431-171">Response</span></span>
<span data-ttu-id="27431-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27431-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



