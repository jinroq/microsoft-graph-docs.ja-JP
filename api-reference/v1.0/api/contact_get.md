# <a name="get-contact"></a><span data-ttu-id="7466a-101">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="7466a-101">Get contact</span></span>

<span data-ttu-id="7466a-102">連絡先オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="7466a-102">Retrieve the properties and relationships of a contact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7466a-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7466a-103">Permissions</span></span>
<span data-ttu-id="7466a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7466a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7466a-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7466a-106">Permission type</span></span>      | <span data-ttu-id="7466a-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7466a-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7466a-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7466a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7466a-109">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7466a-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7466a-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7466a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7466a-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7466a-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7466a-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7466a-112">Application</span></span> | <span data-ttu-id="7466a-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7466a-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7466a-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7466a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="7466a-115">ユーザーの既定 [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="7466a-115">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="7466a-116">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="7466a-116">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="7466a-p102">[contactFolder](../resources/mailfolder.md) の子フォルダー内に含まれる [連絡先](../resources/contact.md)。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="7466a-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7466a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7466a-119">Optional query parameters</span></span>
|<span data-ttu-id="7466a-120">名前</span><span class="sxs-lookup"><span data-stu-id="7466a-120">Name</span></span>|<span data-ttu-id="7466a-121">値</span><span class="sxs-lookup"><span data-stu-id="7466a-121">Value</span></span>|<span data-ttu-id="7466a-122">説明</span><span class="sxs-lookup"><span data-stu-id="7466a-122">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="7466a-123">$expand</span><span class="sxs-lookup"><span data-stu-id="7466a-123">$expand</span></span>|<span data-ttu-id="7466a-124">string</span><span class="sxs-lookup"><span data-stu-id="7466a-124">string</span></span>|<span data-ttu-id="7466a-p103">展開して応答に含める関係を示すコンマ区切りのリスト。サポートされている名前に関しては、[連絡先](../resources/contact.md) オブジェクトの関係表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7466a-p103">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="7466a-127">$select</span><span class="sxs-lookup"><span data-stu-id="7466a-127">$select</span></span>|<span data-ttu-id="7466a-128">string</span><span class="sxs-lookup"><span data-stu-id="7466a-128">string</span></span>|<span data-ttu-id="7466a-129">応答に含めるプロパティを示すコンマ区切りのリスト。</span><span class="sxs-lookup"><span data-stu-id="7466a-129">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7466a-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7466a-130">Request headers</span></span>
| <span data-ttu-id="7466a-131">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7466a-131">Header</span></span>       | <span data-ttu-id="7466a-132">値</span><span class="sxs-lookup"><span data-stu-id="7466a-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7466a-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="7466a-133">Authorization</span></span>  | <span data-ttu-id="7466a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7466a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7466a-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="7466a-136">Request body</span></span>
<span data-ttu-id="7466a-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7466a-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7466a-138">応答</span><span class="sxs-lookup"><span data-stu-id="7466a-138">Response</span></span>

<span data-ttu-id="7466a-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7466a-139">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7466a-140">例</span><span class="sxs-lookup"><span data-stu-id="7466a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7466a-141">要求</span><span class="sxs-lookup"><span data-stu-id="7466a-141">Request</span></span>
<span data-ttu-id="7466a-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7466a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="7466a-143">応答</span><span class="sxs-lookup"><span data-stu-id="7466a-143">Response</span></span>
<span data-ttu-id="7466a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7466a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
