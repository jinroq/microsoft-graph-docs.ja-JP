---
title: 'educationSubmission: 提出'
description: 学生が作業を行い、割り当ての準備が整っていることを示すアクション。 このアクションは、受講者のみが実行できます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 55e8704df4374ea7fe42dc8ac7af6f496bc8984e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259501"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="e8bad-104">educationSubmission: 提出</span><span class="sxs-lookup"><span data-stu-id="e8bad-104">educationSubmission: submit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8bad-105">学生が作業を行い、割り当ての準備が整っていることを示すアクション。</span><span class="sxs-lookup"><span data-stu-id="e8bad-105">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="e8bad-106">このアクションは、受講者のみが実行できます。</span><span class="sxs-lookup"><span data-stu-id="e8bad-106">This action can only be taken by the student.</span></span> <span data-ttu-id="e8bad-107">これにより、送信の状態が "作業" から "送信済み" に変更されます。</span><span class="sxs-lookup"><span data-stu-id="e8bad-107">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="e8bad-108">送信プロセス中に、すべてのリソースが submittedResources バケットにコピーされます。</span><span class="sxs-lookup"><span data-stu-id="e8bad-108">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="e8bad-109">教師は、お客様のために送信されたリソースの一覧を調べます。</span><span class="sxs-lookup"><span data-stu-id="e8bad-109">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8bad-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8bad-110">Permissions</span></span>
<span data-ttu-id="e8bad-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8bad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8bad-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8bad-113">Permission type</span></span>      | <span data-ttu-id="e8bad-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8bad-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8bad-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8bad-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="e8bad-116">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="e8bad-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e8bad-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8bad-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e8bad-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8bad-118">Not supported.</span></span>  |
|<span data-ttu-id="e8bad-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8bad-119">Application</span></span> | <span data-ttu-id="e8bad-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8bad-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e8bad-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8bad-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="e8bad-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8bad-122">Request headers</span></span>
| <span data-ttu-id="e8bad-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8bad-123">Header</span></span>       | <span data-ttu-id="e8bad-124">値</span><span class="sxs-lookup"><span data-stu-id="e8bad-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8bad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8bad-125">Authorization</span></span>  | <span data-ttu-id="e8bad-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e8bad-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8bad-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8bad-128">Request body</span></span>
<span data-ttu-id="e8bad-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8bad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8bad-130">応答</span><span class="sxs-lookup"><span data-stu-id="e8bad-130">Response</span></span>
<span data-ttu-id="e8bad-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e8bad-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8bad-133">例</span><span class="sxs-lookup"><span data-stu-id="e8bad-133">Example</span></span>
<span data-ttu-id="e8bad-134">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e8bad-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e8bad-135">要求</span><span class="sxs-lookup"><span data-stu-id="e8bad-135">Request</span></span>
<span data-ttu-id="e8bad-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8bad-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="e8bad-137">応答</span><span class="sxs-lookup"><span data-stu-id="e8bad-137">Response</span></span>
<span data-ttu-id="e8bad-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8bad-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8bad-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e8bad-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8bad-140">C#</span><span class="sxs-lookup"><span data-stu-id="e8bad-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/educationsubmission_submit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8bad-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="e8bad-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/educationsubmission_submit-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e8bad-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="e8bad-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/educationsubmission_submit-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-submit.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsubmission-submit.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmission-submit.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
