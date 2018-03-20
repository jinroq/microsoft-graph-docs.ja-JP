# <a name="list-detectedapps"></a><span data-ttu-id="24efa-101">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="24efa-101">List detectedApps</span></span>

> <span data-ttu-id="24efa-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24efa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24efa-103">[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="24efa-103">List properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24efa-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="24efa-104">Prerequisites</span></span>
<span data-ttu-id="24efa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24efa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24efa-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24efa-107">Permission type</span></span>|<span data-ttu-id="24efa-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24efa-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24efa-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24efa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="24efa-110">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="24efa-110">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="24efa-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24efa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24efa-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24efa-112">Not supported.</span></span>|
|<span data-ttu-id="24efa-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24efa-113">Application</span></span>|<span data-ttu-id="24efa-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24efa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24efa-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24efa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="24efa-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24efa-116">Request headers</span></span>
|<span data-ttu-id="24efa-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24efa-117">Header</span></span>|<span data-ttu-id="24efa-118">値</span><span class="sxs-lookup"><span data-stu-id="24efa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24efa-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="24efa-119">Authorization</span></span>|<span data-ttu-id="24efa-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="24efa-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="24efa-121">Accept</span><span class="sxs-lookup"><span data-stu-id="24efa-121">Accept</span></span>|<span data-ttu-id="24efa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="24efa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24efa-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="24efa-123">Request body</span></span>
<span data-ttu-id="24efa-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="24efa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24efa-125">応答</span><span class="sxs-lookup"><span data-stu-id="24efa-125">Response</span></span>
<span data-ttu-id="24efa-126">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="24efa-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_devices_detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24efa-127">例</span><span class="sxs-lookup"><span data-stu-id="24efa-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="24efa-128">要求</span><span class="sxs-lookup"><span data-stu-id="24efa-128">Request</span></span>
<span data-ttu-id="24efa-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24efa-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="24efa-130">応答</span><span class="sxs-lookup"><span data-stu-id="24efa-130">Response</span></span>
<span data-ttu-id="24efa-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24efa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```



