# <a name="list-messages"></a><span data-ttu-id="b4192-101">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b4192-101">List messages</span></span>

<span data-ttu-id="b4192-102">サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。</span><span class="sxs-lookup"><span data-stu-id="b4192-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="b4192-103">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="b4192-103">Currently, this operation returns message bodies in only HTML format.</span></span>

<span data-ttu-id="b4192-104">アプリが別のユーザーのメール フォルダーのメッセージを取得できる 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="b4192-104">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="b4192-105">このアプリにアプリケーションのアクセス許可がある場合、または、</span><span class="sxs-lookup"><span data-stu-id="b4192-105">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b4192-106">このアプリに、1 人のユーザーから適切な[アクセス許可](#permissions)が委任され、別のユーザーは、そのユーザーとメール フォルダーを共有しているか、またはそのユーザーにアクセスを委任しているかする場合。</span><span class="sxs-lookup"><span data-stu-id="b4192-106">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b4192-107">[詳細と例](../../../concepts/outlook-share-messages-folders.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b4192-107">See [details and an example](../../../concepts/outlook-share-messages-folders.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4192-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b4192-108">Permissions</span></span>
<span data-ttu-id="b4192-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4192-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4192-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b4192-111">Permission type</span></span>      | <span data-ttu-id="b4192-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b4192-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4192-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b4192-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b4192-114">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4192-114">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b4192-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b4192-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4192-116">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4192-116">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b4192-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b4192-117">Application</span></span> | <span data-ttu-id="b4192-118">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4192-118">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4192-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b4192-119">HTTP request</span></span>

<span data-ttu-id="b4192-120">ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="b4192-120">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="b4192-121">ユーザーのメールボックス内の特定のフォルダーにあるメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="b4192-121">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4192-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b4192-122">Optional query parameters</span></span>
<span data-ttu-id="b4192-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b4192-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b4192-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b4192-124">Request headers</span></span>
| <span data-ttu-id="b4192-125">名前</span><span class="sxs-lookup"><span data-stu-id="b4192-125">Name</span></span>       | <span data-ttu-id="b4192-126">型</span><span class="sxs-lookup"><span data-stu-id="b4192-126">Type</span></span> | <span data-ttu-id="b4192-127">説明</span><span class="sxs-lookup"><span data-stu-id="b4192-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b4192-128">承認</span><span class="sxs-lookup"><span data-stu-id="b4192-128">Authorization</span></span>  | <span data-ttu-id="b4192-129">文字列</span><span class="sxs-lookup"><span data-stu-id="b4192-129">string</span></span>  | <span data-ttu-id="b4192-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b4192-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4192-132">優先: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="b4192-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="b4192-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b4192-133">string</span></span> | <span data-ttu-id="b4192-134">**body** プロパティと **uniqueBody** プロパティが返されるときの形式です。</span><span class="sxs-lookup"><span data-stu-id="b4192-134">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="b4192-135">値は、"text" または "html" になります。</span><span class="sxs-lookup"><span data-stu-id="b4192-135">Values can be "text" or "html".</span></span> <span data-ttu-id="b4192-136">ヘッダーが指定されていない場合は、**body** プロパティと **uniqueBody** プロパティは HTML 形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="b4192-136">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="b4192-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b4192-137">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b4192-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="b4192-138">Request body</span></span>
<span data-ttu-id="b4192-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b4192-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4192-140">応答</span><span class="sxs-lookup"><span data-stu-id="b4192-140">Response</span></span>

<span data-ttu-id="b4192-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b4192-141">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="b4192-142">この要求の既定のページ サイズは、メッセージ 10 個です。</span><span class="sxs-lookup"><span data-stu-id="b4192-142">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="b4192-143">例</span><span class="sxs-lookup"><span data-stu-id="b4192-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4192-144">要求</span><span class="sxs-lookup"><span data-stu-id="b4192-144">Request</span></span>
<span data-ttu-id="b4192-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b4192-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="b4192-146">応答</span><span class="sxs-lookup"><span data-stu-id="b4192-146">Response</span></span>
<span data-ttu-id="b4192-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b4192-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
