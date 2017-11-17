# <a name="get-mailfolder"></a><span data-ttu-id="d6347-101">mailFolder を取得する</span><span class="sxs-lookup"><span data-stu-id="d6347-101">Get mailFolder</span></span>

<span data-ttu-id="d6347-102">メッセージ フォルダー オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d6347-102">Retrieve the properties and relationships of a message object.</span></span>


### <a name="get-another-users-message-folder"></a><span data-ttu-id="d6347-103">別のユーザーのメッセージ フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="d6347-103">Get another user's contact folder</span></span>

<span data-ttu-id="d6347-104">アプリケーションのアクセス許可がある場合や、1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合には、別のユーザーのメッセージ フォルダーを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="d6347-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="d6347-105">このセクションでは、委任されたアクセス許可に関連するシナリオについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d6347-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="d6347-106">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="d6347-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="d6347-107">別のユーザー Garth は、John とメッセージ フォルダーを共有しています。</span><span class="sxs-lookup"><span data-stu-id="d6347-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="d6347-108">その場合、以下に示す例のクエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有フォルダーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="d6347-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/mailFolders/{id}
```

<span data-ttu-id="d6347-109">この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対するすべての GET メッセージ フォルダー操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d6347-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="d6347-110">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="d6347-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="d6347-111">Garth が John とメッセージ フォルダーを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="d6347-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="d6347-112">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身のメッセージ フォルダーを取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="d6347-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
```

<span data-ttu-id="d6347-113">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="d6347-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="d6347-114">共有の連絡先フォルダー、予定表、メッセージ フォルダー</span><span class="sxs-lookup"><span data-stu-id="d6347-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="d6347-115">連絡先、イベント、共有フォルダー内のメッセージ</span><span class="sxs-lookup"><span data-stu-id="d6347-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="d6347-116">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="d6347-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="d6347-117">この機能は、連絡先、イベント、メッセージ、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="d6347-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="d6347-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6347-118">Permissions</span></span>
<span data-ttu-id="d6347-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6347-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d6347-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6347-121">Permission type</span></span>      | <span data-ttu-id="d6347-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6347-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6347-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6347-123">Delegated (work or school account)</span></span> | <span data-ttu-id="d6347-124">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6347-124">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d6347-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6347-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6347-126">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6347-126">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="d6347-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6347-127">Application</span></span> | <span data-ttu-id="d6347-128">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6347-128">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6347-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6347-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6347-130">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d6347-130">Optional query parameters</span></span>
<span data-ttu-id="d6347-131">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d6347-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d6347-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6347-132">Request headers</span></span>
| <span data-ttu-id="d6347-133">名前</span><span class="sxs-lookup"><span data-stu-id="d6347-133">Name</span></span>       | <span data-ttu-id="d6347-134">型</span><span class="sxs-lookup"><span data-stu-id="d6347-134">Type</span></span> | <span data-ttu-id="d6347-135">説明</span><span class="sxs-lookup"><span data-stu-id="d6347-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d6347-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6347-136">Authorization</span></span>  | <span data-ttu-id="d6347-137">string</span><span class="sxs-lookup"><span data-stu-id="d6347-137">string</span></span>  | <span data-ttu-id="d6347-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d6347-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6347-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6347-140">Request body</span></span>
<span data-ttu-id="d6347-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d6347-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6347-142">応答</span><span class="sxs-lookup"><span data-stu-id="d6347-142">Response</span></span>

<span data-ttu-id="d6347-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mailFolder](../resources/mailfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d6347-143">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6347-144">例</span><span class="sxs-lookup"><span data-stu-id="d6347-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6347-145">要求</span><span class="sxs-lookup"><span data-stu-id="d6347-145">Request</span></span>
<span data-ttu-id="d6347-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6347-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="d6347-147">応答</span><span class="sxs-lookup"><span data-stu-id="d6347-147">Response</span></span>
<span data-ttu-id="d6347-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6347-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
