---
title: 連絡先を一覧表示する
description: サインイン中のユーザーの既定の連絡先フォルダー内の連絡先フォルダーのコレクションを取得します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a3532aac45ed2fcabadb2430b032f4bb3d7c9d9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026965"
---
# <a name="list-contacts"></a><span data-ttu-id="bf4ad-103">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bf4ad-103">List contacts</span></span>

<span data-ttu-id="bf4ad-104">サインイン中のユーザーの既定の連絡先フォルダー内の連絡先フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="bf4ad-105">アプリが別のユーザーの連絡先フォルダーから連絡先を取得できるシナリオは2つあります。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="bf4ad-106">アプリにアプリケーションのアクセス許可がある場合。または</span><span class="sxs-lookup"><span data-stu-id="bf4ad-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="bf4ad-107">アプリに「あるユーザーから適切に委任された[アクセス許可](#permissions)」があり、別のユーザーがそのユーザーとコンタクトフォルダーを共有しているか、そのユーザーに委任されたアクセスを付与している場合。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="bf4ad-108">[詳細と例](/graph/outlook-get-shared-contacts-folders)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="bf4ad-109">権限</span><span class="sxs-lookup"><span data-stu-id="bf4ad-109">Permissions</span></span>
<span data-ttu-id="bf4ad-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf4ad-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bf4ad-112">Permission type</span></span>      | <span data-ttu-id="bf4ad-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bf4ad-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf4ad-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bf4ad-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bf4ad-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf4ad-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bf4ad-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf4ad-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf4ad-117">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf4ad-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bf4ad-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bf4ad-118">Application</span></span> | <span data-ttu-id="bf4ad-119">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf4ad-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf4ad-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf4ad-120">HTTP request</span></span>

<span data-ttu-id="bf4ad-121">ユーザーのメールボックス内のすべての連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="bf4ad-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="bf4ad-122">ユーザーのメールボックス内の特定のフォルダーにある連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="bf4ad-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bf4ad-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bf4ad-123">Optional query parameters</span></span>
<span data-ttu-id="bf4ad-124">たとえば、`$filter` クエリ パラメーターを使って、メール アドレスに基づいて連絡先をフィルターすることができます。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="bf4ad-125">`$filter`、`any`そして`eq`演算子を使用できるのは**emailAddresses**コレクションの**address**サブプロパティのみなので注意が必要です 。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="bf4ad-126">すなわち、**氏名** または**emailAddresses**の 1 つのインスタンスの他のサブ プロパティでフィルター抽出することはできませんし、`filter` 以下のような `ne`, `le`や `startswith()`その他の演算子や関数を適用したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="bf4ad-127">`$filter`クエリのパラメーターの一般的な情報については、[OData クエリ パラメーター](/graph/query-parameters)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="bf4ad-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf4ad-128">Request headers</span></span>
| <span data-ttu-id="bf4ad-129">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf4ad-129">Header</span></span>       | <span data-ttu-id="bf4ad-130">値</span><span class="sxs-lookup"><span data-stu-id="bf4ad-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf4ad-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf4ad-131">Authorization</span></span>  | <span data-ttu-id="bf4ad-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf4ad-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf4ad-134">Content-Type</span></span>   | <span data-ttu-id="bf4ad-135">application/json</span><span class="sxs-lookup"><span data-stu-id="bf4ad-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf4ad-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="bf4ad-136">Request body</span></span>
<span data-ttu-id="bf4ad-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf4ad-138">応答</span><span class="sxs-lookup"><span data-stu-id="bf4ad-138">Response</span></span>

<span data-ttu-id="bf4ad-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-139">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bf4ad-140">例</span><span class="sxs-lookup"><span data-stu-id="bf4ad-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf4ad-141">要求</span><span class="sxs-lookup"><span data-stu-id="bf4ad-141">Request</span></span>
<span data-ttu-id="bf4ad-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bf4ad-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="bf4ad-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bf4ad-144">C#</span><span class="sxs-lookup"><span data-stu-id="bf4ad-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf4ad-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="bf4ad-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bf4ad-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bf4ad-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bf4ad-147">Java</span><span class="sxs-lookup"><span data-stu-id="bf4ad-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="bf4ad-148">応答</span><span class="sxs-lookup"><span data-stu-id="bf4ad-148">Response</span></span>
<span data-ttu-id="bf4ad-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bf4ad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
