---
title: EducationAssignment の削除
description: 既存の割り当てを削除します。 割り当てを削除できるのは、クラス内の教師だけです。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39d26a7fdc20ec7a28e89d1186733821f5189850
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436180"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="a7978-104">EducationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="a7978-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7978-105">既存の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="a7978-105">Delete an existing assignment.</span></span> <span data-ttu-id="a7978-106">割り当てを削除できるのは、クラス内の教師だけです。</span><span class="sxs-lookup"><span data-stu-id="a7978-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7978-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7978-107">Permissions</span></span>

<span data-ttu-id="a7978-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7978-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7978-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7978-110">Permission type</span></span>                        | <span data-ttu-id="a7978-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7978-111">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="a7978-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7978-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7978-113">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="a7978-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="a7978-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7978-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7978-115">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="a7978-115">Not Supported.</span></span>                                          |
| <span data-ttu-id="a7978-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7978-116">Application</span></span>                            | <span data-ttu-id="a7978-117">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="a7978-117">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="a7978-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7978-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7978-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7978-119">Request headers</span></span>

| <span data-ttu-id="a7978-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7978-120">Header</span></span>        | <span data-ttu-id="a7978-121">値</span><span class="sxs-lookup"><span data-stu-id="a7978-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="a7978-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7978-122">Authorization</span></span> | <span data-ttu-id="a7978-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a7978-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7978-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7978-125">Request body</span></span>

<span data-ttu-id="a7978-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a7978-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7978-127">応答</span><span class="sxs-lookup"><span data-stu-id="a7978-127">Response</span></span>

<span data-ttu-id="a7978-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="a7978-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7978-130">例</span><span class="sxs-lookup"><span data-stu-id="a7978-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7978-131">要求</span><span class="sxs-lookup"><span data-stu-id="a7978-131">Request</span></span>

<span data-ttu-id="a7978-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a7978-132">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a7978-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a7978-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7978-134">C#</span><span class="sxs-lookup"><span data-stu-id="a7978-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7978-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="a7978-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7978-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="a7978-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a7978-137">応答</span><span class="sxs-lookup"><span data-stu-id="a7978-137">Response</span></span>
<span data-ttu-id="a7978-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a7978-138">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
