# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="5ec87-101">deviceManagementTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="5ec87-101">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="5ec87-102">**重要:**Microsoft Graph のベータ版 (/beta) の API はプレビュー中で、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ec87-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ec87-103">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ec87-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ec87-104">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ec87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ec87-105">新しい [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ec87-105">Create a new [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ec87-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="5ec87-106">Prerequisites</span></span>
<span data-ttu-id="5ec87-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ec87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5ec87-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ec87-109">Permission type</span></span>|<span data-ttu-id="5ec87-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ec87-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ec87-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ec87-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5ec87-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ec87-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5ec87-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ec87-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ec87-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ec87-114">Not supported.</span></span>|
|<span data-ttu-id="5ec87-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ec87-115">Application</span></span>|<span data-ttu-id="5ec87-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ec87-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ec87-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ec87-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="5ec87-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ec87-118">Request headers</span></span>
|<span data-ttu-id="5ec87-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ec87-119">Header</span></span>|<span data-ttu-id="5ec87-120">値</span><span class="sxs-lookup"><span data-stu-id="5ec87-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ec87-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ec87-121">Authorization</span></span>|<span data-ttu-id="5ec87-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5ec87-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ec87-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5ec87-123">Accept</span></span>|<span data-ttu-id="5ec87-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5ec87-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ec87-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ec87-125">Request body</span></span>
<span data-ttu-id="5ec87-126">要求本文で、deviceManagementTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5ec87-126">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="5ec87-127">次の表に、deviceManagementTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5ec87-127">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="5ec87-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ec87-128">Property</span></span>|<span data-ttu-id="5ec87-129">型</span><span class="sxs-lookup"><span data-stu-id="5ec87-129">Type</span></span>|<span data-ttu-id="5ec87-130">説明</span><span class="sxs-lookup"><span data-stu-id="5ec87-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ec87-131">id</span><span class="sxs-lookup"><span data-stu-id="5ec87-131">id</span></span>|<span data-ttu-id="5ec87-132">String</span><span class="sxs-lookup"><span data-stu-id="5ec87-132">String</span></span>|<span data-ttu-id="5ec87-133">オブジェクトの UUID</span><span class="sxs-lookup"><span data-stu-id="5ec87-133">UUID for the object</span></span>|
|<span data-ttu-id="5ec87-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="5ec87-134">eventDateTime</span></span>|<span data-ttu-id="5ec87-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ec87-135">DateTimeOffset</span></span>|<span data-ttu-id="5ec87-136">イベントが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="5ec87-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="5ec87-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="5ec87-137">correlationId</span></span>|<span data-ttu-id="5ec87-138">String</span><span class="sxs-lookup"><span data-stu-id="5ec87-138">String</span></span>|<span data-ttu-id="5ec87-139">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="5ec87-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="5ec87-140">応答</span><span class="sxs-lookup"><span data-stu-id="5ec87-140">Response</span></span>
<span data-ttu-id="5ec87-141">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5ec87-141">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ec87-142">例</span><span class="sxs-lookup"><span data-stu-id="5ec87-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ec87-143">要求</span><span class="sxs-lookup"><span data-stu-id="5ec87-143">Request</span></span>
<span data-ttu-id="5ec87-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ec87-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="5ec87-145">応答</span><span class="sxs-lookup"><span data-stu-id="5ec87-145">Response</span></span>
<span data-ttu-id="5ec87-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5ec87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```



