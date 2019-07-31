---
title: プログラムの削除
description: Azure AD access レビュー機能で、プログラムオブジェクトを削除します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0db7db7c33ea7c173e4d14b975baa84b612dc471
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978597"
---
# <a name="delete-program"></a><span data-ttu-id="76b72-103">プログラムの削除</span><span class="sxs-lookup"><span data-stu-id="76b72-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76b72-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、[プログラム](../resources/program.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="76b72-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="76b72-105">まだ`programControl`リンクされているプログラムを削除しないでください。これらのアクセスレビューは、最初にプログラムから削除するか、別のプログラムにリンクする必要があります。</span><span class="sxs-lookup"><span data-stu-id="76b72-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="76b72-106">また、組み込みの既定のプログラムは削除できないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="76b72-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="76b72-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="76b72-107">Permissions</span></span>
<span data-ttu-id="76b72-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76b72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76b72-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76b72-110">Permission type</span></span>                        | <span data-ttu-id="76b72-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="76b72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="76b72-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76b72-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="76b72-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b72-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="76b72-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76b72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76b72-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76b72-115">Not supported.</span></span> |
|<span data-ttu-id="76b72-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76b72-116">Application</span></span>                            | <span data-ttu-id="76b72-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76b72-117">Not supported.</span></span> |

<span data-ttu-id="76b72-118">サインインしているユーザーは、プログラムを作成することを許可するディレクトリロールにある必要があります。</span><span class="sxs-lookup"><span data-stu-id="76b72-118">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="76b72-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76b72-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="76b72-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76b72-120">Request headers</span></span>
| <span data-ttu-id="76b72-121">名前</span><span class="sxs-lookup"><span data-stu-id="76b72-121">Name</span></span>         | <span data-ttu-id="76b72-122">型</span><span class="sxs-lookup"><span data-stu-id="76b72-122">Type</span></span>        | <span data-ttu-id="76b72-123">説明</span><span class="sxs-lookup"><span data-stu-id="76b72-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="76b72-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="76b72-124">Authorization</span></span> | <span data-ttu-id="76b72-125">string</span><span class="sxs-lookup"><span data-stu-id="76b72-125">string</span></span> | <span data-ttu-id="76b72-p103">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="76b72-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76b72-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="76b72-128">Request body</span></span>
<span data-ttu-id="76b72-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="76b72-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="76b72-130">応答</span><span class="sxs-lookup"><span data-stu-id="76b72-130">Response</span></span>
<span data-ttu-id="76b72-p104">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="76b72-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76b72-133">例</span><span class="sxs-lookup"><span data-stu-id="76b72-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76b72-134">要求</span><span class="sxs-lookup"><span data-stu-id="76b72-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76b72-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="76b72-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76b72-136">C#</span><span class="sxs-lookup"><span data-stu-id="76b72-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76b72-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="76b72-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76b72-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="76b72-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="76b72-139">Java</span><span class="sxs-lookup"><span data-stu-id="76b72-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="76b72-140">応答</span><span class="sxs-lookup"><span data-stu-id="76b72-140">Response</span></span>
><span data-ttu-id="76b72-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="76b72-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
