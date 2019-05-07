---
title: 連絡先を一覧表示する
description: ユーザーのメールボックス内の連絡先を取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 97cc72958ecd992cd4854da68d58074ddb809887
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637305"
---
# <a name="list-contacts"></a><span data-ttu-id="b0dcb-103">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b0dcb-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0dcb-104">ユーザーのメールボックス内の連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="b0dcb-105">アプリが別のユーザーの連絡先フォルダーから連絡先を取得できるシナリオは2つあります。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="b0dcb-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="b0dcb-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b0dcb-107">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーとコンタクトフォルダーを共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b0dcb-108">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="b0dcb-109">権限</span><span class="sxs-lookup"><span data-stu-id="b0dcb-109">Permissions</span></span>
<span data-ttu-id="b0dcb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0dcb-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0dcb-112">Permission type</span></span>      | <span data-ttu-id="b0dcb-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0dcb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0dcb-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0dcb-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b0dcb-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0dcb-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b0dcb-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0dcb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0dcb-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0dcb-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="b0dcb-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0dcb-118">Application</span></span> | <span data-ttu-id="b0dcb-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0dcb-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0dcb-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0dcb-120">HTTP request</span></span>

<span data-ttu-id="b0dcb-121">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="b0dcb-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="b0dcb-122">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="b0dcb-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0dcb-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0dcb-123">Optional query parameters</span></span>
<span data-ttu-id="b0dcb-124">たとえば、`$filter` クエリ パラメーターを使って、メール アドレスに基づいて連絡先をフィルターすることができます。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="b0dcb-125">`$filter`、`any`そして`eq`演算子を使用できるのは**emailAddresses**コレクションの**address**サブプロパティのみなので注意が必要です 。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="b0dcb-126">すなわち、**氏名** または**emailAddresses**の 1 つのインスタンスの他のサブ プロパティでフィルター抽出することはできませんし、`filter` 以下のような `ne`, `le`や `startswith()`その他の演算子や関数を適用したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="b0dcb-127">`$filter`クエリのパラメーターの一般的な情報については、[OData クエリ パラメーター](/graph/query-parameters)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0dcb-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0dcb-128">Request headers</span></span>
| <span data-ttu-id="b0dcb-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0dcb-129">Header</span></span>       | <span data-ttu-id="b0dcb-130">値</span><span class="sxs-lookup"><span data-stu-id="b0dcb-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b0dcb-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0dcb-131">Authorization</span></span>  | <span data-ttu-id="b0dcb-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b0dcb-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0dcb-134">Request body</span></span>
<span data-ttu-id="b0dcb-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0dcb-136">応答</span><span class="sxs-lookup"><span data-stu-id="b0dcb-136">Response</span></span>

<span data-ttu-id="b0dcb-137">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[contact](../resources/contact.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0dcb-138">例</span><span class="sxs-lookup"><span data-stu-id="b0dcb-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0dcb-139">要求</span><span class="sxs-lookup"><span data-stu-id="b0dcb-139">Request</span></span>
<span data-ttu-id="b0dcb-140">次の例では、サインインしているユーザーの連絡先の**displayName**と**emailaddresses**のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="b0dcb-141">応答</span><span class="sxs-lookup"><span data-stu-id="b0dcb-141">Response</span></span>
<span data-ttu-id="b0dcb-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0dcb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b0dcb-145">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="b0dcb-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b0dcb-146">Visual</span><span class="sxs-lookup"><span data-stu-id="b0dcb-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_contacts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0dcb-147">Java</span><span class="sxs-lookup"><span data-stu-id="b0dcb-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_contacts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
