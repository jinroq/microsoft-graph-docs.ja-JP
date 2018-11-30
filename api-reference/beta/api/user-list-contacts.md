---
title: 連絡先を一覧表示する
description: ユーザーのメールボックス内の連絡先を取得します。
ms.openlocfilehash: 2554836607705138702e5b04a60cf4a77a8e53f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067065"
---
# <a name="list-contacts"></a><span data-ttu-id="79409-103">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="79409-103">List contacts</span></span>

> <span data-ttu-id="79409-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79409-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79409-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79409-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79409-106">ユーザーのメールボックス内の連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="79409-106">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="79409-107">アプリケーションが別のユーザーの連絡先フォルダーに連絡先を入手するための 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="79409-107">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="79409-108">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="79409-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="79409-109">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーの連絡先フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="79409-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="79409-110">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79409-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="79409-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79409-111">Permissions</span></span>
<span data-ttu-id="79409-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79409-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79409-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79409-114">Permission type</span></span>      | <span data-ttu-id="79409-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79409-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79409-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79409-116">Delegated (work or school account)</span></span> | <span data-ttu-id="79409-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79409-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="79409-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79409-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79409-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79409-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="79409-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79409-120">Application</span></span> | <span data-ttu-id="79409-121">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79409-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="79409-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79409-122">HTTP request</span></span>

<span data-ttu-id="79409-123">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="79409-123">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="79409-124">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="79409-124">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="79409-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79409-125">Optional query parameters</span></span>
<span data-ttu-id="79409-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79409-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="79409-127">たとえば、`$filter` クエリ パラメーターを使って、メール アドレスのドメインに基づいて連絡先をフィルターすることができます。</span><span class="sxs-lookup"><span data-stu-id="79409-127">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`

## <a name="request-headers"></a><span data-ttu-id="79409-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79409-128">Request headers</span></span>
| <span data-ttu-id="79409-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79409-129">Header</span></span>       | <span data-ttu-id="79409-130">値</span><span class="sxs-lookup"><span data-stu-id="79409-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79409-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="79409-131">Authorization</span></span>  | <span data-ttu-id="79409-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="79409-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79409-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="79409-134">Request body</span></span>
<span data-ttu-id="79409-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79409-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79409-136">応答</span><span class="sxs-lookup"><span data-stu-id="79409-136">Response</span></span>

<span data-ttu-id="79409-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文[にお問い合わせください](../resources/contact.md)のオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="79409-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79409-138">例</span><span class="sxs-lookup"><span data-stu-id="79409-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79409-139">要求</span><span class="sxs-lookup"><span data-stu-id="79409-139">Request</span></span>
<span data-ttu-id="79409-140">次の例では、サインインしているユーザーの連絡先の**表示名**と**emailAddresses**プロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="79409-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="79409-141">応答</span><span class="sxs-lookup"><span data-stu-id="79409-141">Response</span></span>
<span data-ttu-id="79409-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79409-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts(displayName,emailAddresses)",
    "value":[
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
            "id":"AAMkADh6v5AAAvgTCFAAA=",
            "displayName":"Elvis Blank",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Elvis Blank",
                    "address":"elvisb@relecloud.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Elvis Blank",
                    "address":"elvisb@fabrikam.onmicrosoft.com"
                }
            ]
        },
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
            "id":"AAMkADh6v5AAAvgTCEAAA=",
            "displayName":"Pavel Bansky",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Pavel Bansky",
                    "address":"pavelb@contoso.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Pavel Bansky",
                    "address":"pavelb@fabrikam.onmicrosoft.com"
                }
            ]
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
