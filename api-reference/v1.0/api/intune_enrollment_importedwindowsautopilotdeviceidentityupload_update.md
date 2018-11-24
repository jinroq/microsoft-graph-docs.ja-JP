# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="a5b18-101">ImportedWindowsAutopilotDeviceIdentityUpload を更新します。</span><span class="sxs-lookup"><span data-stu-id="a5b18-101">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="a5b18-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5b18-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5b18-103">[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5b18-103">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5b18-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="a5b18-104">Prerequisites</span></span>
<span data-ttu-id="a5b18-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5b18-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5b18-107">Permission type</span></span>|<span data-ttu-id="a5b18-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5b18-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5b18-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5b18-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a5b18-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5b18-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a5b18-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5b18-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5b18-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5b18-112">Not supported.</span></span>|
|<span data-ttu-id="a5b18-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5b18-113">Application</span></span>|<span data-ttu-id="a5b18-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5b18-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5b18-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5b18-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="a5b18-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5b18-116">Request headers</span></span>
|<span data-ttu-id="a5b18-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5b18-117">Header</span></span>|<span data-ttu-id="a5b18-118">値</span><span class="sxs-lookup"><span data-stu-id="a5b18-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5b18-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5b18-119">Authorization</span></span>|<span data-ttu-id="a5b18-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a5b18-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5b18-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a5b18-121">Accept</span></span>|<span data-ttu-id="a5b18-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a5b18-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5b18-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5b18-123">Request body</span></span>
<span data-ttu-id="a5b18-124">要求の本文に[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5b18-124">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="a5b18-125">[ImportedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="a5b18-125">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="a5b18-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5b18-126">Property</span></span>|<span data-ttu-id="a5b18-127">型</span><span class="sxs-lookup"><span data-stu-id="a5b18-127">Type</span></span>|<span data-ttu-id="a5b18-128">説明</span><span class="sxs-lookup"><span data-stu-id="a5b18-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5b18-129">id</span><span class="sxs-lookup"><span data-stu-id="a5b18-129">id</span></span>|<span data-ttu-id="a5b18-130">String</span><span class="sxs-lookup"><span data-stu-id="a5b18-130">String</span></span>|<span data-ttu-id="a5b18-131">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="a5b18-131">The GUID for the object</span></span>|
|<span data-ttu-id="a5b18-132">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="a5b18-132">createdDateTimeUtc</span></span>|<span data-ttu-id="a5b18-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5b18-133">DateTimeOffset</span></span>|<span data-ttu-id="a5b18-134">日時を設定すると、エンティティを作成します。</span><span class="sxs-lookup"><span data-stu-id="a5b18-134">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="a5b18-135">status</span><span class="sxs-lookup"><span data-stu-id="a5b18-135">status</span></span>|[<span data-ttu-id="a5b18-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="a5b18-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="a5b18-137">ステータスをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="a5b18-137">Upload status.</span></span> <span data-ttu-id="a5b18-138">可能な値は、`noUpload`、`pending`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="a5b18-138">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="a5b18-139">応答</span><span class="sxs-lookup"><span data-stu-id="a5b18-139">Response</span></span>
<span data-ttu-id="a5b18-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a5b18-140">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5b18-141">例</span><span class="sxs-lookup"><span data-stu-id="a5b18-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5b18-142">要求</span><span class="sxs-lookup"><span data-stu-id="a5b18-142">Request</span></span>
<span data-ttu-id="a5b18-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5b18-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="a5b18-144">応答</span><span class="sxs-lookup"><span data-stu-id="a5b18-144">Response</span></span>
<span data-ttu-id="a5b18-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5b18-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```



