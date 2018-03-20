# <a name="create-user"></a><span data-ttu-id="aa452-101">user の作成</span><span class="sxs-lookup"><span data-stu-id="aa452-101">Create User</span></span>

> <span data-ttu-id="aa452-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa452-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa452-103">新しい [user](../resources/intune_onboarding_user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="aa452-103">Create a new user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa452-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="aa452-104">Prerequisites</span></span>
<span data-ttu-id="aa452-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa452-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aa452-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aa452-107">Permission type</span></span>|<span data-ttu-id="aa452-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aa452-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa452-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aa452-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aa452-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa452-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aa452-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aa452-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa452-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa452-112">Not supported.</span></span>|
|<span data-ttu-id="aa452-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aa452-113">Application</span></span>|<span data-ttu-id="aa452-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa452-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa452-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aa452-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="aa452-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa452-116">Request headers</span></span>
|<span data-ttu-id="aa452-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa452-117">Header</span></span>|<span data-ttu-id="aa452-118">値</span><span class="sxs-lookup"><span data-stu-id="aa452-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa452-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa452-119">Authorization</span></span>|<span data-ttu-id="aa452-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa452-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aa452-121">Accept</span><span class="sxs-lookup"><span data-stu-id="aa452-121">Accept</span></span>|<span data-ttu-id="aa452-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aa452-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa452-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="aa452-123">Request body</span></span>
<span data-ttu-id="aa452-124">要求本文で、user オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="aa452-124">In the request body, supply a JSON representation of user object.</span></span>

<span data-ttu-id="aa452-125">次の表に、user の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="aa452-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="aa452-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa452-126">Property</span></span>|<span data-ttu-id="aa452-127">型</span><span class="sxs-lookup"><span data-stu-id="aa452-127">Type</span></span>|<span data-ttu-id="aa452-128">説明</span><span class="sxs-lookup"><span data-stu-id="aa452-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa452-129">id</span><span class="sxs-lookup"><span data-stu-id="aa452-129">id</span></span>|<span data-ttu-id="aa452-130">String</span><span class="sxs-lookup"><span data-stu-id="aa452-130">String</span></span>|<span data-ttu-id="aa452-131">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="aa452-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="aa452-132">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="aa452-132">deviceEnrollmentLimit</span></span>|<span data-ttu-id="aa452-133">Int32</span><span class="sxs-lookup"><span data-stu-id="aa452-133">Int32</span></span>|<span data-ttu-id="aa452-134">ユーザーが登録を許可されているデバイスの最大数。</span><span class="sxs-lookup"><span data-stu-id="aa452-134">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="aa452-135">使用できる値は 5 または 1000 です。</span><span class="sxs-lookup"><span data-stu-id="aa452-135">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="aa452-136">応答</span><span class="sxs-lookup"><span data-stu-id="aa452-136">Response</span></span>
<span data-ttu-id="aa452-137">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [user](../resources/intune_onboarding_user.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aa452-137">If successful, this method returns a `201 Created` response code and [user](../resources/intune_onboarding_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa452-138">例</span><span class="sxs-lookup"><span data-stu-id="aa452-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa452-139">要求</span><span class="sxs-lookup"><span data-stu-id="aa452-139">Request</span></span>
<span data-ttu-id="aa452-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aa452-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.user",
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="aa452-141">応答</span><span class="sxs-lookup"><span data-stu-id="aa452-141">Response</span></span>
<span data-ttu-id="aa452-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa452-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```



