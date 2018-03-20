# <a name="geteffectivepermissions-function"></a><span data-ttu-id="0a262-101">getEffectivePermissions 関数</span><span class="sxs-lookup"><span data-stu-id="0a262-101">getEffectivePermissions function</span></span>

> <span data-ttu-id="0a262-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a262-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a262-103">現在の認証ユーザーの有効なアクセス許可を取得します</span><span class="sxs-lookup"><span data-stu-id="0a262-103">Retrieves the effective permissions of the currently authenticated user</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a262-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0a262-104">Prerequisites</span></span>
<span data-ttu-id="0a262-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0a262-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a262-107">Permission type</span></span>|<span data-ttu-id="0a262-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a262-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a262-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a262-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0a262-110">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a262-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="0a262-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a262-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a262-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a262-112">Not supported.</span></span>|
|<span data-ttu-id="0a262-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a262-113">Application</span></span>|<span data-ttu-id="0a262-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a262-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a262-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a262-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="0a262-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a262-116">Request headers</span></span>
|<span data-ttu-id="0a262-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a262-117">Header</span></span>|<span data-ttu-id="0a262-118">値</span><span class="sxs-lookup"><span data-stu-id="0a262-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a262-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a262-119">Authorization</span></span>|<span data-ttu-id="0a262-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a262-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0a262-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0a262-121">Accept</span></span>|<span data-ttu-id="0a262-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0a262-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a262-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a262-123">Request body</span></span>
<span data-ttu-id="0a262-124">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a262-124">In the request URL, provide the following required query parameters with values.</span></span>
<span data-ttu-id="0a262-125">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="0a262-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0a262-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a262-126">Property</span></span>|<span data-ttu-id="0a262-127">型</span><span class="sxs-lookup"><span data-stu-id="0a262-127">Type</span></span>|<span data-ttu-id="0a262-128">説明</span><span class="sxs-lookup"><span data-stu-id="0a262-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a262-129">scope</span><span class="sxs-lookup"><span data-stu-id="0a262-129">scope</span></span>|<span data-ttu-id="0a262-130">String</span><span class="sxs-lookup"><span data-stu-id="0a262-130">String</span></span>|<span data-ttu-id="0a262-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0a262-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0a262-132">応答</span><span class="sxs-lookup"><span data-stu-id="0a262-132">Response</span></span>
<span data-ttu-id="0a262-133">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [rolePermission](../resources/intune_rbac_rolepermission.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0a262-133">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/intune_rbac_rolepermission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a262-134">例</span><span class="sxs-lookup"><span data-stu-id="0a262-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a262-135">要求</span><span class="sxs-lookup"><span data-stu-id="0a262-135">Request</span></span>
<span data-ttu-id="0a262-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a262-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="0a262-137">応答</span><span class="sxs-lookup"><span data-stu-id="0a262-137">Response</span></span>
<span data-ttu-id="0a262-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a262-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ]
}
```



