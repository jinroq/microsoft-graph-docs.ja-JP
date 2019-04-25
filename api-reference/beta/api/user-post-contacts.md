---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dbac25f4cf86074876fd1be4f0632a5afdb08dc1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544089"
---
# <a name="create-contact"></a><span data-ttu-id="3c481-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="3c481-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c481-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="3c481-104">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="3c481-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3c481-105">Permissions</span></span>
<span data-ttu-id="3c481-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c481-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3c481-108">Permission type</span></span>      | <span data-ttu-id="3c481-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3c481-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c481-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3c481-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c481-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c481-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3c481-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3c481-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c481-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c481-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3c481-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3c481-114">Application</span></span> | <span data-ttu-id="3c481-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c481-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c481-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3c481-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="3c481-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c481-117">Request headers</span></span>
| <span data-ttu-id="3c481-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3c481-118">Header</span></span>       | <span data-ttu-id="3c481-119">値</span><span class="sxs-lookup"><span data-stu-id="3c481-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3c481-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c481-120">Authorization</span></span>  | <span data-ttu-id="3c481-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3c481-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3c481-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c481-123">Content-Type</span></span>  | <span data-ttu-id="3c481-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3c481-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3c481-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3c481-125">Request body</span></span>
<span data-ttu-id="3c481-126">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c481-126">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3c481-127">応答</span><span class="sxs-lookup"><span data-stu-id="3c481-127">Response</span></span>

<span data-ttu-id="3c481-128">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3c481-128">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c481-129">例</span><span class="sxs-lookup"><span data-stu-id="3c481-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c481-130">要求</span><span class="sxs-lookup"><span data-stu-id="3c481-130">Request</span></span>
<span data-ttu-id="3c481-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3c481-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="3c481-132">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3c481-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="3c481-133">応答</span><span class="sxs-lookup"><span data-stu-id="3c481-133">Response</span></span>
<span data-ttu-id="3c481-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3c481-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3c481-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="3c481-137">See also</span></span>

- [<span data-ttu-id="3c481-138">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="3c481-138">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3c481-139">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="3c481-139">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
    "Error: /api-reference/beta/api/user-post-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
