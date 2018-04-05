# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="aea32-101">Get deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="aea32-101">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="aea32-102">**重要:**Microsoft Graph のベータ版 (/beta) の API はプレビュー中で、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aea32-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aea32-103">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aea32-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aea32-104">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aea32-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aea32-105">[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aea32-105">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aea32-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="aea32-106">Prerequisites</span></span>
<span data-ttu-id="aea32-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aea32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aea32-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aea32-109">Permission type</span></span>|<span data-ttu-id="aea32-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aea32-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aea32-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aea32-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aea32-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="aea32-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="aea32-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aea32-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aea32-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aea32-114">Not supported.</span></span>|
|<span data-ttu-id="aea32-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aea32-115">Application</span></span>|<span data-ttu-id="aea32-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aea32-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aea32-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aea32-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aea32-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="aea32-118">Optional query parameters</span></span>
<span data-ttu-id="aea32-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="aea32-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="aea32-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aea32-120">Request headers</span></span>
|<span data-ttu-id="aea32-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aea32-121">Header</span></span>|<span data-ttu-id="aea32-122">値</span><span class="sxs-lookup"><span data-stu-id="aea32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aea32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aea32-123">Authorization</span></span>|<span data-ttu-id="aea32-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="aea32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aea32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aea32-125">Accept</span></span>|<span data-ttu-id="aea32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aea32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aea32-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="aea32-127">Request body</span></span>
<span data-ttu-id="aea32-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="aea32-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aea32-129">応答</span><span class="sxs-lookup"><span data-stu-id="aea32-129">Response</span></span>
<span data-ttu-id="aea32-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aea32-130">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aea32-131">例</span><span class="sxs-lookup"><span data-stu-id="aea32-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="aea32-132">要求</span><span class="sxs-lookup"><span data-stu-id="aea32-132">Request</span></span>
<span data-ttu-id="aea32-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aea32-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="aea32-134">応答</span><span class="sxs-lookup"><span data-stu-id="aea32-134">Response</span></span>
<span data-ttu-id="aea32-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aea32-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value"
  }
}
```



