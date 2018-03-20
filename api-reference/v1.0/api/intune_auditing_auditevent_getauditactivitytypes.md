# <a name="getauditactivitytypes-function"></a><span data-ttu-id="ad238-101">getAuditActivityTypes 関数</span><span class="sxs-lookup"><span data-stu-id="ad238-101">getAuditActivityTypes function</span></span>

> <span data-ttu-id="ad238-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad238-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad238-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ad238-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad238-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad238-104">Prerequisites</span></span>
<span data-ttu-id="ad238-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad238-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad238-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad238-107">Permission type</span></span>|<span data-ttu-id="ad238-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad238-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad238-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad238-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ad238-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad238-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ad238-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad238-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad238-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad238-112">Not supported.</span></span>|
|<span data-ttu-id="ad238-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad238-113">Application</span></span>|<span data-ttu-id="ad238-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad238-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad238-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad238-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="ad238-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad238-116">Request headers</span></span>
|<span data-ttu-id="ad238-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad238-117">Header</span></span>|<span data-ttu-id="ad238-118">値</span><span class="sxs-lookup"><span data-stu-id="ad238-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad238-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad238-119">Authorization</span></span>|<span data-ttu-id="ad238-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad238-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ad238-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ad238-121">Accept</span></span>|<span data-ttu-id="ad238-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ad238-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad238-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad238-123">Request body</span></span>
<span data-ttu-id="ad238-124">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad238-124">In the request URL, provide the following required query parameters with values.</span></span>
<span data-ttu-id="ad238-125">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ad238-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ad238-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad238-126">Property</span></span>|<span data-ttu-id="ad238-127">型</span><span class="sxs-lookup"><span data-stu-id="ad238-127">Type</span></span>|<span data-ttu-id="ad238-128">説明</span><span class="sxs-lookup"><span data-stu-id="ad238-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad238-129">category</span><span class="sxs-lookup"><span data-stu-id="ad238-129">category</span></span>|<span data-ttu-id="ad238-130">String</span><span class="sxs-lookup"><span data-stu-id="ad238-130">String</span></span>|<span data-ttu-id="ad238-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ad238-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ad238-132">応答</span><span class="sxs-lookup"><span data-stu-id="ad238-132">Response</span></span>
<span data-ttu-id="ad238-133">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ad238-133">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad238-134">例</span><span class="sxs-lookup"><span data-stu-id="ad238-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad238-135">要求</span><span class="sxs-lookup"><span data-stu-id="ad238-135">Request</span></span>
<span data-ttu-id="ad238-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad238-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ad238-137">応答</span><span class="sxs-lookup"><span data-stu-id="ad238-137">Response</span></span>
<span data-ttu-id="ad238-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad238-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```



