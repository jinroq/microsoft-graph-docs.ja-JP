# <a name="list-registereddevices"></a><span data-ttu-id="ad178-101">registeredDevices を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="ad178-101">List registeredDevices</span></span>

<span data-ttu-id="ad178-102">ユーザーの登録済みデバイスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ad178-102">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad178-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ad178-103">Permissions</span></span>
<span data-ttu-id="ad178-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad178-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad178-106">Permission type</span></span>      | <span data-ttu-id="ad178-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad178-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad178-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad178-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ad178-109">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad178-109">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad178-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad178-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad178-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad178-111">Not supported.</span></span>    |
|<span data-ttu-id="ad178-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad178-112">Application</span></span> | <span data-ttu-id="ad178-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad178-113">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad178-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad178-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ad178-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ad178-115">Optional query parameters</span></span>
<span data-ttu-id="ad178-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ad178-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ad178-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad178-117">Request headers</span></span>
| <span data-ttu-id="ad178-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad178-118">Header</span></span>       | <span data-ttu-id="ad178-119">値</span><span class="sxs-lookup"><span data-stu-id="ad178-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad178-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad178-120">Authorization</span></span>  | <span data-ttu-id="ad178-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ad178-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ad178-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ad178-123">Accept</span></span>  | <span data-ttu-id="ad178-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ad178-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad178-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad178-125">Request body</span></span>
<span data-ttu-id="ad178-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad178-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad178-127">応答</span><span class="sxs-lookup"><span data-stu-id="ad178-127">Response</span></span>

<span data-ttu-id="ad178-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ad178-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad178-129">例</span><span class="sxs-lookup"><span data-stu-id="ad178-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad178-130">要求</span><span class="sxs-lookup"><span data-stu-id="ad178-130">Request</span></span>
<span data-ttu-id="ad178-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad178-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="ad178-132">応答</span><span class="sxs-lookup"><span data-stu-id="ad178-132">Response</span></span>
<span data-ttu-id="ad178-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad178-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->