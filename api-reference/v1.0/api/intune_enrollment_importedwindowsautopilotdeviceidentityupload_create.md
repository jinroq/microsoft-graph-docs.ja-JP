# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="18dd3-101">ImportedWindowsAutopilotDeviceIdentityUpload を作成します</span><span class="sxs-lookup"><span data-stu-id="18dd3-101">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="18dd3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="18dd3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18dd3-103">新しい [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="18dd3-103">Create a new [deviceConfigurationAssignment](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18dd3-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="18dd3-104">Prerequisites</span></span>
<span data-ttu-id="18dd3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18dd3-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18dd3-107">Permission type</span></span>|<span data-ttu-id="18dd3-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18dd3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18dd3-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="18dd3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="18dd3-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18dd3-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="18dd3-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18dd3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18dd3-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18dd3-112">Not supported.</span></span>|
|<span data-ttu-id="18dd3-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18dd3-113">Application</span></span>|<span data-ttu-id="18dd3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18dd3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18dd3-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18dd3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="18dd3-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18dd3-116">Request headers</span></span>
|<span data-ttu-id="18dd3-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18dd3-117">Header</span></span>|<span data-ttu-id="18dd3-118">値</span><span class="sxs-lookup"><span data-stu-id="18dd3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18dd3-119">承認</span><span class="sxs-lookup"><span data-stu-id="18dd3-119">Authorization</span></span>|<span data-ttu-id="18dd3-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="18dd3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18dd3-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="18dd3-121">Accept</span></span>|<span data-ttu-id="18dd3-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="18dd3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18dd3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="18dd3-123">Request body</span></span>
<span data-ttu-id="18dd3-124">要求本文で、importedWindowsAutopilotDeviceIdentityUpload オブジェクトに JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="18dd3-124">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="18dd3-125">次の表に、importedWindowsAutopilotDeviceIdentityUploadの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="18dd3-125">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="18dd3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18dd3-126">Property</span></span>|<span data-ttu-id="18dd3-127">型</span><span class="sxs-lookup"><span data-stu-id="18dd3-127">Type</span></span>|<span data-ttu-id="18dd3-128">説明</span><span class="sxs-lookup"><span data-stu-id="18dd3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18dd3-129">ID</span><span class="sxs-lookup"><span data-stu-id="18dd3-129">id</span></span>|<span data-ttu-id="18dd3-130">文字列</span><span class="sxs-lookup"><span data-stu-id="18dd3-130">String</span></span>|<span data-ttu-id="18dd3-131">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="18dd3-131">The GUID for the object</span></span>|
|<span data-ttu-id="18dd3-132">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="18dd3-132">createdDateTimeUtc</span></span>|<span data-ttu-id="18dd3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18dd3-133">DateTimeOffset</span></span>|<span data-ttu-id="18dd3-134">日時を設定すると、エンティティを作成します。</span><span class="sxs-lookup"><span data-stu-id="18dd3-134">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="18dd3-135">状態</span><span class="sxs-lookup"><span data-stu-id="18dd3-135">status</span></span>|[<span data-ttu-id="18dd3-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="18dd3-136">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="18dd3-137">アップロードステータス</span><span class="sxs-lookup"><span data-stu-id="18dd3-137">Upload status.</span></span> <span data-ttu-id="18dd3-138">可能な値は、`noUpload`、`pending`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="18dd3-138">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="18dd3-139">応答</span><span class="sxs-lookup"><span data-stu-id="18dd3-139">Response</span></span>
<span data-ttu-id="18dd3-140">成功した場合、このメソッドは  応答コードと、`201 Created` 応答本文で更新された [ importedWindowsAutopilotDeviceIdentityUpload](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="18dd3-140">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18dd3-141">例</span><span class="sxs-lookup"><span data-stu-id="18dd3-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="18dd3-142">要求</span><span class="sxs-lookup"><span data-stu-id="18dd3-142">Request</span></span>
<span data-ttu-id="18dd3-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18dd3-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="18dd3-144">応答</span><span class="sxs-lookup"><span data-stu-id="18dd3-144">Response</span></span>
<span data-ttu-id="18dd3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18dd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```








