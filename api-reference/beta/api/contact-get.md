---
title: 連絡先を取得する
description: 連絡先オブジェクトのプロパティと関係を取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 537a0fda80ca2f034782e99e25fb069cf667e135
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437685"
---
# <a name="get-contact"></a><span data-ttu-id="6d5b4-103">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="6d5b4-103">Get contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d5b4-104">連絡先オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-104">Retrieve the properties and relationships of contact object.</span></span>

<span data-ttu-id="6d5b4-105">アプリでは、次の2つのシナリオを使用して、別のユーザーの連絡先フォルダーに連絡先を取得できます。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-105">There are two scenarios where an app can get a contact in another user's contact folder:</span></span>

* <span data-ttu-id="6d5b4-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="6d5b4-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="6d5b4-107">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーとコンタクトフォルダーを共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="6d5b4-108">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="6d5b4-109">権限</span><span class="sxs-lookup"><span data-stu-id="6d5b4-109">Permissions</span></span>
<span data-ttu-id="6d5b4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d5b4-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d5b4-112">Permission type</span></span>      | <span data-ttu-id="6d5b4-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d5b4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d5b4-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d5b4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6d5b4-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d5b4-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6d5b4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d5b4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d5b4-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d5b4-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6d5b4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d5b4-118">Application</span></span> | <span data-ttu-id="6d5b4-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d5b4-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d5b4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d5b4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="6d5b4-121">ユーザーのメールボックス内の[連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-121">A [contact](../resources/contact.md) in the user's mailbox.</span></span>
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="6d5b4-122">ユーザーのトップレベルの[Contactfolder](../resources/contactfolder.md)からの[連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-122">A [contact](../resources/contact.md) from a top level [contactFolder](../resources/contactfolder.md) of the user's.</span></span>
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
<span data-ttu-id="6d5b4-123">[contactFolder](../resources/contact.md) の子フォルダー内に含まれる [連絡先](../resources/mailfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-123">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="6d5b4-124">次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-124">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d5b4-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6d5b4-125">Optional query parameters</span></span>
|<span data-ttu-id="6d5b4-126">名前</span><span class="sxs-lookup"><span data-stu-id="6d5b4-126">Name</span></span>|<span data-ttu-id="6d5b4-127">値</span><span class="sxs-lookup"><span data-stu-id="6d5b4-127">Value</span></span>|<span data-ttu-id="6d5b4-128">説明</span><span class="sxs-lookup"><span data-stu-id="6d5b4-128">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="6d5b4-129">$expand</span><span class="sxs-lookup"><span data-stu-id="6d5b4-129">$expand</span></span>|<span data-ttu-id="6d5b4-130">string</span><span class="sxs-lookup"><span data-stu-id="6d5b4-130">string</span></span>|<span data-ttu-id="6d5b4-131">展開して応答に含める関係を示すコンマ区切りのリスト。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-131">Comma-separated list of relationships to expand and include in the response.</span></span> <span data-ttu-id="6d5b4-132">サポートされて[](../resources/contact.md)いる名前については、「リレーションシップ」の表を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-132">See relationships table of [contact](../resources/contact.md) object for supported names.</span></span> |
|<span data-ttu-id="6d5b4-133">$select</span><span class="sxs-lookup"><span data-stu-id="6d5b4-133">$select</span></span>|<span data-ttu-id="6d5b4-134">string</span><span class="sxs-lookup"><span data-stu-id="6d5b4-134">string</span></span>|<span data-ttu-id="6d5b4-135">応答に含めるプロパティを示すコンマ区切りのリスト。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-135">Comma-separated list of properties to include in the response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6d5b4-136">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d5b4-136">Request headers</span></span>
| <span data-ttu-id="6d5b4-137">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d5b4-137">Header</span></span>       | <span data-ttu-id="6d5b4-138">値</span><span class="sxs-lookup"><span data-stu-id="6d5b4-138">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d5b4-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d5b4-139">Authorization</span></span>  | <span data-ttu-id="6d5b4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d5b4-142">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d5b4-142">Request body</span></span>
<span data-ttu-id="6d5b4-143">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d5b4-144">応答</span><span class="sxs-lookup"><span data-stu-id="6d5b4-144">Response</span></span>

<span data-ttu-id="6d5b4-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-145">If successful, this method returns a `200 OK` response code and [contact](../resources/contact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d5b4-146">例</span><span class="sxs-lookup"><span data-stu-id="6d5b4-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d5b4-147">要求</span><span class="sxs-lookup"><span data-stu-id="6d5b4-147">Request</span></span>
<span data-ttu-id="6d5b4-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6d5b4-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6d5b4-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d5b4-150">C#</span><span class="sxs-lookup"><span data-stu-id="6d5b4-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d5b4-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d5b4-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d5b4-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="6d5b4-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6d5b4-153">応答</span><span class="sxs-lookup"><span data-stu-id="6d5b4-153">Response</span></span>
<span data-ttu-id="6d5b4-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6d5b4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com",
      "type": "unknown"
    },
    {
      "name": "Garth",
      "address": "garth@contoso.onmicrosoft.com",
      "type": "personal"
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
  "assistantName": null,
  "manager": null,
  "phones": [{
    "type": "business",
    "number": "+1 918 555 0101"
  }],
  "postalAddresses": [{
    "type": "business",
    "postOfficeBox": "P.O. Box 100",
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "countryOrRegion": "USA",
    "postalCode": "98121"
  }],
  "spouseName": null,
  "personalNotes": null,
  "children": [], 
  "gender": null,
  "websites": [{
      "type": "work",
      "address": "https://www.contoso.com",
      "name": "Contoso"
  }],
  "weddingAnniversary": null
}
```

## <a name="see-also"></a><span data-ttu-id="6d5b4-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d5b4-157">See also</span></span>

- [<span data-ttu-id="6d5b4-158">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="6d5b4-158">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6d5b4-159">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6d5b4-159">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
