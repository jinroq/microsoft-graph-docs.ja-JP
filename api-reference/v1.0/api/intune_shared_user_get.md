# <a name="get-user"></a><span data-ttu-id="a1a1a-101">ユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="a1a1a-101">Get user</span></span>

> <span data-ttu-id="a1a1a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1a1a-103">[user](../resources/intune_shared_user.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-103">Read properties and relationships of the [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1a1a-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="a1a1a-104">Prerequisites</span></span>
<span data-ttu-id="a1a1a-105">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="a1a1a-106">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="a1a1a-107">特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-107">The specific permission depends on the context.</span></span>

|<span data-ttu-id="a1a1a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1a1a-108">Permission type</span></span>|<span data-ttu-id="a1a1a-109">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1a1a-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1a1a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1a1a-110">Delegated (work or school account)</span></span>| <span data-ttu-id="a1a1a-111">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="a1a1a-111">_varies by context_</span></span>|
| <span data-ttu-id="a1a1a-112">&nbsp; &nbsp; デバイス</span><span class="sxs-lookup"><span data-stu-id="a1a1a-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="a1a1a-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a1a-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="a1a1a-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="a1a1a-114">.mam</span></span> | <span data-ttu-id="a1a1a-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a1a-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="a1a1a-116">&nbsp; &nbsp; 採用</span><span class="sxs-lookup"><span data-stu-id="a1a1a-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="a1a1a-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a1a-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="a1a1a-118">&nbsp; &nbsp; トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="a1a1a-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="a1a1a-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1a1a-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="a1a1a-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1a1a-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1a1a-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-121">Not supported.</span></span>|
|<span data-ttu-id="a1a1a-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1a1a-122">Application</span></span>|<span data-ttu-id="a1a1a-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1a1a-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1a1a-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1a1a-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a1a1a-125">Optional query parameters</span></span>
<span data-ttu-id="a1a1a-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a1a1a-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1a1a-127">Request headers</span></span>
|<span data-ttu-id="a1a1a-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1a1a-128">Header</span></span>|<span data-ttu-id="a1a1a-129">値</span><span class="sxs-lookup"><span data-stu-id="a1a1a-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1a1a-130">承認</span><span class="sxs-lookup"><span data-stu-id="a1a1a-130">Authorization</span></span>|<span data-ttu-id="a1a1a-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1a1a-132">承諾</span><span class="sxs-lookup"><span data-stu-id="a1a1a-132">Accept</span></span>|<span data-ttu-id="a1a1a-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a1a1a-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1a1a-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1a1a-134">Request body</span></span>
<span data-ttu-id="a1a1a-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1a1a-136">応答</span><span class="sxs-lookup"><span data-stu-id="a1a1a-136">Response</span></span>
<span data-ttu-id="a1a1a-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[ユーザー](../resources/intune_shared_user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-137">If successful, this method returns a `200 OK` response code and [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1a1a-138">例</span><span class="sxs-lookup"><span data-stu-id="a1a1a-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1a1a-139">要求</span><span class="sxs-lookup"><span data-stu-id="a1a1a-139">Request</span></span>
<span data-ttu-id="a1a1a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="a1a1a-141">応答</span><span class="sxs-lookup"><span data-stu-id="a1a1a-141">Response</span></span>
<span data-ttu-id="a1a1a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1a1a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```



