# <a name="get-contactfolder"></a><span data-ttu-id="3c1a2-101">Get contactFolder</span><span class="sxs-lookup"><span data-stu-id="3c1a2-101">Get contactFolder</span></span>

<span data-ttu-id="3c1a2-102">連絡先フォルダー ID を使用して連絡先フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-102">Get a contact folder by using the contact folder ID.</span></span>


### <a name="get-another-users-contact-folder"></a><span data-ttu-id="3c1a2-103">他のユーザーの連絡先フォルダーを取得</span><span class="sxs-lookup"><span data-stu-id="3c1a2-103">Get another user's contact folder</span></span>

<span data-ttu-id="3c1a2-104">アプリケーションのアクセス許可がある場合や、1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合には、別のユーザーの連絡先フォルダーを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to a get contact folder of another user's.</span></span> <span data-ttu-id="3c1a2-105">このセクションでは、委任されたアクセス許可に関連するシナリオに焦点を当てます。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="3c1a2-106">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="3c1a2-107">別のユーザー Garth は、John と連絡先フォルダーを共有しています。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="3c1a2-108">その場合、以下に示す例のクエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有フォルダーを取得できます。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-108">You can get that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contactFolders/{id}
```

<span data-ttu-id="3c1a2-109">この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対するすべての GET 連絡先フォルダー操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-109">This capability applies to all GET contact folder operations for an individual user, as described in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="3c1a2-110">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="3c1a2-111">Garth が John と連絡先フォルダーを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="3c1a2-112">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身の連絡先フォルダーを取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-112">In such cases, specifying a user ID or user principal name only works for getting a contact folder of the signed-in user’s, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
```

<span data-ttu-id="3c1a2-113">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="3c1a2-114">共有の連絡先フォルダー</span><span class="sxs-lookup"><span data-stu-id="3c1a2-114">Shared contact folders</span></span>
- <span data-ttu-id="3c1a2-115">共有の予定表</span><span class="sxs-lookup"><span data-stu-id="3c1a2-115">Shared calendars</span></span>
- <span data-ttu-id="3c1a2-116">共有フォルダー内の連絡先およびイベント</span><span class="sxs-lookup"><span data-stu-id="3c1a2-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="3c1a2-117">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="3c1a2-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="3c1a2-118">この機能は、連絡先、イベント、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="3c1a2-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3c1a2-119">Permissions</span></span>
<span data-ttu-id="3c1a2-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3c1a2-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c1a2-122">Permission type</span></span>      | <span data-ttu-id="3c1a2-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c1a2-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c1a2-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c1a2-124">Delegated (work or school account)</span></span> | <span data-ttu-id="3c1a2-125">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c1a2-125">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3c1a2-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c1a2-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c1a2-127">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c1a2-127">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3c1a2-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c1a2-128">Application</span></span> | <span data-ttu-id="3c1a2-129">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c1a2-129">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c1a2-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c1a2-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c1a2-131">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3c1a2-131">Optional query parameters</span></span>
<span data-ttu-id="3c1a2-132">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-132">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3c1a2-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c1a2-133">Request headers</span></span>
| <span data-ttu-id="3c1a2-134">名前</span><span class="sxs-lookup"><span data-stu-id="3c1a2-134">Name</span></span>       | <span data-ttu-id="3c1a2-135">型</span><span class="sxs-lookup"><span data-stu-id="3c1a2-135">Type</span></span> | <span data-ttu-id="3c1a2-136">説明</span><span class="sxs-lookup"><span data-stu-id="3c1a2-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3c1a2-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c1a2-137">Authorization</span></span>  | <span data-ttu-id="3c1a2-138">string</span><span class="sxs-lookup"><span data-stu-id="3c1a2-138">string</span></span>  | <span data-ttu-id="3c1a2-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c1a2-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c1a2-141">Request body</span></span>
<span data-ttu-id="3c1a2-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c1a2-143">応答</span><span class="sxs-lookup"><span data-stu-id="3c1a2-143">Response</span></span>

<span data-ttu-id="3c1a2-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [contactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-144">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c1a2-145">例</span><span class="sxs-lookup"><span data-stu-id="3c1a2-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c1a2-146">要求</span><span class="sxs-lookup"><span data-stu-id="3c1a2-146">Request</span></span>
<span data-ttu-id="3c1a2-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="3c1a2-148">応答</span><span class="sxs-lookup"><span data-stu-id="3c1a2-148">Response</span></span>
<span data-ttu-id="3c1a2-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c1a2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
