# <a name="wipe-action"></a><span data-ttu-id="6064e-101">wipe action</span><span class="sxs-lookup"><span data-stu-id="6064e-101">wipe action</span></span>

> <span data-ttu-id="6064e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6064e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6064e-103">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="6064e-103">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6064e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="6064e-104">Prerequisites</span></span>
<span data-ttu-id="6064e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6064e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6064e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6064e-107">Permission type</span></span>|<span data-ttu-id="6064e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6064e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6064e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6064e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6064e-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6064e-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6064e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6064e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6064e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6064e-112">Not supported.</span></span>|
|<span data-ttu-id="6064e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6064e-113">Application</span></span>|<span data-ttu-id="6064e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6064e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6064e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6064e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="6064e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6064e-116">Request headers</span></span>
|<span data-ttu-id="6064e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6064e-117">Header</span></span>|<span data-ttu-id="6064e-118">値</span><span class="sxs-lookup"><span data-stu-id="6064e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6064e-119">承認</span><span class="sxs-lookup"><span data-stu-id="6064e-119">Authorization</span></span>|<span data-ttu-id="6064e-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6064e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6064e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6064e-121">Accept</span></span>|<span data-ttu-id="6064e-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="6064e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6064e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6064e-123">Request body</span></span>
<span data-ttu-id="6064e-124">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6064e-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6064e-125">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="6064e-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6064e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6064e-126">Property</span></span>|<span data-ttu-id="6064e-127">型</span><span class="sxs-lookup"><span data-stu-id="6064e-127">Type</span></span>|<span data-ttu-id="6064e-128">説明</span><span class="sxs-lookup"><span data-stu-id="6064e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6064e-129">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="6064e-129">keepEnrollmentData</span></span>|<span data-ttu-id="6064e-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="6064e-130">Boolean</span></span>|<span data-ttu-id="6064e-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6064e-131">Not yet documented</span></span>|
|<span data-ttu-id="6064e-132">keepUserData</span><span class="sxs-lookup"><span data-stu-id="6064e-132">keepUserData</span></span>|<span data-ttu-id="6064e-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6064e-133">Boolean</span></span>|<span data-ttu-id="6064e-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6064e-134">Not yet documented</span></span>|
|<span data-ttu-id="6064e-135">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="6064e-135">macOsUnlockCode</span></span>|<span data-ttu-id="6064e-136">文字列</span><span class="sxs-lookup"><span data-stu-id="6064e-136">String</span></span>|<span data-ttu-id="6064e-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6064e-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6064e-138">応答</span><span class="sxs-lookup"><span data-stu-id="6064e-138">Response</span></span>
<span data-ttu-id="6064e-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6064e-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6064e-140">例</span><span class="sxs-lookup"><span data-stu-id="6064e-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="6064e-141">要求</span><span class="sxs-lookup"><span data-stu-id="6064e-141">Request</span></span>
<span data-ttu-id="6064e-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6064e-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="6064e-143">応答</span><span class="sxs-lookup"><span data-stu-id="6064e-143">Response</span></span>
<span data-ttu-id="6064e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6064e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








