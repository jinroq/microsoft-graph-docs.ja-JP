---
title: 連絡先を作成する
description: 連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e61bfe311028fd303faa0dfbc71dcd6471879b9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417957"
---
# <a name="create-contact"></a><span data-ttu-id="92202-103">連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="92202-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92202-104">連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの `contacts` エンドポイントに追加します。</span><span class="sxs-lookup"><span data-stu-id="92202-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="92202-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="92202-105">Permissions</span></span>
<span data-ttu-id="92202-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92202-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92202-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92202-108">Permission type</span></span>      | <span data-ttu-id="92202-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="92202-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92202-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92202-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92202-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92202-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="92202-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92202-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92202-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92202-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="92202-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92202-114">Application</span></span> | <span data-ttu-id="92202-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92202-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="92202-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92202-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="92202-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92202-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="92202-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92202-118">Request headers</span></span>
| <span data-ttu-id="92202-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92202-119">Header</span></span>       | <span data-ttu-id="92202-120">値</span><span class="sxs-lookup"><span data-stu-id="92202-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92202-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="92202-121">Authorization</span></span>  | <span data-ttu-id="92202-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="92202-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="92202-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92202-124">Content-Type</span></span>  | <span data-ttu-id="92202-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="92202-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92202-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="92202-127">Request body</span></span>
<span data-ttu-id="92202-128">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="92202-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="92202-129">応答</span><span class="sxs-lookup"><span data-stu-id="92202-129">Response</span></span>

<span data-ttu-id="92202-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で[連絡先](../resources/contact.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="92202-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92202-131">例</span><span class="sxs-lookup"><span data-stu-id="92202-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92202-132">要求</span><span class="sxs-lookup"><span data-stu-id="92202-132">Request</span></span>
<span data-ttu-id="92202-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92202-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="92202-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="92202-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92202-135">C#</span><span class="sxs-lookup"><span data-stu-id="92202-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contact-from-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92202-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92202-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contact-from-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92202-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="92202-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contact-from-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="92202-138">要求本文で、[連絡先](../resources/contact.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="92202-138">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="92202-139">応答</span><span class="sxs-lookup"><span data-stu-id="92202-139">Response</span></span>
<span data-ttu-id="92202-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92202-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
