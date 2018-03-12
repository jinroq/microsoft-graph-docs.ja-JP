# <a name="get-auditevent"></a><span data-ttu-id="2662f-101">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="2662f-101">Get auditEvent</span></span>

> <span data-ttu-id="2662f-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2662f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2662f-103">[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2662f-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_auditing_auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2662f-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2662f-104">Prerequisites</span></span>
<span data-ttu-id="2662f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2662f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2662f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2662f-107">Permission type</span></span>|<span data-ttu-id="2662f-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2662f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2662f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2662f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2662f-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2662f-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2662f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2662f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2662f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2662f-112">Not supported.</span></span>|
|<span data-ttu-id="2662f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2662f-113">Application</span></span>|<span data-ttu-id="2662f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2662f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2662f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2662f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2662f-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2662f-116">Optional query parameters</span></span>
<span data-ttu-id="2662f-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2662f-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2662f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2662f-118">Request headers</span></span>
|<span data-ttu-id="2662f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2662f-119">Header</span></span>|<span data-ttu-id="2662f-120">値</span><span class="sxs-lookup"><span data-stu-id="2662f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2662f-121">承認</span><span class="sxs-lookup"><span data-stu-id="2662f-121">Authorization</span></span>|<span data-ttu-id="2662f-122">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="2662f-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2662f-123">承諾</span><span class="sxs-lookup"><span data-stu-id="2662f-123">Accept</span></span>|<span data-ttu-id="2662f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2662f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2662f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2662f-125">Request body</span></span>
<span data-ttu-id="2662f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2662f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2662f-127">応答</span><span class="sxs-lookup"><span data-stu-id="2662f-127">Response</span></span>
<span data-ttu-id="2662f-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2662f-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_auditing_auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2662f-129">例</span><span class="sxs-lookup"><span data-stu-id="2662f-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2662f-130">要求</span><span class="sxs-lookup"><span data-stu-id="2662f-130">Request</span></span>
<span data-ttu-id="2662f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2662f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="2662f-132">応答</span><span class="sxs-lookup"><span data-stu-id="2662f-132">Response</span></span>
<span data-ttu-id="2662f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2662f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1598

{
  "value": {
    "@odata.type": "#microsoft.graph.auditEvent",
    "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
    "displayName": "Display Name value",
    "componentName": "Component Name value",
    "actor": {
      "@odata.type": "microsoft.graph.auditActor",
      "type": "Type value",
      "permissions": [
        "Permissions value"
      ],
      "userPermissions": [
        "User Permissions value"
      ],
      "applicationId": "Application Id value",
      "applicationDisplayName": "Application Display Name value",
      "userPrincipalName": "User Principal Name value",
      "servicePrincipalName": "Service Principal Name value",
      "ipAddress": "Ip Address value",
      "userId": "User Id value"
    },
    "activity": "Activity value",
    "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
    "activityType": "Activity Type value",
    "activityOperationType": "Activity Operation Type value",
    "activityResult": "Activity Result value",
    "correlationId": "<Unknown Primitive Type Edm.Guid>",
    "resources": [
      {
        "@odata.type": "microsoft.graph.auditResource",
        "displayName": "Display Name value",
        "modifiedProperties": [
          {
            "@odata.type": "microsoft.graph.auditProperty",
            "displayName": "Display Name value",
            "oldValue": "Old Value value",
            "newValue": "New Value value"
          }
        ],
        "type": "Type value",
        "resourceId": "Resource Id value"
      }
    ],
    "category": "Category value"
  }
}
```



