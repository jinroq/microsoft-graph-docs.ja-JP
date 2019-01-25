---
title: 連絡先を一覧表示する
description: ユーザーのメールボックス内の連絡先を取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c444a818b933196ddc46ae0d12d64355656bd7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510912"
---
# <a name="list-contacts"></a><span data-ttu-id="e4261-103">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e4261-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4261-104">ユーザーのメールボックス内の連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="e4261-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="e4261-105">アプリケーションが別のユーザーの連絡先フォルダーに連絡先を入手するための 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="e4261-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="e4261-106">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="e4261-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="e4261-107">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーの連絡先フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="e4261-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="e4261-108">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4261-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="e4261-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e4261-109">Permissions</span></span>
<span data-ttu-id="e4261-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4261-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4261-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e4261-112">Permission type</span></span>      | <span data-ttu-id="e4261-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e4261-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4261-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e4261-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e4261-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4261-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e4261-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e4261-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4261-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4261-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e4261-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4261-118">Application</span></span> | <span data-ttu-id="e4261-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4261-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4261-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e4261-120">HTTP request</span></span>

<span data-ttu-id="e4261-121">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="e4261-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="e4261-122">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="e4261-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4261-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e4261-123">Optional query parameters</span></span>
<span data-ttu-id="e4261-124">使用することができます、`$filter`の電子メール アドレスに基づいて、連絡先をフィルターするクエリのパラメーター。</span><span class="sxs-lookup"><span data-stu-id="e4261-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="e4261-125">注使用することができます`$filter`、`any`と`eq`演算子、 **emailAddresses**コレクション内のインスタンスの**アドレス**サブ プロパティのみにします。</span><span class="sxs-lookup"><span data-stu-id="e4261-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="e4261-126">**名前**または他のサブの**emailAddresses**インスタンスのプロパティにフィルターを適用することはできずするその他の演算子を適用したり、機能を持つ`filter`、次のように`ne`、`le`と`startswith()`。</span><span class="sxs-lookup"><span data-stu-id="e4261-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="e4261-127">全般については、`$filter`クエリのパラメーターで、 [OData クエリのパラメーター](/graph/query-parameters)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4261-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4261-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4261-128">Request headers</span></span>
| <span data-ttu-id="e4261-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4261-129">Header</span></span>       | <span data-ttu-id="e4261-130">値</span><span class="sxs-lookup"><span data-stu-id="e4261-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4261-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4261-131">Authorization</span></span>  | <span data-ttu-id="e4261-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e4261-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4261-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="e4261-134">Request body</span></span>
<span data-ttu-id="e4261-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e4261-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4261-136">応答</span><span class="sxs-lookup"><span data-stu-id="e4261-136">Response</span></span>

<span data-ttu-id="e4261-137">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文[にお問い合わせください](../resources/contact.md)のオブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e4261-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4261-138">例</span><span class="sxs-lookup"><span data-stu-id="e4261-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4261-139">要求</span><span class="sxs-lookup"><span data-stu-id="e4261-139">Request</span></span>
<span data-ttu-id="e4261-140">次の例では、サインインしているユーザーの連絡先の**表示名**と**emailAddresses**プロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="e4261-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="e4261-141">応答</span><span class="sxs-lookup"><span data-stu-id="e4261-141">Response</span></span>
<span data-ttu-id="e4261-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e4261-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
