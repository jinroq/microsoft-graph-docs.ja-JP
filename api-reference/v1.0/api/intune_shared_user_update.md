# <a name="update-user"></a><span data-ttu-id="633d3-101">user の更新</span><span class="sxs-lookup"><span data-stu-id="633d3-101">Update user</span></span>

> <span data-ttu-id="633d3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="633d3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="633d3-103">[user](../resources/intune_shared_user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="633d3-103">Update the properties of a [user](../resources/intune_shared_user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="633d3-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="633d3-104">Prerequisites</span></span>
<span data-ttu-id="633d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="633d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="633d3-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="633d3-107">Permission type</span></span>|<span data-ttu-id="633d3-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="633d3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="633d3-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="633d3-109">Delegated (work or school account)</span></span>| <span data-ttu-id="633d3-110">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="633d3-110">_varies by context_</span></span>|
| <span data-ttu-id="633d3-111">&nbsp;&nbsp;デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="633d3-111">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="633d3-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="633d3-112">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="633d3-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="633d3-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="633d3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="633d3-114">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="633d3-115">&nbsp;&nbsp;契約時</span><span class="sxs-lookup"><span data-stu-id="633d3-115">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="633d3-116">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="633d3-116">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="633d3-117">&nbsp;&nbsp;のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="633d3-117">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="633d3-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="633d3-118">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="633d3-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="633d3-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="633d3-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="633d3-120">Not supported.</span></span>|
|<span data-ttu-id="633d3-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="633d3-121">Application</span></span>|<span data-ttu-id="633d3-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="633d3-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="633d3-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="633d3-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="633d3-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="633d3-124">Request headers</span></span>
|<span data-ttu-id="633d3-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="633d3-125">Header</span></span>|<span data-ttu-id="633d3-126">値</span><span class="sxs-lookup"><span data-stu-id="633d3-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="633d3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="633d3-127">Authorization</span></span>|<span data-ttu-id="633d3-128">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="633d3-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="633d3-129">Accept</span><span class="sxs-lookup"><span data-stu-id="633d3-129">Accept</span></span>|<span data-ttu-id="633d3-130">application/json</span><span class="sxs-lookup"><span data-stu-id="633d3-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="633d3-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="633d3-131">Request body</span></span>
<span data-ttu-id="633d3-132">要求本文で、[user](../resources/intune_shared_user.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="633d3-132">In the request body, supply a JSON representation for the [user](../resources/intune_shared_user.md) object.</span></span>

<span data-ttu-id="633d3-133">次の表に、[user](../resources/intune_shared_user.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="633d3-133">The following table shows the properties that are required when you create the [user](../resources/intune_shared_user.md).</span></span>

|<span data-ttu-id="633d3-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="633d3-134">Property</span></span>|<span data-ttu-id="633d3-135">型</span><span class="sxs-lookup"><span data-stu-id="633d3-135">Type</span></span>|<span data-ttu-id="633d3-136">説明</span><span class="sxs-lookup"><span data-stu-id="633d3-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="633d3-137">id</span><span class="sxs-lookup"><span data-stu-id="633d3-137">id</span></span>|<span data-ttu-id="633d3-138">String</span><span class="sxs-lookup"><span data-stu-id="633d3-138">String</span></span>|<span data-ttu-id="633d3-139">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="633d3-139">Unique identifier of the user.</span></span>|
|<span data-ttu-id="633d3-140">**契約時**</span><span class="sxs-lookup"><span data-stu-id="633d3-140">**Onboarding**</span></span>|
|<span data-ttu-id="633d3-141">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="633d3-141">deviceEnrollmentLimit</span></span>|<span data-ttu-id="633d3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="633d3-142">Int32</span></span>|<span data-ttu-id="633d3-143">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="633d3-143">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="633d3-144">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="633d3-144">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="633d3-145">応答</span><span class="sxs-lookup"><span data-stu-id="633d3-145">Response</span></span>
<span data-ttu-id="633d3-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [user](../resources/intune_shared_user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="633d3-146">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune_shared_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="633d3-147">例</span><span class="sxs-lookup"><span data-stu-id="633d3-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="633d3-148">要求</span><span class="sxs-lookup"><span data-stu-id="633d3-148">Request</span></span>
<span data-ttu-id="633d3-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="633d3-149">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="633d3-150">応答</span><span class="sxs-lookup"><span data-stu-id="633d3-150">Response</span></span>
<span data-ttu-id="633d3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="633d3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



