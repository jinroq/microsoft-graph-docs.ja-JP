# <a name="list-messages"></a><span data-ttu-id="44bdb-101">メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="44bdb-101">List messages</span></span>

<span data-ttu-id="44bdb-102">サインイン中のユーザーのメールボックス内のメッセージを取得します (削除済みアイテムと低優先メール フォルダーを含む)。</span><span class="sxs-lookup"><span data-stu-id="44bdb-102">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span>

<span data-ttu-id="44bdb-103">現在、この操作によって返されるメッセージの本文は HTML 形式のみです。</span><span class="sxs-lookup"><span data-stu-id="44bdb-103">Currently, this operation returns message bodies in only HTML format.</span></span>


### <a name="get-messages-in-another-users-message-folder"></a><span data-ttu-id="44bdb-104">別のユーザーのメッセージ フォルダーでメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="44bdb-104">Get messages in another user's message folder</span></span>

<span data-ttu-id="44bdb-105">アプリケーションのアクセス許可がある場合、または 1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合、別のユーザーのメッセージ フォルダーからメッセージを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="44bdb-105">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="44bdb-106">このセクションでは、委任されたアクセス許可に関連するシナリオについて説明します。</span><span class="sxs-lookup"><span data-stu-id="44bdb-106">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="44bdb-107">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="44bdb-107">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="44bdb-108">別のユーザー Garth は、John とメッセージ フォルダーを共有しています。</span><span class="sxs-lookup"><span data-stu-id="44bdb-108">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="44bdb-109">その場合、以下に示すサンプル クエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有フォルダーでメッセージを取得できます。</span><span class="sxs-lookup"><span data-stu-id="44bdb-109">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages
```

<span data-ttu-id="44bdb-110">この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対しサポートされているすべての GET メッセージ操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="44bdb-110">This capability applies to all the supported GET events operations for an individual user, as listed in the [HTTP request](#http-request) section below .</span></span> <span data-ttu-id="44bdb-111">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="44bdb-111">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="44bdb-112">Garth が John とメッセージ フォルダーを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="44bdb-112">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="44bdb-113">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身のメッセージ フォルダーでメッセージを取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="44bdb-113">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
```

<span data-ttu-id="44bdb-114">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="44bdb-114">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="44bdb-115">共有の連絡先フォルダー、予定表、メッセージ フォルダー</span><span class="sxs-lookup"><span data-stu-id="44bdb-115">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="44bdb-116">連絡先、イベント、共有フォルダー内のメッセージ</span><span class="sxs-lookup"><span data-stu-id="44bdb-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="44bdb-117">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="44bdb-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="44bdb-118">この機能は、連絡先、イベント、メッセージ、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="44bdb-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="44bdb-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44bdb-119">Permissions</span></span>
<span data-ttu-id="44bdb-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44bdb-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44bdb-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44bdb-122">Permission type</span></span>      | <span data-ttu-id="44bdb-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44bdb-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44bdb-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44bdb-124">Delegated (work or school account)</span></span> | <span data-ttu-id="44bdb-125">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44bdb-125">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="44bdb-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44bdb-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44bdb-127">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44bdb-127">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="44bdb-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44bdb-128">Application</span></span> | <span data-ttu-id="44bdb-129">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44bdb-129">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="44bdb-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44bdb-130">HTTP request</span></span>

<span data-ttu-id="44bdb-131">ユーザーのメールボックス内のすべてのメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="44bdb-131">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="44bdb-132">ユーザーのメールボックス内の特定のフォルダーにあるメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="44bdb-132">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44bdb-133">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="44bdb-133">Optional query parameters</span></span>
<span data-ttu-id="44bdb-134">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="44bdb-134">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="44bdb-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44bdb-135">Request headers</span></span>
| <span data-ttu-id="44bdb-136">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44bdb-136">Header</span></span>       | <span data-ttu-id="44bdb-137">値</span><span class="sxs-lookup"><span data-stu-id="44bdb-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44bdb-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="44bdb-138">Authorization</span></span>  | <span data-ttu-id="44bdb-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44bdb-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44bdb-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="44bdb-141">Request body</span></span>
<span data-ttu-id="44bdb-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44bdb-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44bdb-143">応答</span><span class="sxs-lookup"><span data-stu-id="44bdb-143">Response</span></span>

<span data-ttu-id="44bdb-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Message](../resources/message.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="44bdb-144">If successful, this method returns a `200 OK` response code and collection of [Message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="44bdb-145">この要求の既定のページ サイズは、メッセージ 10 個です。</span><span class="sxs-lookup"><span data-stu-id="44bdb-145">The default page size for this request is 10 messages.</span></span>

## <a name="example"></a><span data-ttu-id="44bdb-146">例</span><span class="sxs-lookup"><span data-stu-id="44bdb-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44bdb-147">要求</span><span class="sxs-lookup"><span data-stu-id="44bdb-147">Request</span></span>
<span data-ttu-id="44bdb-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44bdb-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a><span data-ttu-id="44bdb-149">応答</span><span class="sxs-lookup"><span data-stu-id="44bdb-149">Response</span></span>
<span data-ttu-id="44bdb-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44bdb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
