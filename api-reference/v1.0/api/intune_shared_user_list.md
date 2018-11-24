# <a name="list-users"></a><span data-ttu-id="bd28b-101">users のリスト</span><span class="sxs-lookup"><span data-stu-id="bd28b-101">List users</span></span>

> <span data-ttu-id="bd28b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd28b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd28b-103">[user](../resources/intune_shared_user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bd28b-103">List properties and relationships of the [user](../resources/intune_shared_user.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd28b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="bd28b-104">Prerequisites</span></span>
<span data-ttu-id="bd28b-105">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="bd28b-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="bd28b-106">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd28b-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="bd28b-107">特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="bd28b-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="bd28b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd28b-108">Permission type</span></span>|<span data-ttu-id="bd28b-109">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd28b-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd28b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd28b-110">Delegated (work or school account)</span></span>| <span data-ttu-id="bd28b-111">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="bd28b-111">_varies by context_</span></span>|
| <span data-ttu-id="bd28b-112">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="bd28b-112">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="bd28b-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd28b-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="bd28b-114">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="bd28b-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="bd28b-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd28b-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="bd28b-116">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="bd28b-116">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="bd28b-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd28b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="bd28b-118">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="bd28b-118">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="bd28b-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd28b-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="bd28b-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd28b-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd28b-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd28b-121">Not supported.</span></span>|
|<span data-ttu-id="bd28b-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd28b-122">Application</span></span>|<span data-ttu-id="bd28b-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd28b-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd28b-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd28b-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users
```

## <a name="request-headers"></a><span data-ttu-id="bd28b-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd28b-125">Request headers</span></span>
|<span data-ttu-id="bd28b-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd28b-126">Header</span></span>|<span data-ttu-id="bd28b-127">値</span><span class="sxs-lookup"><span data-stu-id="bd28b-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd28b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd28b-128">Authorization</span></span>|<span data-ttu-id="bd28b-129">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bd28b-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd28b-130">Accept</span><span class="sxs-lookup"><span data-stu-id="bd28b-130">Accept</span></span>|<span data-ttu-id="bd28b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="bd28b-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd28b-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd28b-132">Request body</span></span>
<span data-ttu-id="bd28b-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bd28b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd28b-134">応答</span><span class="sxs-lookup"><span data-stu-id="bd28b-134">Response</span></span>
<span data-ttu-id="bd28b-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [user](../resources/intune_shared_user.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bd28b-135">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/intune_shared_user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd28b-136">例</span><span class="sxs-lookup"><span data-stu-id="bd28b-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd28b-137">要求</span><span class="sxs-lookup"><span data-stu-id="bd28b-137">Request</span></span>
<span data-ttu-id="bd28b-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bd28b-138">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users
```

### <a name="response"></a><span data-ttu-id="bd28b-139">応答</span><span class="sxs-lookup"><span data-stu-id="bd28b-139">Response</span></span>
<span data-ttu-id="bd28b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd28b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
    }
  ]
}
```



