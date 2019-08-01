---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 85ec6d704402e1596a5376ed76fea155e61f4fe2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003127"
---
# <a name="create-contact"></a><span data-ttu-id="8af2e-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="8af2e-103">Create contact</span></span>

<span data-ttu-id="8af2e-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="8af2e-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="8af2e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8af2e-105">Permissions</span></span>

<span data-ttu-id="8af2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8af2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8af2e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8af2e-108">Permission type</span></span>      | <span data-ttu-id="8af2e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8af2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8af2e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8af2e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8af2e-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8af2e-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8af2e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8af2e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8af2e-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8af2e-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8af2e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8af2e-114">Application</span></span> | <span data-ttu-id="8af2e-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8af2e-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8af2e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8af2e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="8af2e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8af2e-117">Request headers</span></span>

| <span data-ttu-id="8af2e-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8af2e-118">Header</span></span>       | <span data-ttu-id="8af2e-119">値</span><span class="sxs-lookup"><span data-stu-id="8af2e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8af2e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8af2e-120">Authorization</span></span>  | <span data-ttu-id="8af2e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8af2e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8af2e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8af2e-123">Content-Type</span></span>  | <span data-ttu-id="8af2e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8af2e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8af2e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8af2e-126">Request body</span></span>
<span data-ttu-id="8af2e-127">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8af2e-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8af2e-128">応答</span><span class="sxs-lookup"><span data-stu-id="8af2e-128">Response</span></span>

<span data-ttu-id="8af2e-129">成功した場合、このメソッドは `201 Created` 応答コードと[連絡先](../resources/contact.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="8af2e-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8af2e-130">例</span><span class="sxs-lookup"><span data-stu-id="8af2e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8af2e-131">要求</span><span class="sxs-lookup"><span data-stu-id="8af2e-131">Request</span></span>

<span data-ttu-id="8af2e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8af2e-132">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8af2e-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8af2e-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8af2e-134">C#</span><span class="sxs-lookup"><span data-stu-id="8af2e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8af2e-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="8af2e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8af2e-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="8af2e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8af2e-137">Java</span><span class="sxs-lookup"><span data-stu-id="8af2e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contact-from-contactfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<br/>

<span data-ttu-id="8af2e-138">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8af2e-138">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="8af2e-139">応答</span><span class="sxs-lookup"><span data-stu-id="8af2e-139">Response</span></span>

<span data-ttu-id="8af2e-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="8af2e-140">Here is an example of the response.</span></span> <span data-ttu-id="8af2e-141">**注:** 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="8af2e-141">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8af2e-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8af2e-142">All the properties will be returned from an actual call.</span></span>

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
