---
title: Outlook カテゴリを削除する
description: 指定した outlookCategory オブジェクトを削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d22fb1df275264536b5e18d4749645cc27f5f1cc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414204"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="18634-103">Outlook カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="18634-103">Delete Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18634-104">指定した [outlookCategory](../resources/outlookcategory.md) オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="18634-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18634-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18634-105">Permissions</span></span>
<span data-ttu-id="18634-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18634-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18634-108">Permission type</span></span>      | <span data-ttu-id="18634-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18634-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18634-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18634-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18634-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18634-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="18634-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18634-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18634-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18634-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="18634-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18634-114">Application</span></span> | <span data-ttu-id="18634-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18634-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="18634-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18634-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="18634-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18634-117">Request headers</span></span>
| <span data-ttu-id="18634-118">名前</span><span class="sxs-lookup"><span data-stu-id="18634-118">Name</span></span>      |<span data-ttu-id="18634-119">説明</span><span class="sxs-lookup"><span data-stu-id="18634-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="18634-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="18634-120">Authorization</span></span>  | <span data-ttu-id="18634-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18634-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18634-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="18634-123">Request body</span></span>
<span data-ttu-id="18634-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="18634-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18634-125">応答</span><span class="sxs-lookup"><span data-stu-id="18634-125">Response</span></span>

<span data-ttu-id="18634-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="18634-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18634-128">例</span><span class="sxs-lookup"><span data-stu-id="18634-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18634-129">要求</span><span class="sxs-lookup"><span data-stu-id="18634-129">Request</span></span>
<span data-ttu-id="18634-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18634-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18634-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="18634-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="18634-132">C#</span><span class="sxs-lookup"><span data-stu-id="18634-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18634-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18634-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18634-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="18634-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="18634-135">応答</span><span class="sxs-lookup"><span data-stu-id="18634-135">Response</span></span>
<span data-ttu-id="18634-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="18634-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
