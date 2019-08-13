---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0892ca0e30aaf65161531005613fb298c61aa10e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326007"
---
# <a name="create-contact"></a><span data-ttu-id="03e15-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="03e15-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03e15-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="03e15-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="03e15-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="03e15-105">Permissions</span></span>
<span data-ttu-id="03e15-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03e15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03e15-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03e15-108">Permission type</span></span>      | <span data-ttu-id="03e15-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="03e15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03e15-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03e15-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03e15-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03e15-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="03e15-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03e15-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03e15-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03e15-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="03e15-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03e15-114">Application</span></span> | <span data-ttu-id="03e15-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03e15-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="03e15-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03e15-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="03e15-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03e15-117">Request headers</span></span>
| <span data-ttu-id="03e15-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03e15-118">Header</span></span>       | <span data-ttu-id="03e15-119">値</span><span class="sxs-lookup"><span data-stu-id="03e15-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="03e15-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="03e15-120">Authorization</span></span>  | <span data-ttu-id="03e15-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="03e15-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="03e15-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03e15-123">Content-Type</span></span>  | <span data-ttu-id="03e15-124">application/json</span><span class="sxs-lookup"><span data-stu-id="03e15-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03e15-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="03e15-125">Request body</span></span>
<span data-ttu-id="03e15-126">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="03e15-126">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="03e15-127">応答</span><span class="sxs-lookup"><span data-stu-id="03e15-127">Response</span></span>

<span data-ttu-id="03e15-128">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="03e15-128">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e15-129">例</span><span class="sxs-lookup"><span data-stu-id="03e15-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03e15-130">要求</span><span class="sxs-lookup"><span data-stu-id="03e15-130">Request</span></span>
<span data-ttu-id="03e15-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03e15-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="03e15-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="03e15-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@contoso.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "personal"
    },
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky",
      "type": "other",
      "otherLabel": "Volunteer work"
    }
  ],
  "phones" : [
    {
      "number": "+1 732 555 0102",
      "type": "business"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="03e15-133">C#</span><span class="sxs-lookup"><span data-stu-id="03e15-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03e15-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03e15-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03e15-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="03e15-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="03e15-136">Java</span><span class="sxs-lookup"><span data-stu-id="03e15-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="03e15-137">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="03e15-137">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="03e15-138">応答</span><span class="sxs-lookup"><span data-stu-id="03e15-138">Response</span></span>
<span data-ttu-id="03e15-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="03e15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T19:56:07Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fW",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@contoso.onmicrosoft.com"
        },
        {
            "otherLabel": "Volunteer work",
            "type":"other",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="03e15-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="03e15-142">See also</span></span>

- [<span data-ttu-id="03e15-143">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="03e15-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="03e15-144">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="03e15-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
