# <a name="wipemanagedappregistrationsbydevicetag-action"></a><span data-ttu-id="bd1cd-101">wipeManagedAppRegistrationsByDeviceTag アクション</span><span class="sxs-lookup"><span data-stu-id="bd1cd-101">wipeManagedAppRegistrationsByDeviceTag action</span></span>

> <span data-ttu-id="bd1cd-102">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd1cd-103">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-103">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd1cd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd1cd-105">指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-105">Issues a wipe operation on an app registration with specified device tag.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd1cd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="bd1cd-106">Prerequisites</span></span>
<span data-ttu-id="bd1cd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd1cd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd1cd-109">Permission type</span></span>|<span data-ttu-id="bd1cd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd1cd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd1cd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd1cd-111">Delegated (work or school account)</span></span>| <span data-ttu-id="bd1cd-112">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="bd1cd-112">_varies by context_</span></span> |
| <span data-ttu-id="bd1cd-113">&nbsp; &nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="bd1cd-113">.mam</span></span> | <span data-ttu-id="bd1cd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd1cd-114">DeviceManagementApps.ReadWrite.All</span></span> |
|<span data-ttu-id="bd1cd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd1cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd1cd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-116">Not supported.</span></span>|
|<span data-ttu-id="bd1cd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd1cd-117">Application</span></span>|<span data-ttu-id="bd1cd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd1cd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd1cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/wipeManagedAppRegistrationsByDeviceTag
```

## <a name="request-headers"></a><span data-ttu-id="bd1cd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd1cd-120">Request headers</span></span>
|<span data-ttu-id="bd1cd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd1cd-121">Header</span></span>|<span data-ttu-id="bd1cd-122">値</span><span class="sxs-lookup"><span data-stu-id="bd1cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd1cd-123">承認</span><span class="sxs-lookup"><span data-stu-id="bd1cd-123">Authorization</span></span>|<span data-ttu-id="bd1cd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd1cd-125">承諾</span><span class="sxs-lookup"><span data-stu-id="bd1cd-125">Accept</span></span>|<span data-ttu-id="bd1cd-126">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="bd1cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd1cd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd1cd-127">Request body</span></span>
<span data-ttu-id="bd1cd-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bd1cd-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bd1cd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd1cd-130">Property</span></span>|<span data-ttu-id="bd1cd-131">型</span><span class="sxs-lookup"><span data-stu-id="bd1cd-131">Type</span></span>|<span data-ttu-id="bd1cd-132">説明</span><span class="sxs-lookup"><span data-stu-id="bd1cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd1cd-133">deviceTag</span><span class="sxs-lookup"><span data-stu-id="bd1cd-133">deviceTag</span></span>|<span data-ttu-id="bd1cd-134">文字列</span><span class="sxs-lookup"><span data-stu-id="bd1cd-134">String</span></span>|<span data-ttu-id="bd1cd-135">デバイス タグ</span><span class="sxs-lookup"><span data-stu-id="bd1cd-135">device tag</span></span>|

## <a name="response"></a><span data-ttu-id="bd1cd-136">応答</span><span class="sxs-lookup"><span data-stu-id="bd1cd-136">Response</span></span>
<span data-ttu-id="bd1cd-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bd1cd-138">例</span><span class="sxs-lookup"><span data-stu-id="bd1cd-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd1cd-139">要求</span><span class="sxs-lookup"><span data-stu-id="bd1cd-139">Request</span></span>
<span data-ttu-id="bd1cd-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-140">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users/{usersId}/wipeManagedAppRegistrationsByDeviceTag

Content-type: application/json
Content-length: 39

{
  "deviceTag": "Device Tag value"
}
```

### <a name="response"></a><span data-ttu-id="bd1cd-141">応答</span><span class="sxs-lookup"><span data-stu-id="bd1cd-141">Response</span></span>
<span data-ttu-id="bd1cd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd1cd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



