# <a name="update-devicecategory"></a><span data-ttu-id="61124-101">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="61124-101">Update deviceCategory</span></span>

> <span data-ttu-id="61124-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="61124-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61124-103">[deviceCategory](../resources/intune_devices_devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="61124-103">Update the properties of a [calendar](../resources/intune_devices_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61124-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="61124-104">Prerequisites</span></span>
<span data-ttu-id="61124-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="61124-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61124-107">Permission type</span></span>|<span data-ttu-id="61124-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="61124-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61124-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61124-109">Delegated (work or school account)</span></span>|<span data-ttu-id="61124-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61124-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="61124-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61124-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61124-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61124-112">Not supported.</span></span>|
|<span data-ttu-id="61124-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61124-113">Application</span></span>|<span data-ttu-id="61124-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61124-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61124-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61124-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="61124-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61124-116">Request headers</span></span>
|<span data-ttu-id="61124-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61124-117">Header</span></span>|<span data-ttu-id="61124-118">値</span><span class="sxs-lookup"><span data-stu-id="61124-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61124-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="61124-119">Authorization</span></span>|<span data-ttu-id="61124-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="61124-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="61124-121">Accept</span><span class="sxs-lookup"><span data-stu-id="61124-121">Accept</span></span>|<span data-ttu-id="61124-122">application/json</span><span class="sxs-lookup"><span data-stu-id="61124-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61124-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="61124-123">Request body</span></span>
<span data-ttu-id="61124-124">要求本文で、[deviceCategory](../resources/intune_devices_devicecategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="61124-124">In the request body, supply a JSON representation of [Message](../resources/intune_devices_devicecategory.md) object.</span></span>

<span data-ttu-id="61124-125">次の表に、[deviceCategory](../resources/intune_devices_devicecategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="61124-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="61124-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61124-126">Property</span></span>|<span data-ttu-id="61124-127">型</span><span class="sxs-lookup"><span data-stu-id="61124-127">Type</span></span>|<span data-ttu-id="61124-128">説明</span><span class="sxs-lookup"><span data-stu-id="61124-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61124-129">id</span><span class="sxs-lookup"><span data-stu-id="61124-129">id</span></span>|<span data-ttu-id="61124-130">String</span><span class="sxs-lookup"><span data-stu-id="61124-130">String</span></span>|<span data-ttu-id="61124-131">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="61124-131">Unique identifier for the device category.</span></span> <span data-ttu-id="61124-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="61124-132">Read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="61124-133">応答</span><span class="sxs-lookup"><span data-stu-id="61124-133">Response</span></span>
<span data-ttu-id="61124-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCategory](../resources/intune_devices_devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="61124-134">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61124-135">例</span><span class="sxs-lookup"><span data-stu-id="61124-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="61124-136">要求</span><span class="sxs-lookup"><span data-stu-id="61124-136">Request</span></span>
<span data-ttu-id="61124-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="61124-137">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="61124-138">応答</span><span class="sxs-lookup"><span data-stu-id="61124-138">Response</span></span>
<span data-ttu-id="61124-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="61124-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8"
}
```



