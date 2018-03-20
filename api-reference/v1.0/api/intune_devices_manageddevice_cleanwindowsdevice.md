# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="3bb11-101">cleanWindowsDevice アクション</span><span class="sxs-lookup"><span data-stu-id="3bb11-101">cleanWindowsDevice action</span></span>

> <span data-ttu-id="3bb11-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bb11-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bb11-103">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="3bb11-103">Clean Windows device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3bb11-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="3bb11-104">Prerequisites</span></span>
<span data-ttu-id="3bb11-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bb11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3bb11-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bb11-107">Permission type</span></span>|<span data-ttu-id="3bb11-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bb11-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bb11-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bb11-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3bb11-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="3bb11-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="3bb11-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bb11-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bb11-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bb11-112">Not supported.</span></span>|
|<span data-ttu-id="3bb11-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bb11-113">Application</span></span>|<span data-ttu-id="3bb11-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bb11-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bb11-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bb11-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="3bb11-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bb11-116">Request headers</span></span>
|<span data-ttu-id="3bb11-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bb11-117">Header</span></span>|<span data-ttu-id="3bb11-118">値</span><span class="sxs-lookup"><span data-stu-id="3bb11-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bb11-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bb11-119">Authorization</span></span>|<span data-ttu-id="3bb11-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3bb11-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3bb11-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3bb11-121">Accept</span></span>|<span data-ttu-id="3bb11-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3bb11-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bb11-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bb11-123">Request body</span></span>
<span data-ttu-id="3bb11-124">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3bb11-124">In the request body, supply a JSON representation of the Contact object.</span></span>

<span data-ttu-id="3bb11-125">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3bb11-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3bb11-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bb11-126">Property</span></span>|<span data-ttu-id="3bb11-127">型</span><span class="sxs-lookup"><span data-stu-id="3bb11-127">Type</span></span>|<span data-ttu-id="3bb11-128">説明</span><span class="sxs-lookup"><span data-stu-id="3bb11-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bb11-129">keepUserData</span><span class="sxs-lookup"><span data-stu-id="3bb11-129">keepUserData</span></span>|<span data-ttu-id="3bb11-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bb11-130">Boolean</span></span>|<span data-ttu-id="3bb11-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3bb11-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3bb11-132">応答</span><span class="sxs-lookup"><span data-stu-id="3bb11-132">Response</span></span>
<span data-ttu-id="3bb11-133">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="3bb11-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3bb11-134">例</span><span class="sxs-lookup"><span data-stu-id="3bb11-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="3bb11-135">要求</span><span class="sxs-lookup"><span data-stu-id="3bb11-135">Request</span></span>
<span data-ttu-id="3bb11-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bb11-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="3bb11-137">応答</span><span class="sxs-lookup"><span data-stu-id="3bb11-137">Response</span></span>
<span data-ttu-id="3bb11-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3bb11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



