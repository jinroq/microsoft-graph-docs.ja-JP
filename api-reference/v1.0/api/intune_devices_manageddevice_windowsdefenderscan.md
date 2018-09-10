# <a name="windowsdefenderscan-action"></a><span data-ttu-id="e44dc-101">windowsDefenderScan アクション</span><span class="sxs-lookup"><span data-stu-id="e44dc-101">windowsDefenderScan action</span></span>

> <span data-ttu-id="e44dc-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e44dc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e44dc-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e44dc-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e44dc-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e44dc-104">Prerequisites</span></span>
<span data-ttu-id="e44dc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e44dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e44dc-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e44dc-107">Permission type</span></span>|<span data-ttu-id="e44dc-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e44dc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e44dc-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e44dc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e44dc-110">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="e44dc-110">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="e44dc-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e44dc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e44dc-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e44dc-112">Not supported.</span></span>|
|<span data-ttu-id="e44dc-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e44dc-113">Application</span></span>|<span data-ttu-id="e44dc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e44dc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e44dc-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e44dc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="e44dc-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e44dc-116">Request headers</span></span>
|<span data-ttu-id="e44dc-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e44dc-117">Header</span></span>|<span data-ttu-id="e44dc-118">値</span><span class="sxs-lookup"><span data-stu-id="e44dc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e44dc-119">承認</span><span class="sxs-lookup"><span data-stu-id="e44dc-119">Authorization</span></span>|<span data-ttu-id="e44dc-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e44dc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e44dc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e44dc-121">Accept</span></span>|<span data-ttu-id="e44dc-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="e44dc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e44dc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e44dc-123">Request body</span></span>
<span data-ttu-id="e44dc-124">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e44dc-124">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e44dc-125">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="e44dc-125">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e44dc-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e44dc-126">Property</span></span>|<span data-ttu-id="e44dc-127">型</span><span class="sxs-lookup"><span data-stu-id="e44dc-127">Type</span></span>|<span data-ttu-id="e44dc-128">説明</span><span class="sxs-lookup"><span data-stu-id="e44dc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44dc-129">quickScan</span><span class="sxs-lookup"><span data-stu-id="e44dc-129">quickScan</span></span>|<span data-ttu-id="e44dc-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44dc-130">Boolean</span></span>|<span data-ttu-id="e44dc-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e44dc-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e44dc-132">応答</span><span class="sxs-lookup"><span data-stu-id="e44dc-132">Response</span></span>
<span data-ttu-id="e44dc-133">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e44dc-133">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e44dc-134">例</span><span class="sxs-lookup"><span data-stu-id="e44dc-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="e44dc-135">要求</span><span class="sxs-lookup"><span data-stu-id="e44dc-135">Request</span></span>
<span data-ttu-id="e44dc-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e44dc-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="e44dc-137">応答</span><span class="sxs-lookup"><span data-stu-id="e44dc-137">Response</span></span>
<span data-ttu-id="e44dc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e44dc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








