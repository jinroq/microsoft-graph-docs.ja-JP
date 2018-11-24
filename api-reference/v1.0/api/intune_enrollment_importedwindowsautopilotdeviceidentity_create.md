# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="60612-101">Create importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="60612-101">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="60612-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="60612-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60612-103">新規で [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="60612-103">Create a new [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60612-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="60612-104">Prerequisites</span></span>
<span data-ttu-id="60612-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60612-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="60612-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60612-107">Permission type</span></span>|<span data-ttu-id="60612-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="60612-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60612-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="60612-109">Delegated (work or school account)</span></span>|<span data-ttu-id="60612-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60612-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="60612-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60612-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60612-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60612-112">Not supported.</span></span>|
|<span data-ttu-id="60612-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60612-113">Application</span></span>|<span data-ttu-id="60612-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60612-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60612-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60612-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="60612-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60612-116">Request headers</span></span>
|<span data-ttu-id="60612-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60612-117">Header</span></span>|<span data-ttu-id="60612-118">値</span><span class="sxs-lookup"><span data-stu-id="60612-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60612-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="60612-119">Authorization</span></span>|<span data-ttu-id="60612-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="60612-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60612-121">Accept</span><span class="sxs-lookup"><span data-stu-id="60612-121">Accept</span></span>|<span data-ttu-id="60612-122">application/json</span><span class="sxs-lookup"><span data-stu-id="60612-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60612-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="60612-123">Request body</span></span>
<span data-ttu-id="60612-124">要求本文で、importedWindowsAutopilotDeviceIdentity オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="60612-124">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="60612-125">次の表に、importedWindowsAutopilotDeviceIdentity の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="60612-125">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="60612-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60612-126">Property</span></span>|<span data-ttu-id="60612-127">型</span><span class="sxs-lookup"><span data-stu-id="60612-127">Type</span></span>|<span data-ttu-id="60612-128">説明</span><span class="sxs-lookup"><span data-stu-id="60612-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60612-129">id</span><span class="sxs-lookup"><span data-stu-id="60612-129">id</span></span>|<span data-ttu-id="60612-130">String</span><span class="sxs-lookup"><span data-stu-id="60612-130">String</span></span>|<span data-ttu-id="60612-131">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="60612-131">The GUID for the object</span></span>|
|<span data-ttu-id="60612-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="60612-132">orderIdentifier</span></span>|<span data-ttu-id="60612-133">String</span><span class="sxs-lookup"><span data-stu-id="60612-133">String</span></span>|<span data-ttu-id="60612-134">Windows オートパイロット デバイスの受注 ID。</span><span class="sxs-lookup"><span data-stu-id="60612-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="60612-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="60612-135">serialNumber</span></span>|<span data-ttu-id="60612-136">String</span><span class="sxs-lookup"><span data-stu-id="60612-136">String</span></span>|<span data-ttu-id="60612-137">Windows オートパイロット デバイスのシリアル番号。</span><span class="sxs-lookup"><span data-stu-id="60612-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="60612-138">productKey</span><span class="sxs-lookup"><span data-stu-id="60612-138">productKey</span></span>|<span data-ttu-id="60612-139">String</span><span class="sxs-lookup"><span data-stu-id="60612-139">String</span></span>|<span data-ttu-id="60612-140">Windows オートパイロット デバイスのプロダクト キー。</span><span class="sxs-lookup"><span data-stu-id="60612-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="60612-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="60612-141">hardwareIdentifier</span></span>|<span data-ttu-id="60612-142">バイナリ</span><span class="sxs-lookup"><span data-stu-id="60612-142">Binary</span></span>|<span data-ttu-id="60612-143">Windows オートパイロット デバイスのハードウェア BLOB。</span><span class="sxs-lookup"><span data-stu-id="60612-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="60612-144">state</span><span class="sxs-lookup"><span data-stu-id="60612-144">state</span></span>|[<span data-ttu-id="60612-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="60612-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="60612-146">インポートしたデバイスの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="60612-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="60612-147">応答</span><span class="sxs-lookup"><span data-stu-id="60612-147">Response</span></span>
<span data-ttu-id="60612-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="60612-148">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60612-149">例</span><span class="sxs-lookup"><span data-stu-id="60612-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="60612-150">要求</span><span class="sxs-lookup"><span data-stu-id="60612-150">Request</span></span>
<span data-ttu-id="60612-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60612-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a><span data-ttu-id="60612-152">応答</span><span class="sxs-lookup"><span data-stu-id="60612-152">Response</span></span>
<span data-ttu-id="60612-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60612-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```



