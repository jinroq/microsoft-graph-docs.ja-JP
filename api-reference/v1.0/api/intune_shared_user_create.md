# <a name="create-user"></a><span data-ttu-id="79112-101">user の作成</span><span class="sxs-lookup"><span data-stu-id="79112-101">Create user</span></span>

> <span data-ttu-id="79112-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79112-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79112-103">新しい [user](../resources/intune_shared_user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="79112-103">Create a new [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="79112-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="79112-104">Prerequisites</span></span>
<span data-ttu-id="79112-105">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="79112-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="79112-106">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79112-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="79112-107">必要な特定のアクセス許可は、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="79112-107">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="79112-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79112-108">Permission type</span></span>|<span data-ttu-id="79112-109">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79112-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79112-110">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="79112-110">Delegated (work or school account)</span></span>| <span data-ttu-id="79112-111">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="79112-111">_varies by context_</span></span> |
| <span data-ttu-id="79112-112">&nbsp; &nbsp; デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="79112-112">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="79112-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79112-113">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="79112-114">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="79112-114">.mam</span></span> | <span data-ttu-id="79112-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79112-115">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="79112-116">&nbsp; &nbsp; 採用</span><span class="sxs-lookup"><span data-stu-id="79112-116">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="79112-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79112-117">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="79112-118">&nbsp; &nbsp; トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="79112-118">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="79112-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79112-119">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="79112-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79112-120">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79112-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79112-121">Not supported.</span></span>|
|<span data-ttu-id="79112-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79112-122">Application</span></span>|<span data-ttu-id="79112-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79112-123">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79112-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79112-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="79112-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79112-125">Request headers</span></span>
|<span data-ttu-id="79112-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79112-126">Header</span></span>|<span data-ttu-id="79112-127">値</span><span class="sxs-lookup"><span data-stu-id="79112-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79112-128">承認</span><span class="sxs-lookup"><span data-stu-id="79112-128">Authorization</span></span>|<span data-ttu-id="79112-129">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="79112-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79112-130">承諾</span><span class="sxs-lookup"><span data-stu-id="79112-130">Accept</span></span>|<span data-ttu-id="79112-131">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="79112-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79112-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="79112-132">Request body</span></span>
<span data-ttu-id="79112-133">要求本文で、user オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="79112-133">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="79112-134">次の表に、user の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="79112-134">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="79112-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79112-135">Property</span></span>|<span data-ttu-id="79112-136">タイプ</span><span class="sxs-lookup"><span data-stu-id="79112-136">Type</span></span>|<span data-ttu-id="79112-137">説明</span><span class="sxs-lookup"><span data-stu-id="79112-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79112-138">ID</span><span class="sxs-lookup"><span data-stu-id="79112-138">id</span></span>|<span data-ttu-id="79112-139">文字列</span><span class="sxs-lookup"><span data-stu-id="79112-139">String</span></span>|<span data-ttu-id="79112-140">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="79112-140">Unique identifier of the user.</span></span>|
|<span data-ttu-id="79112-141">**採用**</span><span class="sxs-lookup"><span data-stu-id="79112-141">**On-boarding**</span></span>|
|<span data-ttu-id="79112-142">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="79112-142">deviceEnrollmentLimit</span></span>|<span data-ttu-id="79112-143">Int32</span><span class="sxs-lookup"><span data-stu-id="79112-143">Int32</span></span>|<span data-ttu-id="79112-144">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="79112-144">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="79112-145">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="79112-145">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="79112-146">要求本文のプロパティのサポートは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="79112-146">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="79112-147">応答</span><span class="sxs-lookup"><span data-stu-id="79112-147">Response</span></span>
<span data-ttu-id="79112-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [user](../resources/intune_shared_user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79112-148">If successful, this method returns a `201 Created` response code and a [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79112-149">例</span><span class="sxs-lookup"><span data-stu-id="79112-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="79112-150">要求</span><span class="sxs-lookup"><span data-stu-id="79112-150">Request</span></span>
<span data-ttu-id="79112-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79112-151">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="79112-152">応答</span><span class="sxs-lookup"><span data-stu-id="79112-152">Response</span></span>
<span data-ttu-id="79112-153">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="79112-153">Here is an example of the response.</span></span> <span data-ttu-id="79112-154">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="79112-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="79112-155">実際の呼び出しから返されるプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="79112-155">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



