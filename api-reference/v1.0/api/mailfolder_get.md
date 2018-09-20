# <a name="get-mailfolder"></a><span data-ttu-id="0dfc7-101">mailFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="0dfc7-101">Get mailFolder</span></span>

<span data-ttu-id="0dfc7-102">メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-102">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="0dfc7-103">アプリが別のユーザーのメール フォルダーを取得できる 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-103">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="0dfc7-104">このアプリにアプリケーションのアクセス許可がある場合、または、</span><span class="sxs-lookup"><span data-stu-id="0dfc7-104">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0dfc7-105">このアプリに、1 人のユーザーから適切な[アクセス許可](#permissions)が委任され、別のユーザーは、そのユーザーとメールフォルダーを共有しているか、またはそのユーザーにアクセスを委任しているかする場合。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-105">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0dfc7-106">[詳細と例](../../../concepts/outlook-share-messages-folders.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-106">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="0dfc7-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0dfc7-107">Permissions</span></span>
<span data-ttu-id="0dfc7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0dfc7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0dfc7-110">Permission type</span></span>      | <span data-ttu-id="0dfc7-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0dfc7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0dfc7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0dfc7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0dfc7-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0dfc7-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0dfc7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0dfc7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0dfc7-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0dfc7-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0dfc7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0dfc7-116">Application</span></span> | <span data-ttu-id="0dfc7-117">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0dfc7-117">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0dfc7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0dfc7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0dfc7-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0dfc7-119">Optional query parameters</span></span>
<span data-ttu-id="0dfc7-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0dfc7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0dfc7-121">Request headers</span></span>
| <span data-ttu-id="0dfc7-122">名前</span><span class="sxs-lookup"><span data-stu-id="0dfc7-122">Name</span></span>       | <span data-ttu-id="0dfc7-123">型</span><span class="sxs-lookup"><span data-stu-id="0dfc7-123">Type</span></span> | <span data-ttu-id="0dfc7-124">説明</span><span class="sxs-lookup"><span data-stu-id="0dfc7-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0dfc7-125">承認</span><span class="sxs-lookup"><span data-stu-id="0dfc7-125">Authorization</span></span>  | <span data-ttu-id="0dfc7-126">文字列</span><span class="sxs-lookup"><span data-stu-id="0dfc7-126">string</span></span>  | <span data-ttu-id="0dfc7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0dfc7-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0dfc7-129">Request body</span></span>
<span data-ttu-id="0dfc7-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dfc7-131">応答</span><span class="sxs-lookup"><span data-stu-id="0dfc7-131">Response</span></span>

<span data-ttu-id="0dfc7-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-132">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0dfc7-133">例</span><span class="sxs-lookup"><span data-stu-id="0dfc7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0dfc7-134">要求</span><span class="sxs-lookup"><span data-stu-id="0dfc7-134">Request</span></span>
<span data-ttu-id="0dfc7-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="0dfc7-136">応答</span><span class="sxs-lookup"><span data-stu-id="0dfc7-136">Response</span></span>
<span data-ttu-id="0dfc7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0dfc7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
