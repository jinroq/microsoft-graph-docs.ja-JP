---
title: 連絡先を一覧表示する
description: サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3f0f7fd86987e3d2923d8ea81a8ca7fbf87900b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984137"
---
# <a name="list-contacts"></a><span data-ttu-id="8d166-103">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8d166-103">List contacts</span></span>

<span data-ttu-id="8d166-104">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8d166-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="8d166-105">アプリケーションが別のユーザーの連絡先フォルダーに連絡先を入手するための 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="8d166-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="8d166-106">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="8d166-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="8d166-107">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーの連絡先フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="8d166-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="8d166-108">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d166-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="8d166-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8d166-109">Permissions</span></span>
<span data-ttu-id="8d166-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d166-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d166-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d166-112">Permission type</span></span>      | <span data-ttu-id="8d166-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d166-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d166-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d166-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8d166-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d166-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8d166-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d166-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d166-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d166-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8d166-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d166-118">Application</span></span> | <span data-ttu-id="8d166-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d166-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d166-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d166-120">HTTP request</span></span>

<span data-ttu-id="8d166-121">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="8d166-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="8d166-122">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="8d166-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d166-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8d166-123">Optional query parameters</span></span>
<span data-ttu-id="8d166-124">使用することができます、`$filter`の電子メール アドレスに基づいて、連絡先をフィルターするクエリのパラメーター。</span><span class="sxs-lookup"><span data-stu-id="8d166-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="8d166-125">注使用することができます`$filter`、`any`と`eq`演算子、 **emailAddresses**コレクション内のインスタンスの**アドレス**サブ プロパティのみにします。</span><span class="sxs-lookup"><span data-stu-id="8d166-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="8d166-126">**名前**または他のサブの**emailAddresses**インスタンスのプロパティにフィルターを適用することはできずするその他の演算子を適用したり、機能を持つ`filter`、次のように`ne`、`le`と`startswith()`。</span><span class="sxs-lookup"><span data-stu-id="8d166-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="8d166-127">全般については、`$filter`クエリのパラメーターで、 [OData クエリのパラメーター](/graph/query-parameters)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d166-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="8d166-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d166-128">Request headers</span></span>
| <span data-ttu-id="8d166-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d166-129">Header</span></span>       | <span data-ttu-id="8d166-130">値</span><span class="sxs-lookup"><span data-stu-id="8d166-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d166-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d166-131">Authorization</span></span>  | <span data-ttu-id="8d166-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8d166-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8d166-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d166-134">Content-Type</span></span>   | <span data-ttu-id="8d166-135">application/json</span><span class="sxs-lookup"><span data-stu-id="8d166-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d166-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d166-136">Request body</span></span>
<span data-ttu-id="8d166-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8d166-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d166-138">応答</span><span class="sxs-lookup"><span data-stu-id="8d166-138">Response</span></span>

<span data-ttu-id="8d166-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8d166-139">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d166-140">例</span><span class="sxs-lookup"><span data-stu-id="8d166-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d166-141">要求</span><span class="sxs-lookup"><span data-stu-id="8d166-141">Request</span></span>
<span data-ttu-id="8d166-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d166-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="8d166-143">応答</span><span class="sxs-lookup"><span data-stu-id="8d166-143">Response</span></span>
<span data-ttu-id="8d166-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d166-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
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
