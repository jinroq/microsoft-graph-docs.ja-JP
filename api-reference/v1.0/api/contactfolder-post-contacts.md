---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fafc6759f89c219e2d4fcbf6c32b4589bf25543b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443029"
---
# <a name="create-contact"></a><span data-ttu-id="1344a-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="1344a-103">Create contact</span></span>

<span data-ttu-id="1344a-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="1344a-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1344a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1344a-105">Permissions</span></span>

<span data-ttu-id="1344a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1344a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1344a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1344a-108">Permission type</span></span>      | <span data-ttu-id="1344a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1344a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1344a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1344a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1344a-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1344a-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1344a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1344a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1344a-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1344a-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="1344a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1344a-114">Application</span></span> | <span data-ttu-id="1344a-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1344a-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1344a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1344a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="1344a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1344a-117">Request headers</span></span>

| <span data-ttu-id="1344a-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1344a-118">Header</span></span>       | <span data-ttu-id="1344a-119">値</span><span class="sxs-lookup"><span data-stu-id="1344a-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1344a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1344a-120">Authorization</span></span>  | <span data-ttu-id="1344a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1344a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1344a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1344a-123">Content-Type</span></span>  | <span data-ttu-id="1344a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1344a-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1344a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1344a-126">Request body</span></span>
<span data-ttu-id="1344a-127">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1344a-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1344a-128">応答</span><span class="sxs-lookup"><span data-stu-id="1344a-128">Response</span></span>

<span data-ttu-id="1344a-129">成功した場合、このメソッドは `201 Created` 応答コードと[連絡先](../resources/contact.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="1344a-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1344a-130">例</span><span class="sxs-lookup"><span data-stu-id="1344a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1344a-131">要求</span><span class="sxs-lookup"><span data-stu-id="1344a-131">Request</span></span>

<span data-ttu-id="1344a-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1344a-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1344a-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1344a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1344a-134">C#</span><span class="sxs-lookup"><span data-stu-id="1344a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1344a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1344a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1344a-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="1344a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

<span data-ttu-id="1344a-137">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1344a-137">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="1344a-138">応答</span><span class="sxs-lookup"><span data-stu-id="1344a-138">Response</span></span>

<span data-ttu-id="1344a-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1344a-139">Here is an example of the response.</span></span> <span data-ttu-id="1344a-140">**注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="1344a-140">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1344a-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1344a-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
