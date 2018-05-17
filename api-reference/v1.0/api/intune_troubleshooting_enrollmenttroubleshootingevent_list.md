# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="ad70e-101">enrollmentTroubleshootingEvent のリスト</span><span class="sxs-lookup"><span data-stu-id="ad70e-101">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="ad70e-102">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad70e-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad70e-103">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad70e-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad70e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad70e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad70e-105">[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ad70e-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad70e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad70e-106">Prerequisites</span></span>
<span data-ttu-id="ad70e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad70e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad70e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad70e-109">Permission type</span></span>|<span data-ttu-id="ad70e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad70e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad70e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad70e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad70e-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad70e-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ad70e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad70e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad70e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad70e-114">Not supported.</span></span>|
|<span data-ttu-id="ad70e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad70e-115">Application</span></span>|<span data-ttu-id="ad70e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad70e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad70e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad70e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="ad70e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad70e-118">Request headers</span></span>
|<span data-ttu-id="ad70e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad70e-119">Header</span></span>|<span data-ttu-id="ad70e-120">値</span><span class="sxs-lookup"><span data-stu-id="ad70e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad70e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad70e-121">Authorization</span></span>|<span data-ttu-id="ad70e-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ad70e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad70e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ad70e-123">Accept</span></span>|<span data-ttu-id="ad70e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ad70e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad70e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad70e-125">Request body</span></span>
<span data-ttu-id="ad70e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad70e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad70e-127">応答</span><span class="sxs-lookup"><span data-stu-id="ad70e-127">Response</span></span>
<span data-ttu-id="ad70e-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ad70e-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad70e-129">例</span><span class="sxs-lookup"><span data-stu-id="ad70e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad70e-130">要求</span><span class="sxs-lookup"><span data-stu-id="ad70e-130">Request</span></span>
<span data-ttu-id="ad70e-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad70e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="ad70e-132">応答</span><span class="sxs-lookup"><span data-stu-id="ad70e-132">Response</span></span>
<span data-ttu-id="ad70e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad70e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
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
  ]
}
```



