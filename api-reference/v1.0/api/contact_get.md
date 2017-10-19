# <a name="get-contact"></a><span data-ttu-id="3452e-101">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="3452e-101">Get contact</span></span>

<span data-ttu-id="3452e-102">連絡先オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="3452e-102">Retrieve the properties and relationships of a contact object.</span></span>


### <a name="get-contacts-in-another-users-contact-folder"></a><span data-ttu-id="3452e-103">他のユーザーの連絡先フォルダーで連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="3452e-103">Get contacts in another user's contact folder</span></span>

<span data-ttu-id="3452e-104">アプリケーションのアクセス許可がある場合、または 1 人のユーザーから適切に委任された[アクセス許可](#permissions)がある場合、別のユーザーの連絡先フォルダーから連絡先を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="3452e-104">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get contacts from another user's contact folder.</span></span> <span data-ttu-id="3452e-105">このセクションでは、委任されたアクセス許可に関連するシナリオに焦点を当てます。</span><span class="sxs-lookup"><span data-stu-id="3452e-105">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="3452e-106">たとえば、アプリがユーザー John から委任されたアクセス許可を取得したとします。</span><span class="sxs-lookup"><span data-stu-id="3452e-106">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="3452e-107">別のユーザー Garth は、John と連絡先フォルダーを共有しています。</span><span class="sxs-lookup"><span data-stu-id="3452e-107">Suppose another user, Garth, has shared a contact folder with John.</span></span> <span data-ttu-id="3452e-108">その場合、以下に示す例のクエリで、Garth のユーザー ID (またはユーザー プリンシパル名) を指定することにより、その共有フォルダーで連絡先を取得できます。</span><span class="sxs-lookup"><span data-stu-id="3452e-108">You can get a contact in that shared folder by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts/{id}
```

<span data-ttu-id="3452e-109">この機能は、後述の [HTTP 要求](#http-request)セクションに記載されている、個々のユーザーに対しサポートされているすべての GET 連絡先操作に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3452e-109">This capability applies to all the supported GET contacts operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="3452e-110">これは、Garth が John にメールボックス全体を委任した場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="3452e-110">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="3452e-111">Garth が John と連絡先フォルダーを共有していない、もしくはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="3452e-111">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="3452e-112">このような場合、ユーザー ID またはユーザー プリンシパル名の指定は、サインインしているユーザー自身の連絡先フォルダーで連絡先を取得するためにのみ使用でき、そのクエリは /me ショートカットを使用することと同義となります。</span><span class="sxs-lookup"><span data-stu-id="3452e-112">In such cases, specifying a user ID or user principal name only works for getting a contact in the signed-in user’s own contact folders, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}
```

<span data-ttu-id="3452e-113">この機能は、以下の GET 操作でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="3452e-113">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="3452e-114">共有の連絡先フォルダー</span><span class="sxs-lookup"><span data-stu-id="3452e-114">Shared contact folders</span></span>
- <span data-ttu-id="3452e-115">共有の予定表</span><span class="sxs-lookup"><span data-stu-id="3452e-115">Shared calendars</span></span>
- <span data-ttu-id="3452e-116">共有フォルダー内の連絡先およびイベント</span><span class="sxs-lookup"><span data-stu-id="3452e-116">Contacts and events in shared folders</span></span>
- <span data-ttu-id="3452e-117">委任されたメールボックス内の上述のリソース</span><span class="sxs-lookup"><span data-stu-id="3452e-117">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="3452e-118">この機能は、連絡先、イベント、それらのフォルダーに対する他の操作では使用できません。</span><span class="sxs-lookup"><span data-stu-id="3452e-118">This capability is not available in other operations for contacts, events, and their folders.</span></span>


## <a name="permissions"></a><span data-ttu-id="3452e-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3452e-119">Permissions</span></span>
<span data-ttu-id="3452e-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3452e-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3452e-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3452e-122">Permission type</span></span>      | <span data-ttu-id="3452e-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3452e-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3452e-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3452e-124">Delegated (work or school account)</span></span> | <span data-ttu-id="3452e-125">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3452e-125">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3452e-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3452e-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3452e-127">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3452e-127">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3452e-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3452e-128">Application</span></span> | <span data-ttu-id="3452e-129">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3452e-129">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3452e-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3452e-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="3452e-131">ユーザーの既定 [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="3452e-131">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="3452e-132">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="3452e-132">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="3452e-p106">[contactFolder](../resources/mailfolder.md) の子フォルダー内に含まれる [連絡先](../resources/contact.md)。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="3452e-p106">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3452e-135">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3452e-135">Optional query parameters</span></span>
|<span data-ttu-id="3452e-136">名前</span><span class="sxs-lookup"><span data-stu-id="3452e-136">Name</span></span>|<span data-ttu-id="3452e-137">値</span><span class="sxs-lookup"><span data-stu-id="3452e-137">Value</span></span>|<span data-ttu-id="3452e-138">説明</span><span class="sxs-lookup"><span data-stu-id="3452e-138">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="3452e-139">$expand</span><span class="sxs-lookup"><span data-stu-id="3452e-139">$expand</span></span>|<span data-ttu-id="3452e-140">string</span><span class="sxs-lookup"><span data-stu-id="3452e-140">string</span></span>|<span data-ttu-id="3452e-p107">展開して応答に含める関係を示すコンマ区切りのリスト。サポートされている名前に関しては、[連絡先](../resources/contact.md) オブジェクトの関係表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3452e-p107">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="3452e-143">$select</span><span class="sxs-lookup"><span data-stu-id="3452e-143">$select</span></span>|<span data-ttu-id="3452e-144">string</span><span class="sxs-lookup"><span data-stu-id="3452e-144">string</span></span>|<span data-ttu-id="3452e-145">応答に含めるプロパティを示すコンマ区切りのリスト。</span><span class="sxs-lookup"><span data-stu-id="3452e-145">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3452e-146">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3452e-146">Request headers</span></span>
| <span data-ttu-id="3452e-147">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3452e-147">Header</span></span>       | <span data-ttu-id="3452e-148">値</span><span class="sxs-lookup"><span data-stu-id="3452e-148">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3452e-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="3452e-149">Authorization</span></span>  | <span data-ttu-id="3452e-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3452e-p108">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3452e-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="3452e-152">Request body</span></span>
<span data-ttu-id="3452e-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3452e-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3452e-154">応答</span><span class="sxs-lookup"><span data-stu-id="3452e-154">Response</span></span>

<span data-ttu-id="3452e-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3452e-155">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3452e-156">例</span><span class="sxs-lookup"><span data-stu-id="3452e-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3452e-157">要求</span><span class="sxs-lookup"><span data-stu-id="3452e-157">Request</span></span>
<span data-ttu-id="3452e-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3452e-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="3452e-159">応答</span><span class="sxs-lookup"><span data-stu-id="3452e-159">Response</span></span>
<span data-ttu-id="3452e-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3452e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1977

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "businessHomePage": "http://www.contoso.com",
  "assistantName": null,
  "manager": null,
  "homePhones": [],
  "mobilePhone": null,
  "businessPhones": [
    "+1 918 555 0101"
  ],
  "homeAddress": {},
  "businessAddress": {
      "street": "10 Contoso Way",
      "city": "Redmond",
      "state": "WA",
      "countryOrRegion": "USA",
      "postalCode": "98075"  
  },
  "otherAddress": {},
  "spouseName": null,
  "personalNotes": null,
  "children": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
