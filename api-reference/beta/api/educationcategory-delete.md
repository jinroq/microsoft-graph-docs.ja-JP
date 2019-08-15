---
title: EducationCategory の削除
description: 既存のカテゴリを削除します。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8443ab8de0afda3eb7c014946973f180b94d14eb
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416472"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="e3f18-103">EducationCategory の削除</span><span class="sxs-lookup"><span data-stu-id="e3f18-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3f18-104">既存のカテゴリを削除します。</span><span class="sxs-lookup"><span data-stu-id="e3f18-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3f18-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e3f18-105">Permissions</span></span>

<span data-ttu-id="e3f18-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3f18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3f18-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3f18-108">Permission type</span></span>                        | <span data-ttu-id="e3f18-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3f18-109">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="e3f18-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3f18-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3f18-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="e3f18-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="e3f18-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3f18-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3f18-113">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="e3f18-113">Not Supported.</span></span>                                          |
| <span data-ttu-id="e3f18-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3f18-114">Application</span></span>                            | <span data-ttu-id="e3f18-115">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="e3f18-115">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="e3f18-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3f18-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e3f18-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3f18-117">Request headers</span></span>

| <span data-ttu-id="e3f18-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3f18-118">Header</span></span>        | <span data-ttu-id="e3f18-119">値</span><span class="sxs-lookup"><span data-stu-id="e3f18-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e3f18-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3f18-120">Authorization</span></span> | <span data-ttu-id="e3f18-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e3f18-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3f18-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3f18-123">Request body</span></span>

<span data-ttu-id="e3f18-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e3f18-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3f18-125">応答</span><span class="sxs-lookup"><span data-stu-id="e3f18-125">Response</span></span>

<span data-ttu-id="e3f18-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e3f18-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3f18-128">例</span><span class="sxs-lookup"><span data-stu-id="e3f18-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3f18-129">要求</span><span class="sxs-lookup"><span data-stu-id="e3f18-129">Request</span></span>

<span data-ttu-id="e3f18-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3f18-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e3f18-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e3f18-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3f18-132">C#</span><span class="sxs-lookup"><span data-stu-id="e3f18-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3f18-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3f18-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3f18-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="e3f18-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e3f18-135">応答</span><span class="sxs-lookup"><span data-stu-id="e3f18-135">Response</span></span>

<span data-ttu-id="e3f18-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e3f18-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
