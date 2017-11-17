# <a name="list-registeredusers"></a><span data-ttu-id="a066d-101">registeredUsers を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a066d-101">List registeredUsers</span></span>

<span data-ttu-id="a066d-102">デバイスの登録ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a066d-102">Retrieve a list of users that are registered users of the device.</span></span>
## <a name="permissions"></a><span data-ttu-id="a066d-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a066d-103">Permissions</span></span>
<span data-ttu-id="a066d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a066d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="a066d-106">Device.ReadWrite.All と User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="a066d-106">Device.ReadWrite.All and User.ReadBasic.All</span></span>
- <span data-ttu-id="a066d-107">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a066d-107">Directory.Read.All</span></span>
- <span data-ttu-id="a066d-108">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a066d-108">Directory.ReadWrite.All</span></span> 
- <span data-ttu-id="a066d-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a066d-109">Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a066d-110">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a066d-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a066d-111">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a066d-111">Optional query parameters</span></span>
<span data-ttu-id="a066d-112">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a066d-112">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a066d-113">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a066d-113">Request headers</span></span>
| <span data-ttu-id="a066d-114">名前</span><span class="sxs-lookup"><span data-stu-id="a066d-114">Name</span></span>       | <span data-ttu-id="a066d-115">型</span><span class="sxs-lookup"><span data-stu-id="a066d-115">Type</span></span> | <span data-ttu-id="a066d-116">説明</span><span class="sxs-lookup"><span data-stu-id="a066d-116">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a066d-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="a066d-117">Authorization</span></span>  | <span data-ttu-id="a066d-118">string</span><span class="sxs-lookup"><span data-stu-id="a066d-118">string</span></span>  | <span data-ttu-id="a066d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a066d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a066d-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="a066d-121">Request body</span></span>
<span data-ttu-id="a066d-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a066d-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a066d-123">応答</span><span class="sxs-lookup"><span data-stu-id="a066d-123">Response</span></span>

<span data-ttu-id="a066d-124">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a066d-124">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a066d-125">例</span><span class="sxs-lookup"><span data-stu-id="a066d-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a066d-126">要求</span><span class="sxs-lookup"><span data-stu-id="a066d-126">Request</span></span>
<span data-ttu-id="a066d-127">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a066d-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="a066d-128">応答</span><span class="sxs-lookup"><span data-stu-id="a066d-128">Response</span></span>
<span data-ttu-id="a066d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a066d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->