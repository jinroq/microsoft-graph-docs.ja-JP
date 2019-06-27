---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fabcaa698c21b4a0118ca108861ffde4b751374a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269959"
---
# <a name="create-contact"></a><span data-ttu-id="1ba3a-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="1ba3a-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ba3a-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="1ba3a-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ba3a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ba3a-105">Permissions</span></span>
<span data-ttu-id="1ba3a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ba3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ba3a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ba3a-108">Permission type</span></span>      | <span data-ttu-id="1ba3a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ba3a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ba3a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ba3a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ba3a-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ba3a-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1ba3a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ba3a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ba3a-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ba3a-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1ba3a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ba3a-114">Application</span></span> | <span data-ttu-id="1ba3a-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ba3a-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ba3a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ba3a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="1ba3a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ba3a-117">Request headers</span></span>
| <span data-ttu-id="1ba3a-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ba3a-118">Header</span></span>       | <span data-ttu-id="1ba3a-119">値</span><span class="sxs-lookup"><span data-stu-id="1ba3a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ba3a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ba3a-120">Authorization</span></span>  | <span data-ttu-id="1ba3a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1ba3a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1ba3a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ba3a-123">Content-Type</span></span>  | <span data-ttu-id="1ba3a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ba3a-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ba3a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ba3a-125">Request body</span></span>
<span data-ttu-id="1ba3a-126">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ba3a-126">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1ba3a-127">応答</span><span class="sxs-lookup"><span data-stu-id="1ba3a-127">Response</span></span>

<span data-ttu-id="1ba3a-128">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1ba3a-128">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ba3a-129">例</span><span class="sxs-lookup"><span data-stu-id="1ba3a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ba3a-130">要求</span><span class="sxs-lookup"><span data-stu-id="1ba3a-130">Request</span></span>
<span data-ttu-id="1ba3a-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1ba3a-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="1ba3a-132">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ba3a-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="1ba3a-133">応答</span><span class="sxs-lookup"><span data-stu-id="1ba3a-133">Response</span></span>
<span data-ttu-id="1ba3a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ba3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ba3a-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="1ba3a-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ba3a-138">C#</span><span class="sxs-lookup"><span data-stu-id="1ba3a-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ba3a-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ba3a-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1ba3a-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="1ba3a-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_contact_from_user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="1ba3a-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ba3a-141">See also</span></span>

- [<span data-ttu-id="1ba3a-142">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="1ba3a-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1ba3a-143">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="1ba3a-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
