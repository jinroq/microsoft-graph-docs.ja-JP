# <a name="list-directreports"></a><span data-ttu-id="e82d5-101">directReports を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="e82d5-101">List directReports</span></span>

<span data-ttu-id="e82d5-p101">ユーザーの直属の部下を取得します。このユーザーがマネージャーとして割り当てられているユーザーと連絡先を返します。</span><span class="sxs-lookup"><span data-stu-id="e82d5-p101">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="e82d5-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e82d5-104">Permissions</span></span>
<span data-ttu-id="e82d5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e82d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e82d5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e82d5-107">Permission type</span></span>      | <span data-ttu-id="e82d5-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e82d5-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e82d5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e82d5-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e82d5-110">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e82d5-110">One of the following scopes is required to execute this API: User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e82d5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e82d5-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e82d5-112">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e82d5-112">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="e82d5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e82d5-113">Application</span></span> | <span data-ttu-id="e82d5-114">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e82d5-114">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e82d5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e82d5-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e82d5-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e82d5-116">Optional query parameters</span></span>
<span data-ttu-id="e82d5-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e82d5-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e82d5-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e82d5-118">Request headers</span></span>
| <span data-ttu-id="e82d5-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e82d5-119">Header</span></span>       | <span data-ttu-id="e82d5-120">値</span><span class="sxs-lookup"><span data-stu-id="e82d5-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e82d5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e82d5-121">Authorization</span></span>  | <span data-ttu-id="e82d5-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e82d5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e82d5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e82d5-124">Content-Type</span></span>   | <span data-ttu-id="e82d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e82d5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e82d5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e82d5-126">Request body</span></span>
<span data-ttu-id="e82d5-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e82d5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e82d5-128">応答</span><span class="sxs-lookup"><span data-stu-id="e82d5-128">Response</span></span>

<span data-ttu-id="e82d5-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e82d5-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e82d5-130">例</span><span class="sxs-lookup"><span data-stu-id="e82d5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e82d5-131">要求</span><span class="sxs-lookup"><span data-stu-id="e82d5-131">Request</span></span>
<span data-ttu-id="e82d5-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e82d5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
##### <a name="response"></a><span data-ttu-id="e82d5-133">応答</span><span class="sxs-lookup"><span data-stu-id="e82d5-133">Response</span></span>
<span data-ttu-id="e82d5-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e82d5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->