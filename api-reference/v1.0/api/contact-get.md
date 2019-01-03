---
title: 連絡先を取得する
description: 連絡先オブジェクトのプロパティとリレーションシップを取得します。
author: angelgolfer-ms
ms.openlocfilehash: 20677bd9cf10f1098ff233a8f60d69e7728aab85
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331487"
---
# <a name="get-contact"></a><span data-ttu-id="ab103-103">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="ab103-103">Get contact</span></span>

<span data-ttu-id="ab103-104">連絡先オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="ab103-104">Retrieve the properties and relationships of a contact object.</span></span>

<span data-ttu-id="ab103-105">2 つシナリオは、アプリケーションが別のユーザーの連絡先フォルダーに連絡先を取得する場所です。</span><span class="sxs-lookup"><span data-stu-id="ab103-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="ab103-106">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="ab103-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ab103-107">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーの連絡先フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="ab103-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ab103-108">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab103-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="ab103-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab103-109">Permissions</span></span>
<span data-ttu-id="ab103-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab103-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab103-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab103-112">Permission type</span></span>      | <span data-ttu-id="ab103-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab103-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab103-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab103-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ab103-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab103-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ab103-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab103-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab103-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab103-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="ab103-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab103-118">Application</span></span> | <span data-ttu-id="ab103-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab103-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab103-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab103-120">HTTP request</span></span>
<span data-ttu-id="ab103-121"><!-- { "blockType": "ignored" } -->[連絡先](../resources/contact.md)ユーザーの既定の[contactFolder](../resources/contactfolder.md)からです。</span><span class="sxs-lookup"><span data-stu-id="ab103-121"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="ab103-122">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="ab103-122">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="ab103-p103">[contactFolder](../resources/mailfolder.md) の子フォルダー内に含まれる [連絡先](../resources/contact.md)。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="ab103-p103">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab103-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ab103-125">Optional query parameters</span></span>
|<span data-ttu-id="ab103-126">名前</span><span class="sxs-lookup"><span data-stu-id="ab103-126">Name</span></span>|<span data-ttu-id="ab103-127">値</span><span class="sxs-lookup"><span data-stu-id="ab103-127">Value</span></span>|<span data-ttu-id="ab103-128">説明</span><span class="sxs-lookup"><span data-stu-id="ab103-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="ab103-129">$expand</span><span class="sxs-lookup"><span data-stu-id="ab103-129">$expand</span></span>|<span data-ttu-id="ab103-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ab103-130">string</span></span>|<span data-ttu-id="ab103-p104">展開して応答に含める関係を示すコンマ区切りのリスト。サポートされている名前に関しては、[連絡先](../resources/contact.md) オブジェクトの関係表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab103-p104">Comma-separated list of relationships to expand and include in the response. See the relationships table of the [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="ab103-133">$select</span><span class="sxs-lookup"><span data-stu-id="ab103-133">$select</span></span>|<span data-ttu-id="ab103-134">文字列</span><span class="sxs-lookup"><span data-stu-id="ab103-134">string</span></span>|<span data-ttu-id="ab103-135">応答に含めるプロパティを示すコンマ区切りのリスト。</span><span class="sxs-lookup"><span data-stu-id="ab103-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="ab103-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab103-136">Request headers</span></span>
| <span data-ttu-id="ab103-137">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab103-137">Header</span></span>       | <span data-ttu-id="ab103-138">値</span><span class="sxs-lookup"><span data-stu-id="ab103-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ab103-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab103-139">Authorization</span></span>  | <span data-ttu-id="ab103-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ab103-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ab103-142">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab103-142">Request body</span></span>
<span data-ttu-id="ab103-143">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ab103-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab103-144">応答</span><span class="sxs-lookup"><span data-stu-id="ab103-144">Response</span></span>

<span data-ttu-id="ab103-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ab103-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab103-146">例</span><span class="sxs-lookup"><span data-stu-id="ab103-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab103-147">要求</span><span class="sxs-lookup"><span data-stu-id="ab103-147">Request</span></span>
<span data-ttu-id="ab103-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ab103-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="ab103-149">応答</span><span class="sxs-lookup"><span data-stu-id="ab103-149">Response</span></span>
<span data-ttu-id="ab103-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ab103-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "businessHomePage": "https://www.contoso.com",
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