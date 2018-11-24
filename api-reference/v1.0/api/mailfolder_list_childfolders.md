# <a name="list-childfolders"></a><span data-ttu-id="b6e8d-101">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b6e8d-101">List childFolders</span></span>

<span data-ttu-id="b6e8d-p101">指定したフォルダーの下のフォルダーのコレクションを取得します。`.../me/MailFolders` ショートカットを使用して、最上位フォルダーのコレクションを取得して、別のフォルダーに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="b6e8d-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="b6e8d-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b6e8d-104">Permissions</span></span>
<span data-ttu-id="b6e8d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6e8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b6e8d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b6e8d-107">Permission type</span></span>      | <span data-ttu-id="b6e8d-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b6e8d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6e8d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b6e8d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b6e8d-110">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6e8d-110">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b6e8d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b6e8d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6e8d-112">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6e8d-112">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b6e8d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b6e8d-113">Application</span></span> | <span data-ttu-id="b6e8d-114">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6e8d-114">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6e8d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b6e8d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6e8d-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b6e8d-116">Optional query parameters</span></span>
<span data-ttu-id="b6e8d-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b6e8d-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b6e8d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b6e8d-118">Request headers</span></span>
| <span data-ttu-id="b6e8d-119">名前</span><span class="sxs-lookup"><span data-stu-id="b6e8d-119">Name</span></span>       | <span data-ttu-id="b6e8d-120">型</span><span class="sxs-lookup"><span data-stu-id="b6e8d-120">Type</span></span> | <span data-ttu-id="b6e8d-121">説明</span><span class="sxs-lookup"><span data-stu-id="b6e8d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b6e8d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6e8d-122">Authorization</span></span>  | <span data-ttu-id="b6e8d-123">string</span><span class="sxs-lookup"><span data-stu-id="b6e8d-123">string</span></span>  | <span data-ttu-id="b6e8d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b6e8d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6e8d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b6e8d-126">Request body</span></span>
<span data-ttu-id="b6e8d-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b6e8d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6e8d-128">応答</span><span class="sxs-lookup"><span data-stu-id="b6e8d-128">Response</span></span>

<span data-ttu-id="b6e8d-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b6e8d-129">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6e8d-130">例</span><span class="sxs-lookup"><span data-stu-id="b6e8d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b6e8d-131">要求</span><span class="sxs-lookup"><span data-stu-id="b6e8d-131">Request</span></span>
<span data-ttu-id="b6e8d-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b6e8d-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="b6e8d-133">応答</span><span class="sxs-lookup"><span data-stu-id="b6e8d-133">Response</span></span>
<span data-ttu-id="b6e8d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b6e8d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
