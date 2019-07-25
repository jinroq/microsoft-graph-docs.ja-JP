---
title: EducationAssignmentResource の削除
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e0ee9fd708c0837ca23473e8509f184645fa52fa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860737"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="18625-103">EducationAssignmentResource の削除</span><span class="sxs-lookup"><span data-stu-id="18625-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18625-104">割り当てからリソースを削除します。</span><span class="sxs-lookup"><span data-stu-id="18625-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="18625-105">クラス内の教師のみがリソースを削除できます。</span><span class="sxs-lookup"><span data-stu-id="18625-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="18625-106">学生に対して割り当てを発行した後は、教師は "distributeToStudents" とマークされているリソースを削除できません。</span><span class="sxs-lookup"><span data-stu-id="18625-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="18625-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18625-107">Permissions</span></span>
<span data-ttu-id="18625-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18625-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18625-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18625-110">Permission type</span></span>      | <span data-ttu-id="18625-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18625-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18625-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18625-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="18625-113">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="18625-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="18625-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18625-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="18625-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18625-115">Not supported.</span></span>  |
|<span data-ttu-id="18625-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18625-116">Application</span></span> | <span data-ttu-id="18625-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18625-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="18625-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18625-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="18625-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18625-119">Request headers</span></span>
| <span data-ttu-id="18625-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18625-120">Header</span></span>       | <span data-ttu-id="18625-121">値</span><span class="sxs-lookup"><span data-stu-id="18625-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18625-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="18625-122">Authorization</span></span>  | <span data-ttu-id="18625-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="18625-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18625-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="18625-125">Request body</span></span>
<span data-ttu-id="18625-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="18625-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="18625-127">応答</span><span class="sxs-lookup"><span data-stu-id="18625-127">Response</span></span>
<span data-ttu-id="18625-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="18625-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18625-130">例</span><span class="sxs-lookup"><span data-stu-id="18625-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18625-131">要求</span><span class="sxs-lookup"><span data-stu-id="18625-131">Request</span></span>
<span data-ttu-id="18625-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="18625-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="18625-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="18625-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="18625-134">C#</span><span class="sxs-lookup"><span data-stu-id="18625-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18625-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="18625-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="18625-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="18625-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="18625-137">Java</span><span class="sxs-lookup"><span data-stu-id="18625-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="18625-138">応答</span><span class="sxs-lookup"><span data-stu-id="18625-138">Response</span></span>
<span data-ttu-id="18625-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="18625-139">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
