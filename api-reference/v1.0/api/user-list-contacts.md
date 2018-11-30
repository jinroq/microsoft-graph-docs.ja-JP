---
title: 連絡先を一覧表示する
description: サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得します。
ms.openlocfilehash: 296844eb4eea93c5bd46e8028f3423fe797142ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022404"
---
# <a name="list-contacts"></a><span data-ttu-id="0db95-103">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0db95-103">List contacts</span></span>

<span data-ttu-id="0db95-104">サインイン中のユーザーの既定の連絡先フォルダーから連絡先のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0db95-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="0db95-105">アプリケーションが別のユーザーの連絡先フォルダーに連絡先を入手するための 2 つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="0db95-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="0db95-106">アプリケーションは、アプリケーションの権限を持つ場合、または、</span><span class="sxs-lookup"><span data-stu-id="0db95-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="0db95-107">アプリケーションがある場合、適切な 1 人のユーザーから[アクセス許可](#permissions)を委任し、他のユーザーは、そのユーザーの連絡先フォルダーを共有するにはまたは、そのユーザーに代理アクセスを与え。</span><span class="sxs-lookup"><span data-stu-id="0db95-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="0db95-108">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0db95-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="0db95-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0db95-109">Permissions</span></span>
<span data-ttu-id="0db95-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0db95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0db95-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0db95-112">Permission type</span></span>      | <span data-ttu-id="0db95-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0db95-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0db95-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0db95-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0db95-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0db95-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0db95-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0db95-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0db95-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0db95-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0db95-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0db95-118">Application</span></span> | <span data-ttu-id="0db95-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0db95-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0db95-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0db95-120">HTTP request</span></span>

<span data-ttu-id="0db95-121">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="0db95-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="0db95-122">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="0db95-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0db95-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0db95-123">Optional query parameters</span></span>
<span data-ttu-id="0db95-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0db95-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="0db95-125">たとえば、`$filter` クエリ パラメーターを使って、メール アドレスのドメインに基づいて連絡先をフィルターすることができます。</span><span class="sxs-lookup"><span data-stu-id="0db95-125">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="0db95-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0db95-126">Request headers</span></span>
| <span data-ttu-id="0db95-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0db95-127">Header</span></span>       | <span data-ttu-id="0db95-128">値</span><span class="sxs-lookup"><span data-stu-id="0db95-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0db95-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="0db95-129">Authorization</span></span>  | <span data-ttu-id="0db95-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0db95-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0db95-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0db95-132">Content-Type</span></span>   | <span data-ttu-id="0db95-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0db95-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0db95-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="0db95-134">Request body</span></span>
<span data-ttu-id="0db95-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0db95-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0db95-136">応答</span><span class="sxs-lookup"><span data-stu-id="0db95-136">Response</span></span>

<span data-ttu-id="0db95-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0db95-137">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0db95-138">例</span><span class="sxs-lookup"><span data-stu-id="0db95-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0db95-139">要求</span><span class="sxs-lookup"><span data-stu-id="0db95-139">Request</span></span>
<span data-ttu-id="0db95-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0db95-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="0db95-141">応答</span><span class="sxs-lookup"><span data-stu-id="0db95-141">Response</span></span>
<span data-ttu-id="0db95-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0db95-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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