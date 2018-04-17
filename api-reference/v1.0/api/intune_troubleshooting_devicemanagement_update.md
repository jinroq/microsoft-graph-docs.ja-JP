# <a name="update-devicemanagement"></a><span data-ttu-id="f6118-101">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="f6118-101">Update deviceManagement</span></span>

> <span data-ttu-id="f6118-102">**重要:**Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f6118-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6118-103">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6118-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6118-104">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6118-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6118-105">[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f6118-105">Update the properties of a [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6118-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f6118-106">Prerequisites</span></span>
<span data-ttu-id="f6118-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6118-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f6118-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6118-109">Permission type</span></span>|<span data-ttu-id="f6118-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6118-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6118-111">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6118-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f6118-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6118-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f6118-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6118-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6118-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6118-114">Not supported.</span></span>|
|<span data-ttu-id="f6118-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6118-115">Application</span></span>|<span data-ttu-id="f6118-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6118-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6118-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6118-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="f6118-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6118-118">Request headers</span></span>
|<span data-ttu-id="f6118-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6118-119">Header</span></span>|<span data-ttu-id="f6118-120">値</span><span class="sxs-lookup"><span data-stu-id="f6118-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6118-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6118-121">Authorization</span></span>|<span data-ttu-id="f6118-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f6118-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6118-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f6118-123">Accept</span></span>|<span data-ttu-id="f6118-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f6118-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6118-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6118-125">Request body</span></span>
<span data-ttu-id="f6118-126">要求本文で、[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6118-126">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object.</span></span>

<span data-ttu-id="f6118-127">次の表に、[deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f6118-127">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md).</span></span>

|<span data-ttu-id="f6118-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6118-128">Property</span></span>|<span data-ttu-id="f6118-129">型</span><span class="sxs-lookup"><span data-stu-id="f6118-129">Type</span></span>|<span data-ttu-id="f6118-130">説明</span><span class="sxs-lookup"><span data-stu-id="f6118-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6118-131">id</span><span class="sxs-lookup"><span data-stu-id="f6118-131">id</span></span>|<span data-ttu-id="f6118-132">String</span><span class="sxs-lookup"><span data-stu-id="f6118-132">String</span></span>|<span data-ttu-id="f6118-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f6118-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f6118-134">応答</span><span class="sxs-lookup"><span data-stu-id="f6118-134">Response</span></span>
<span data-ttu-id="f6118-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f6118-135">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune_troubleshooting_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6118-136">例</span><span class="sxs-lookup"><span data-stu-id="f6118-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6118-137">要求</span><span class="sxs-lookup"><span data-stu-id="f6118-137">Request</span></span>
<span data-ttu-id="f6118-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6118-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="f6118-139">応答</span><span class="sxs-lookup"><span data-stu-id="f6118-139">Response</span></span>
<span data-ttu-id="f6118-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6118-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b"
}
```



