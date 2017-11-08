# <a name="list-contacts"></a><span data-ttu-id="8a4ae-101">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8a4ae-101">List contacts</span></span>

<span data-ttu-id="8a4ae-102">サインイン中のユーザーの既定の連絡先フォルダーから連絡先コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="8a4ae-103">他のユーザーの連絡先フォルダーで連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="8a4ae-104">アプリケーションのアクセス許可がある場合、または 1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合、別のユーザーの連絡先フォルダーから連絡先を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="8a4ae-105">このセクションでは、委任されたアクセス許可に関連するシナリオに焦点を当てます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="8a4ae-106">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="8a4ae-107">別のユーザー Garth は、John と連絡先フォルダーを共有しています。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="8a4ae-108">その場合、以下に示す例のクエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有フォルダーで連絡先を取得できます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-108">You can get the contacts in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

<span data-ttu-id="8a4ae-109">この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対しサポートされているすべての GET 連絡先操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="8a4ae-110">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="8a4ae-111">Garth が John と連絡先フォルダーを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="8a4ae-112">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身の連絡先フォルダーで連絡先を取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-112">In such cases, specifying a user ID or user principal name only works for getting contacts in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
```

<span data-ttu-id="8a4ae-113">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="8a4ae-114">共有の連絡先フォルダー、予定表、メッセージ フォルダー</span><span class="sxs-lookup"><span data-stu-id="8a4ae-114">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="8a4ae-115">連絡先、イベント、共有フォルダー内のメッセージ</span><span class="sxs-lookup"><span data-stu-id="8a4ae-115">Contacts and events in shared folders</span></span>
- <span data-ttu-id="8a4ae-116">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="8a4ae-116">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="8a4ae-117">この機能は、連絡先、イベント、メッセージ、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-117">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="8a4ae-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a4ae-118">Permissions</span></span>
<span data-ttu-id="8a4ae-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8a4ae-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a4ae-121">Permission type</span></span>      | <span data-ttu-id="8a4ae-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a4ae-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a4ae-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a4ae-123">Delegated (work or school account)</span></span> | <span data-ttu-id="8a4ae-124">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4ae-124">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8a4ae-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a4ae-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a4ae-126">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4ae-126">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8a4ae-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a4ae-127">Application</span></span> | <span data-ttu-id="8a4ae-128">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a4ae-128">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a4ae-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a4ae-129">HTTP request</span></span>

<span data-ttu-id="8a4ae-130">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="8a4ae-130">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="8a4ae-131">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="8a4ae-131">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8a4ae-132">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a4ae-132">Optional query parameters</span></span>
<span data-ttu-id="8a4ae-133">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-133">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="8a4ae-134">たとえば、`$filter` クエリ パラメーターを使って、メール アドレスのドメインに基づいて連絡先をフィルターすることができます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-134">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="8a4ae-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a4ae-135">Request headers</span></span>
| <span data-ttu-id="8a4ae-136">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a4ae-136">Header</span></span>       | <span data-ttu-id="8a4ae-137">値</span><span class="sxs-lookup"><span data-stu-id="8a4ae-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a4ae-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a4ae-138">Authorization</span></span>  | <span data-ttu-id="8a4ae-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a4ae-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a4ae-141">Content-Type</span></span>   | <span data-ttu-id="8a4ae-142">application/json</span><span class="sxs-lookup"><span data-stu-id="8a4ae-142">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a4ae-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a4ae-143">Request body</span></span>
<span data-ttu-id="8a4ae-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a4ae-145">応答</span><span class="sxs-lookup"><span data-stu-id="8a4ae-145">Response</span></span>

<span data-ttu-id="8a4ae-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-146">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a4ae-147">例</span><span class="sxs-lookup"><span data-stu-id="8a4ae-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a4ae-148">要求</span><span class="sxs-lookup"><span data-stu-id="8a4ae-148">Request</span></span>
<span data-ttu-id="8a4ae-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="8a4ae-150">応答</span><span class="sxs-lookup"><span data-stu-id="8a4ae-150">Response</span></span>
<span data-ttu-id="8a4ae-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a4ae-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
