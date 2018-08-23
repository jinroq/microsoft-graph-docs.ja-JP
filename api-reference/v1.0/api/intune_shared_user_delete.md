# <a name="delete-user"></a><span data-ttu-id="6dede-101">ユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="6dede-101">Delete user</span></span>

> <span data-ttu-id="6dede-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6dede-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6dede-103">[user](../resources/intune_shared_user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="6dede-103">Deletes a [user](../resources/intune_shared_user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6dede-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="6dede-104">Prerequisites</span></span>
<span data-ttu-id="6dede-105">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="6dede-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="6dede-106">アクセス許可の選択方法などの詳細については [Permissions](../../../concepts/permissions_reference.md) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6dede-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="6dede-107">必要な特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="6dede-107">The specific permission required depends on context.</span></span>

|<span data-ttu-id="6dede-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6dede-108">Permission type</span></span>|<span data-ttu-id="6dede-109">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6dede-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dede-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6dede-110">Delegated (work or school account)</span></span>| <span data-ttu-id="6dede-111">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="6dede-111">_varies by context_</span></span>|
| <span data-ttu-id="6dede-112">&nbsp; &nbsp; デバイス</span><span class="sxs-lookup"><span data-stu-id="6dede-112">&nbsp;&nbsp;</span></span> | <span data-ttu-id="6dede-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dede-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6dede-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="6dede-114">.mam</span></span> | <span data-ttu-id="6dede-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dede-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="6dede-116">&nbsp; &nbsp; 新人研修</span><span class="sxs-lookup"><span data-stu-id="6dede-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="6dede-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dede-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6dede-118">&nbsp; &nbsp; トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="6dede-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="6dede-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dede-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="6dede-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6dede-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dede-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dede-121">Not supported.</span></span>|
|<span data-ttu-id="6dede-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6dede-122">Application</span></span>|<span data-ttu-id="6dede-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dede-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dede-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6dede-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="6dede-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dede-125">Request headers</span></span>
|<span data-ttu-id="6dede-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dede-126">Header</span></span>|<span data-ttu-id="6dede-127">値</span><span class="sxs-lookup"><span data-stu-id="6dede-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dede-128">承認</span><span class="sxs-lookup"><span data-stu-id="6dede-128">Authorization</span></span>|<span data-ttu-id="6dede-129">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6dede-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dede-130">受け入れ</span><span class="sxs-lookup"><span data-stu-id="6dede-130">Accept</span></span>|<span data-ttu-id="6dede-131">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="6dede-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dede-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="6dede-132">Request body</span></span>
<span data-ttu-id="6dede-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6dede-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dede-134">応答</span><span class="sxs-lookup"><span data-stu-id="6dede-134">Response</span></span>
<span data-ttu-id="6dede-135">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6dede-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6dede-136">例</span><span class="sxs-lookup"><span data-stu-id="6dede-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dede-137">要求</span><span class="sxs-lookup"><span data-stu-id="6dede-137">Request</span></span>
<span data-ttu-id="6dede-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6dede-138">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="6dede-139">応答</span><span class="sxs-lookup"><span data-stu-id="6dede-139">Response</span></span>
<span data-ttu-id="6dede-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6dede-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



