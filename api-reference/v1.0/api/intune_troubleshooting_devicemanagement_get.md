# <a name="get-devicemanagement"></a><span data-ttu-id="4ca86-101">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="4ca86-101">Get deviceManagement</span></span>

> <span data-ttu-id="4ca86-102">**重要: **Microsoft Graph のベータ版 (/beta) の API はプレビュー中で、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4ca86-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ca86-103">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ca86-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ca86-104">**注: **Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ca86-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ca86-105">[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4ca86-105">Read properties and relationships of the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ca86-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4ca86-106">Prerequisites</span></span>
<span data-ttu-id="4ca86-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ca86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ca86-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ca86-109">Permission type</span></span>|<span data-ttu-id="4ca86-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ca86-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ca86-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ca86-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ca86-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ca86-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4ca86-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ca86-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ca86-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ca86-114">Not supported.</span></span>|
|<span data-ttu-id="4ca86-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ca86-115">Application</span></span>|<span data-ttu-id="4ca86-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ca86-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ca86-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ca86-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ca86-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4ca86-118">Optional query parameters</span></span>
<span data-ttu-id="4ca86-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4ca86-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4ca86-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ca86-120">Request headers</span></span>
|<span data-ttu-id="4ca86-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ca86-121">Header</span></span>|<span data-ttu-id="4ca86-122">値</span><span class="sxs-lookup"><span data-stu-id="4ca86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ca86-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ca86-123">Authorization</span></span>|<span data-ttu-id="4ca86-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4ca86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ca86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4ca86-125">Accept</span></span>|<span data-ttu-id="4ca86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4ca86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ca86-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ca86-127">Request body</span></span>
<span data-ttu-id="4ca86-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4ca86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ca86-129">応答</span><span class="sxs-lookup"><span data-stu-id="4ca86-129">Response</span></span>
<span data-ttu-id="4ca86-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4ca86-130">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ca86-131">例</span><span class="sxs-lookup"><span data-stu-id="4ca86-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ca86-132">要求</span><span class="sxs-lookup"><span data-stu-id="4ca86-132">Request</span></span>
<span data-ttu-id="4ca86-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4ca86-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="4ca86-134">応答</span><span class="sxs-lookup"><span data-stu-id="4ca86-134">Response</span></span>
<span data-ttu-id="4ca86-p103">以下は、応答の例です。注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4ca86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```



