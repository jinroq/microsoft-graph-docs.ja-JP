# <a name="recoverpasscode-action"></a><span data-ttu-id="b0a86-101">recoverPasscode アクション</span><span class="sxs-lookup"><span data-stu-id="b0a86-101">recoverPasscode action</span></span>

> <span data-ttu-id="b0a86-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0a86-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0a86-103">パスコードの回復</span><span class="sxs-lookup"><span data-stu-id="b0a86-103">Recover passcode</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0a86-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b0a86-104">Prerequisites</span></span>
<span data-ttu-id="b0a86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b0a86-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0a86-107">Permission type</span></span>|<span data-ttu-id="b0a86-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0a86-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0a86-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0a86-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b0a86-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="b0a86-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="b0a86-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0a86-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0a86-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0a86-112">Not supported.</span></span>|
|<span data-ttu-id="b0a86-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0a86-113">Application</span></span>|<span data-ttu-id="b0a86-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0a86-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0a86-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0a86-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/managedDevices/{managedDeviceId}/recoverPasscode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/recoverPasscode
```

## <a name="request-headers"></a><span data-ttu-id="b0a86-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0a86-116">Request headers</span></span>
|<span data-ttu-id="b0a86-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0a86-117">Header</span></span>|<span data-ttu-id="b0a86-118">値</span><span class="sxs-lookup"><span data-stu-id="b0a86-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0a86-119">承認</span><span class="sxs-lookup"><span data-stu-id="b0a86-119">Authorization</span></span>|<span data-ttu-id="b0a86-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="b0a86-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b0a86-121">承諾</span><span class="sxs-lookup"><span data-stu-id="b0a86-121">Accept</span></span>|<span data-ttu-id="b0a86-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b0a86-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0a86-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0a86-123">Request body</span></span>
<span data-ttu-id="b0a86-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0a86-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0a86-125">応答</span><span class="sxs-lookup"><span data-stu-id="b0a86-125">Response</span></span>
<span data-ttu-id="b0a86-126">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="b0a86-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b0a86-127">例</span><span class="sxs-lookup"><span data-stu-id="b0a86-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0a86-128">要求</span><span class="sxs-lookup"><span data-stu-id="b0a86-128">Request</span></span>
<span data-ttu-id="b0a86-129">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0a86-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/recoverPasscode
```

### <a name="response"></a><span data-ttu-id="b0a86-130">応答</span><span class="sxs-lookup"><span data-stu-id="b0a86-130">Response</span></span>
<span data-ttu-id="b0a86-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0a86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



