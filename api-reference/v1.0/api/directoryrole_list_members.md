# <a name="list-members"></a><span data-ttu-id="f2ddb-101">メンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f2ddb-101">List members</span></span>

<span data-ttu-id="f2ddb-p101">ディレクトリ ロールに割り当てられているユーザーの一覧を取得します。ディレクトリに割り当てることができるのはユーザーのみです。</span><span class="sxs-lookup"><span data-stu-id="f2ddb-p101">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2ddb-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f2ddb-104">Prerequisites</span></span>
<span data-ttu-id="f2ddb-105">この API を実行するには、以下のいずれかの**スコープ**が必要です。*Directory.Read.All* または *Directory.ReadWrite.All* または *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="f2ddb-105">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="f2ddb-106">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2ddb-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f2ddb-107">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f2ddb-107">Optional query parameters</span></span>
<span data-ttu-id="f2ddb-108">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f2ddb-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f2ddb-109">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2ddb-109">Request headers</span></span>
| <span data-ttu-id="f2ddb-110">名前</span><span class="sxs-lookup"><span data-stu-id="f2ddb-110">Name</span></span>       | <span data-ttu-id="f2ddb-111">型</span><span class="sxs-lookup"><span data-stu-id="f2ddb-111">Type</span></span> | <span data-ttu-id="f2ddb-112">説明</span><span class="sxs-lookup"><span data-stu-id="f2ddb-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f2ddb-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2ddb-113">Authorization</span></span>  | <span data-ttu-id="f2ddb-114">string</span><span class="sxs-lookup"><span data-stu-id="f2ddb-114">string</span></span>  | <span data-ttu-id="f2ddb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f2ddb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2ddb-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2ddb-117">Request body</span></span>
<span data-ttu-id="f2ddb-118">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f2ddb-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2ddb-119">応答</span><span class="sxs-lookup"><span data-stu-id="f2ddb-119">Response</span></span>

<span data-ttu-id="f2ddb-120">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f2ddb-120">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f2ddb-121">例</span><span class="sxs-lookup"><span data-stu-id="f2ddb-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2ddb-122">要求</span><span class="sxs-lookup"><span data-stu-id="f2ddb-122">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="f2ddb-123">応答</span><span class="sxs-lookup"><span data-stu-id="f2ddb-123">Response</span></span>
<span data-ttu-id="f2ddb-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2ddb-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->