# <a name="delete-devicecategory"></a><span data-ttu-id="40a3c-101">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="40a3c-101">Delete deviceCategory</span></span>

> <span data-ttu-id="40a3c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="40a3c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40a3c-103">[deviceCategory](../resources/intune_shared_devicecategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="40a3c-103">Deletes a [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40a3c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="40a3c-104">Prerequisites</span></span>
<span data-ttu-id="40a3c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40a3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="40a3c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="40a3c-107">Permission type</span></span>|<span data-ttu-id="40a3c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="40a3c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40a3c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="40a3c-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="40a3c-110">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="40a3c-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="40a3c-111">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40a3c-111">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40a3c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="40a3c-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40a3c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40a3c-113">Not supported.</span></span>|
|<span data-ttu-id="40a3c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="40a3c-114">Application</span></span>|<span data-ttu-id="40a3c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40a3c-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40a3c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="40a3c-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="40a3c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40a3c-117">Request headers</span></span>
|<span data-ttu-id="40a3c-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40a3c-118">Header</span></span>|<span data-ttu-id="40a3c-119">値</span><span class="sxs-lookup"><span data-stu-id="40a3c-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40a3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="40a3c-120">Authorization</span></span>|<span data-ttu-id="40a3c-121">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="40a3c-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40a3c-122">Accept</span><span class="sxs-lookup"><span data-stu-id="40a3c-122">Accept</span></span>|<span data-ttu-id="40a3c-123">application/json</span><span class="sxs-lookup"><span data-stu-id="40a3c-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40a3c-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="40a3c-124">Request body</span></span>
<span data-ttu-id="40a3c-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="40a3c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40a3c-126">応答</span><span class="sxs-lookup"><span data-stu-id="40a3c-126">Response</span></span>
<span data-ttu-id="40a3c-127">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="40a3c-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="40a3c-128">例</span><span class="sxs-lookup"><span data-stu-id="40a3c-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="40a3c-129">要求</span><span class="sxs-lookup"><span data-stu-id="40a3c-129">Request</span></span>
<span data-ttu-id="40a3c-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="40a3c-130">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="40a3c-131">応答</span><span class="sxs-lookup"><span data-stu-id="40a3c-131">Response</span></span>
<span data-ttu-id="40a3c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="40a3c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



