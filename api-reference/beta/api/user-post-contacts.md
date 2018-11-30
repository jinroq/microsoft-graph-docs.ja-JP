---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。
ms.openlocfilehash: 8e2745df6e7e43a903020f47cc627aa627e56ca1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067079"
---
# <a name="create-contact"></a><span data-ttu-id="18eaf-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="18eaf-103">Create Contact</span></span>

> <span data-ttu-id="18eaf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18eaf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18eaf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18eaf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18eaf-106">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="18eaf-106">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="18eaf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18eaf-107">Permissions</span></span>
<span data-ttu-id="18eaf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18eaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18eaf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18eaf-110">Permission type</span></span>      | <span data-ttu-id="18eaf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18eaf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18eaf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18eaf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18eaf-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18eaf-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="18eaf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18eaf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18eaf-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18eaf-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="18eaf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18eaf-116">Application</span></span> | <span data-ttu-id="18eaf-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18eaf-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18eaf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18eaf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="18eaf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18eaf-119">Request headers</span></span>
| <span data-ttu-id="18eaf-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18eaf-120">Header</span></span>       | <span data-ttu-id="18eaf-121">値</span><span class="sxs-lookup"><span data-stu-id="18eaf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18eaf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18eaf-122">Authorization</span></span>  | <span data-ttu-id="18eaf-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18eaf-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18eaf-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18eaf-125">Content-Type</span></span>  | <span data-ttu-id="18eaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18eaf-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18eaf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="18eaf-127">Request body</span></span>
<span data-ttu-id="18eaf-128">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="18eaf-128">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="18eaf-129">応答</span><span class="sxs-lookup"><span data-stu-id="18eaf-129">Response</span></span>

<span data-ttu-id="18eaf-130">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体での応答コードおよび[連絡先](../resources/contact.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="18eaf-130">If successful, this method returns `201 Created` response code and [contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18eaf-131">例</span><span class="sxs-lookup"><span data-stu-id="18eaf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18eaf-132">要求</span><span class="sxs-lookup"><span data-stu-id="18eaf-132">Request</span></span>
<span data-ttu-id="18eaf-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18eaf-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="18eaf-134">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="18eaf-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="18eaf-135">応答</span><span class="sxs-lookup"><span data-stu-id="18eaf-135">Response</span></span>
<span data-ttu-id="18eaf-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18eaf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="18eaf-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="18eaf-139">See also</span></span>

- [<span data-ttu-id="18eaf-140">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="18eaf-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="18eaf-141">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="18eaf-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
