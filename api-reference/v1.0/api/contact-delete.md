---
title: 連絡先を削除する
description: 連絡先を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e483fd624baf0ec0f534b7435737fb59e6fc10f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003281"
---
# <a name="delete-contact"></a><span data-ttu-id="9a074-103">連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="9a074-103">Delete contact</span></span>

<span data-ttu-id="9a074-104">連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="9a074-104">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a074-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a074-105">Permissions</span></span>
<span data-ttu-id="9a074-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a074-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a074-108">Permission type</span></span>      | <span data-ttu-id="9a074-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a074-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a074-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a074-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a074-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a074-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9a074-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a074-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a074-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a074-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9a074-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a074-114">Application</span></span> | <span data-ttu-id="9a074-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a074-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a074-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a074-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9a074-117">ユーザーの既定 [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="9a074-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="9a074-118">ユーザーの最上位レベル [contactFolder](../resources/contactfolder.md) からの [連絡先](../resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="9a074-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="9a074-p102">[contactFolder](../resources/mailfolder.md) の子フォルダー内に含まれる [連絡先](../resources/contact.md)。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="9a074-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9a074-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a074-121">Request headers</span></span>
| <span data-ttu-id="9a074-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a074-122">Header</span></span>       | <span data-ttu-id="9a074-123">値</span><span class="sxs-lookup"><span data-stu-id="9a074-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a074-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a074-124">Authorization</span></span>  | <span data-ttu-id="9a074-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a074-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a074-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a074-127">Request body</span></span>
<span data-ttu-id="9a074-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9a074-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a074-129">応答</span><span class="sxs-lookup"><span data-stu-id="9a074-129">Response</span></span>

<span data-ttu-id="9a074-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="9a074-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a074-132">例</span><span class="sxs-lookup"><span data-stu-id="9a074-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a074-133">要求</span><span class="sxs-lookup"><span data-stu-id="9a074-133">Request</span></span>
<span data-ttu-id="9a074-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9a074-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a074-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9a074-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a074-136">C#</span><span class="sxs-lookup"><span data-stu-id="9a074-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a074-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a074-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a074-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="9a074-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9a074-139">Java</span><span class="sxs-lookup"><span data-stu-id="9a074-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a074-140">応答</span><span class="sxs-lookup"><span data-stu-id="9a074-140">Response</span></span>
<span data-ttu-id="9a074-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9a074-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
