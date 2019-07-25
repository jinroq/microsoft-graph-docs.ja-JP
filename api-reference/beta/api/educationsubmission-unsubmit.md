---
title: 'educationSubmission: 未送信'
description: '学生が、入力された後に割り当ての提出を作業したいと指定するアクション。 このアクションは、受講者のみが実行できます。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b5ef81d78d0228dbb101d3d7490efc0fe3f4301e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860287"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="e7998-104">educationSubmission: 未送信</span><span class="sxs-lookup"><span data-stu-id="e7998-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7998-105">学生が、入力された後に割り当ての提出を作業したいと指定するアクション。</span><span class="sxs-lookup"><span data-stu-id="e7998-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="e7998-106">このアクションは、受講者のみが実行できます。</span><span class="sxs-lookup"><span data-stu-id="e7998-106">This action can only be taken by the student.</span></span> <span data-ttu-id="e7998-107">これにより、送信の状態が "送信済み" から "作業" に変更されます。</span><span class="sxs-lookup"><span data-stu-id="e7998-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="e7998-108">送信プロセス中に、すべてのリソースが submittedResources から workingResources バケットにコピーされます。</span><span class="sxs-lookup"><span data-stu-id="e7998-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="e7998-109">教師は、[作業中のリソース] リストを調べて、注目を求めます。</span><span class="sxs-lookup"><span data-stu-id="e7998-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7998-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7998-110">Permissions</span></span>
<span data-ttu-id="e7998-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7998-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7998-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7998-113">Permission type</span></span>      | <span data-ttu-id="e7998-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7998-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7998-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7998-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="e7998-116">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="e7998-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e7998-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7998-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e7998-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7998-118">Not supported.</span></span>  |
|<span data-ttu-id="e7998-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7998-119">Application</span></span> | <span data-ttu-id="e7998-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7998-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e7998-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7998-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="e7998-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7998-122">Request headers</span></span>
| <span data-ttu-id="e7998-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7998-123">Header</span></span>       | <span data-ttu-id="e7998-124">値</span><span class="sxs-lookup"><span data-stu-id="e7998-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e7998-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7998-125">Authorization</span></span>  | <span data-ttu-id="e7998-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7998-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e7998-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7998-128">Request body</span></span>
<span data-ttu-id="e7998-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7998-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7998-130">応答</span><span class="sxs-lookup"><span data-stu-id="e7998-130">Response</span></span>
<span data-ttu-id="e7998-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e7998-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7998-133">例</span><span class="sxs-lookup"><span data-stu-id="e7998-133">Example</span></span>
<span data-ttu-id="e7998-134">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e7998-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e7998-135">要求</span><span class="sxs-lookup"><span data-stu-id="e7998-135">Request</span></span>
<span data-ttu-id="e7998-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7998-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e7998-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e7998-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7998-138">C#</span><span class="sxs-lookup"><span data-stu-id="e7998-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7998-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7998-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7998-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="e7998-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e7998-141">Java</span><span class="sxs-lookup"><span data-stu-id="e7998-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e7998-142">応答</span><span class="sxs-lookup"><span data-stu-id="e7998-142">Response</span></span>
<span data-ttu-id="e7998-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7998-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
