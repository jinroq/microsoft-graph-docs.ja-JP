---
title: 連絡先を一覧表示する
description: サインインしているユーザーのメールボックス内のすべての連絡先を取得する (. ../me/contacts) か、指定した連絡先フォルダーから取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 230fa87233dfb5bfc2fc22cf2d64a4f6131b1ef0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35943247"
---
# <a name="list-contacts"></a><span data-ttu-id="36090-103">連絡先を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="36090-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36090-104">サインインしているユーザーのメールボックス内のすべての連絡先を取得する (. ../me/contacts) か、指定した連絡先フォルダーから取得します。</span><span class="sxs-lookup"><span data-stu-id="36090-104">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="36090-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36090-105">Permissions</span></span>
<span data-ttu-id="36090-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36090-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36090-108">Permission type</span></span>      | <span data-ttu-id="36090-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36090-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36090-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36090-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36090-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36090-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="36090-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36090-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36090-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36090-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="36090-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36090-114">Application</span></span> | <span data-ttu-id="36090-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36090-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="36090-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36090-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36090-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="36090-117">Optional query parameters</span></span>
<span data-ttu-id="36090-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="36090-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="36090-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36090-119">Request headers</span></span>
| <span data-ttu-id="36090-120">名前</span><span class="sxs-lookup"><span data-stu-id="36090-120">Name</span></span>       | <span data-ttu-id="36090-121">型</span><span class="sxs-lookup"><span data-stu-id="36090-121">Type</span></span> | <span data-ttu-id="36090-122">説明</span><span class="sxs-lookup"><span data-stu-id="36090-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="36090-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="36090-123">Authorization</span></span>  | <span data-ttu-id="36090-124">string</span><span class="sxs-lookup"><span data-stu-id="36090-124">string</span></span>  | <span data-ttu-id="36090-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36090-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36090-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="36090-127">Request body</span></span>
<span data-ttu-id="36090-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="36090-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36090-129">応答</span><span class="sxs-lookup"><span data-stu-id="36090-129">Response</span></span>

<span data-ttu-id="36090-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Contact](../resources/contact.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="36090-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36090-131">例</span><span class="sxs-lookup"><span data-stu-id="36090-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36090-132">要求</span><span class="sxs-lookup"><span data-stu-id="36090-132">Request</span></span>
<span data-ttu-id="36090-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36090-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36090-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="36090-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36090-135">C#</span><span class="sxs-lookup"><span data-stu-id="36090-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-contacts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36090-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="36090-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-contacts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36090-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="36090-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-contacts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36090-138">Java</span><span class="sxs-lookup"><span data-stu-id="36090-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-contacts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36090-139">応答</span><span class="sxs-lookup"><span data-stu-id="36090-139">Response</span></span>
<span data-ttu-id="36090-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36090-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "birthday": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
