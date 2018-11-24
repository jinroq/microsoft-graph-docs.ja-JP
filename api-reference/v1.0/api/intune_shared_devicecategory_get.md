# <a name="get-devicecategory"></a><span data-ttu-id="2ba91-101">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="2ba91-101">Get deviceCategory</span></span>



> <span data-ttu-id="2ba91-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ba91-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ba91-103">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ba91-103">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ba91-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ba91-104">Prerequisites</span></span>
<span data-ttu-id="2ba91-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ba91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ba91-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ba91-107">Permission type</span></span>|<span data-ttu-id="2ba91-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ba91-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ba91-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ba91-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2ba91-110">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="2ba91-110">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2ba91-111">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ba91-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="2ba91-112">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="2ba91-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2ba91-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ba91-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2ba91-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ba91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ba91-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ba91-115">Not supported.</span></span>|
|<span data-ttu-id="2ba91-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ba91-116">Application</span></span>|<span data-ttu-id="2ba91-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ba91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ba91-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ba91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ba91-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2ba91-119">Optional query parameters</span></span>
<span data-ttu-id="2ba91-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2ba91-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ba91-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ba91-121">Request headers</span></span>
|<span data-ttu-id="2ba91-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ba91-122">Header</span></span>|<span data-ttu-id="2ba91-123">値</span><span class="sxs-lookup"><span data-stu-id="2ba91-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ba91-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ba91-124">Authorization</span></span>|<span data-ttu-id="2ba91-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2ba91-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ba91-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2ba91-126">Accept</span></span>|<span data-ttu-id="2ba91-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2ba91-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ba91-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ba91-128">Request body</span></span>
<span data-ttu-id="2ba91-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2ba91-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ba91-130">応答</span><span class="sxs-lookup"><span data-stu-id="2ba91-130">Response</span></span>
<span data-ttu-id="2ba91-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ba91-131">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ba91-132">例</span><span class="sxs-lookup"><span data-stu-id="2ba91-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ba91-133">要求</span><span class="sxs-lookup"><span data-stu-id="2ba91-133">Request</span></span>
<span data-ttu-id="2ba91-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ba91-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="2ba91-135">応答</span><span class="sxs-lookup"><span data-stu-id="2ba91-135">Response</span></span>
<span data-ttu-id="2ba91-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2ba91-136">Here is an example of the response.</span></span> <span data-ttu-id="2ba91-137">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2ba91-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2ba91-138">実際の呼び出しから返されるプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="2ba91-138">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```



