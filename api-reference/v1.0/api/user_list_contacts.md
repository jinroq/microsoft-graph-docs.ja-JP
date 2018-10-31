# <a name="list-contacts"></a><span data-ttu-id="9007a-101">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="9007a-101">List contacts</span></span>

<span data-ttu-id="9007a-102">サインイン中のユーザーの既定の連絡先フォルダーから連絡先コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="9007a-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>

<span data-ttu-id="9007a-103">アプリが別のユーザーの連絡先フォルダーの連絡先を取得できる 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="9007a-103">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="9007a-104">このアプリにアプリケーションのアクセス許可がある場合、または、</span><span class="sxs-lookup"><span data-stu-id="9007a-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="9007a-105">このアプリに、1 人のユーザーから適切な[アクセス許可](#permissions)が委任され、別のユーザーは、そのユーザーと連絡先フォルダーを共有しているか、またはそのユーザーにアクセスを委任しているかする場合。</span><span class="sxs-lookup"><span data-stu-id="9007a-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="9007a-106">[詳細と例](../../../concepts/outlook-get-shared-contacts-folders.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9007a-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="9007a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9007a-107">Permissions</span></span>
<span data-ttu-id="9007a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9007a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9007a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9007a-110">Permission type</span></span>      | <span data-ttu-id="9007a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9007a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9007a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9007a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9007a-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9007a-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9007a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9007a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9007a-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9007a-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9007a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9007a-116">Application</span></span> | <span data-ttu-id="9007a-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9007a-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9007a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9007a-118">HTTP request</span></span>

<span data-ttu-id="9007a-119">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="9007a-119">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="9007a-120">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="9007a-120">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9007a-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9007a-121">Optional query parameters</span></span>
<span data-ttu-id="9007a-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9007a-122">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="9007a-123">たとえば、`$filter` クエリ パラメーターを使って、メール アドレスのドメインに基づいて連絡先をフィルターすることができます。</span><span class="sxs-lookup"><span data-stu-id="9007a-123">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="9007a-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9007a-124">Request headers</span></span>
| <span data-ttu-id="9007a-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9007a-125">Header</span></span>       | <span data-ttu-id="9007a-126">値</span><span class="sxs-lookup"><span data-stu-id="9007a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9007a-127">承認</span><span class="sxs-lookup"><span data-stu-id="9007a-127">Authorization</span></span>  | <span data-ttu-id="9007a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9007a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9007a-130">コンテンツ-種類</span><span class="sxs-lookup"><span data-stu-id="9007a-130">Content-Type</span></span>   | <span data-ttu-id="9007a-131">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="9007a-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9007a-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="9007a-132">Request body</span></span>
<span data-ttu-id="9007a-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9007a-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9007a-134">応答</span><span class="sxs-lookup"><span data-stu-id="9007a-134">Response</span></span>

<span data-ttu-id="9007a-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9007a-135">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9007a-136">例</span><span class="sxs-lookup"><span data-stu-id="9007a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9007a-137">要求</span><span class="sxs-lookup"><span data-stu-id="9007a-137">Request</span></span>
<span data-ttu-id="9007a-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9007a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="9007a-139">応答</span><span class="sxs-lookup"><span data-stu-id="9007a-139">Response</span></span>
<span data-ttu-id="9007a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9007a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
