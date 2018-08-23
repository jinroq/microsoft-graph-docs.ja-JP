# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="7bcea-101">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="7bcea-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="7bcea-102">**重要 :** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7bcea-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bcea-103">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bcea-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bcea-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7bcea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bcea-105">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="7bcea-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7bcea-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7bcea-106">Prerequisites</span></span>
<span data-ttu-id="7bcea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7bcea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7bcea-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7bcea-109">Permission type</span></span>|<span data-ttu-id="7bcea-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7bcea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bcea-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7bcea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7bcea-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bcea-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7bcea-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7bcea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bcea-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bcea-114">Not supported.</span></span>|
|<span data-ttu-id="7bcea-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7bcea-115">Application</span></span>|<span data-ttu-id="7bcea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bcea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bcea-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7bcea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="7bcea-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bcea-118">Request headers</span></span>
|<span data-ttu-id="7bcea-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bcea-119">Header</span></span>|<span data-ttu-id="7bcea-120">値</span><span class="sxs-lookup"><span data-stu-id="7bcea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bcea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bcea-121">Authorization</span></span>|<span data-ttu-id="7bcea-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7bcea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bcea-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7bcea-123">Accept</span></span>|<span data-ttu-id="7bcea-124">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="7bcea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bcea-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7bcea-125">Request body</span></span>
<span data-ttu-id="7bcea-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7bcea-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7bcea-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="7bcea-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7bcea-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7bcea-128">Property</span></span>|<span data-ttu-id="7bcea-129">型</span><span class="sxs-lookup"><span data-stu-id="7bcea-129">Type</span></span>|<span data-ttu-id="7bcea-130">説明</span><span class="sxs-lookup"><span data-stu-id="7bcea-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bcea-131">deviceTag</span><span class="sxs-lookup"><span data-stu-id="7bcea-131">deviceTag</span></span>|<span data-ttu-id="7bcea-132">文字列</span><span class="sxs-lookup"><span data-stu-id="7bcea-132">String</span></span>|<span data-ttu-id="7bcea-133">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="7bcea-133">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="7bcea-134">応答</span><span class="sxs-lookup"><span data-stu-id="7bcea-134">Response</span></span>
<span data-ttu-id="7bcea-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7bcea-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7bcea-136">例</span><span class="sxs-lookup"><span data-stu-id="7bcea-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bcea-137">要求</span><span class="sxs-lookup"><span data-stu-id="7bcea-137">Request</span></span>
<span data-ttu-id="7bcea-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7bcea-138">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="7bcea-139">応答</span><span class="sxs-lookup"><span data-stu-id="7bcea-139">Response</span></span>
<span data-ttu-id="7bcea-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7bcea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



