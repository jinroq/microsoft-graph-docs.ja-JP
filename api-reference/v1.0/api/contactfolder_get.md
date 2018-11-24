# <a name="get-contactfolder"></a><span data-ttu-id="14b8f-101">Get contactFolder</span><span class="sxs-lookup"><span data-stu-id="14b8f-101">Get contactFolder</span></span>

<span data-ttu-id="14b8f-102">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="14b8f-102">Get a contact folder by using the contact folder ID.</span></span>

<span data-ttu-id="14b8f-103">2 つシナリオは、アプリケーションが別のユーザーの連絡先フォルダーを取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="14b8f-103">There are two scenarios where an app can get another user's contact folder:</span></span>

* <span data-ttu-id="14b8f-104">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="14b8f-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="14b8f-105">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーの連絡先フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="14b8f-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="14b8f-106">[詳細と例](../../../concepts/outlook-get-shared-contacts-folders.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14b8f-106">See [details and an example](../../../concepts/outlook-get-shared-contacts-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="14b8f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="14b8f-107">Permissions</span></span>
<span data-ttu-id="14b8f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14b8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="14b8f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14b8f-110">Permission type</span></span>      | <span data-ttu-id="14b8f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="14b8f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14b8f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="14b8f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="14b8f-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14b8f-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="14b8f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14b8f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14b8f-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14b8f-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="14b8f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14b8f-116">Application</span></span> | <span data-ttu-id="14b8f-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="14b8f-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="14b8f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14b8f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="14b8f-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="14b8f-119">Optional query parameters</span></span>
<span data-ttu-id="14b8f-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="14b8f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="14b8f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14b8f-121">Request headers</span></span>
| <span data-ttu-id="14b8f-122">名前</span><span class="sxs-lookup"><span data-stu-id="14b8f-122">Name</span></span>       | <span data-ttu-id="14b8f-123">型</span><span class="sxs-lookup"><span data-stu-id="14b8f-123">Type</span></span> | <span data-ttu-id="14b8f-124">説明</span><span class="sxs-lookup"><span data-stu-id="14b8f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="14b8f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="14b8f-125">Authorization</span></span>  | <span data-ttu-id="14b8f-126">string</span><span class="sxs-lookup"><span data-stu-id="14b8f-126">string</span></span>  | <span data-ttu-id="14b8f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="14b8f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14b8f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="14b8f-129">Request body</span></span>
<span data-ttu-id="14b8f-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="14b8f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14b8f-131">応答</span><span class="sxs-lookup"><span data-stu-id="14b8f-131">Response</span></span>

<span data-ttu-id="14b8f-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [contactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="14b8f-132">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14b8f-133">例</span><span class="sxs-lookup"><span data-stu-id="14b8f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14b8f-134">要求</span><span class="sxs-lookup"><span data-stu-id="14b8f-134">Request</span></span>
<span data-ttu-id="14b8f-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="14b8f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="14b8f-136">応答</span><span class="sxs-lookup"><span data-stu-id="14b8f-136">Response</span></span>
<span data-ttu-id="14b8f-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="14b8f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
