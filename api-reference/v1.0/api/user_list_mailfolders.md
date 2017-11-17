# <a name="list-mailfolders"></a><span data-ttu-id="6e610-101">mailFolders を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="6e610-101">List mailFolders</span></span>

<span data-ttu-id="6e610-102">サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="6e610-102">Get the mail folder collection under the root folder of the signed-in user.</span></span> 
## <a name="permissions"></a><span data-ttu-id="6e610-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6e610-103">Permissions</span></span>
<span data-ttu-id="6e610-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6e610-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6e610-106">Permission type</span></span>      | <span data-ttu-id="6e610-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6e610-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e610-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6e610-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6e610-109">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e610-109">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6e610-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6e610-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e610-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e610-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6e610-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6e610-112">Application</span></span> | <span data-ttu-id="6e610-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e610-113">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e610-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6e610-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e610-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6e610-115">Optional query parameters</span></span>
<span data-ttu-id="6e610-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6e610-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6e610-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e610-117">Request headers</span></span>
| <span data-ttu-id="6e610-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6e610-118">Header</span></span>       | <span data-ttu-id="6e610-119">値</span><span class="sxs-lookup"><span data-stu-id="6e610-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e610-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e610-120">Authorization</span></span>  | <span data-ttu-id="6e610-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6e610-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e610-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e610-123">Content-Type</span></span>   | <span data-ttu-id="6e610-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6e610-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e610-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6e610-125">Request body</span></span>
<span data-ttu-id="6e610-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6e610-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e610-127">応答</span><span class="sxs-lookup"><span data-stu-id="6e610-127">Response</span></span>

<span data-ttu-id="6e610-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6e610-128">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e610-129">例</span><span class="sxs-lookup"><span data-stu-id="6e610-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e610-130">要求</span><span class="sxs-lookup"><span data-stu-id="6e610-130">Request</span></span>
<span data-ttu-id="6e610-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6e610-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="6e610-132">応答</span><span class="sxs-lookup"><span data-stu-id="6e610-132">Response</span></span>
<span data-ttu-id="6e610-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6e610-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
