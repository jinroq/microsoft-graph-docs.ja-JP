---
title: 'educationSubmission: unsubmit'
description: . 送信中に、すべてのリソースからコピーされます submittedResources workingResources バケットにします。 先生はグレーディングの作業中のリソースの一覧を見ています。
ms.openlocfilehash: 610b5a69a06c29d2e2b9b1fa6eb501a56d59b076
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067337"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="33b6d-105">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="33b6d-105">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="33b6d-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33b6d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33b6d-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33b6d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="33b6d-108">アクション起動された後、割り当ての送信時に、受講生受講者が要求していることを示します。</span><span class="sxs-lookup"><span data-stu-id="33b6d-108">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="33b6d-109">この操作は、受講者のみ取得できます。</span><span class="sxs-lookup"><span data-stu-id="33b6d-109">This action can only be taken by the student.</span></span> <span data-ttu-id="33b6d-110">「送信」からの提出書類のステータスを変更すると、「処理中」にこのされます。</span><span class="sxs-lookup"><span data-stu-id="33b6d-110">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="33b6d-111">送信中に、すべてのリソースからコピーされます submittedResources workingResources バケットにします。</span><span class="sxs-lookup"><span data-stu-id="33b6d-111">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="33b6d-112">先生はグレーディングの作業中のリソースの一覧を見ています。</span><span class="sxs-lookup"><span data-stu-id="33b6d-112">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="33b6d-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33b6d-113">Permissions</span></span>
<span data-ttu-id="33b6d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33b6d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33b6d-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33b6d-116">Permission type</span></span>      | <span data-ttu-id="33b6d-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="33b6d-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33b6d-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33b6d-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="33b6d-119">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33b6d-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="33b6d-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33b6d-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="33b6d-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33b6d-121">Not supported.</span></span>  |
|<span data-ttu-id="33b6d-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33b6d-122">Application</span></span> | <span data-ttu-id="33b6d-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33b6d-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="33b6d-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33b6d-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="33b6d-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33b6d-125">Request headers</span></span>
| <span data-ttu-id="33b6d-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33b6d-126">Header</span></span>       | <span data-ttu-id="33b6d-127">値</span><span class="sxs-lookup"><span data-stu-id="33b6d-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="33b6d-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="33b6d-128">Authorization</span></span>  | <span data-ttu-id="33b6d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33b6d-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33b6d-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="33b6d-131">Request body</span></span>
<span data-ttu-id="33b6d-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="33b6d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33b6d-133">応答</span><span class="sxs-lookup"><span data-stu-id="33b6d-133">Response</span></span>
<span data-ttu-id="33b6d-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="33b6d-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b6d-136">例</span><span class="sxs-lookup"><span data-stu-id="33b6d-136">Example</span></span>
<span data-ttu-id="33b6d-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="33b6d-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33b6d-138">要求</span><span class="sxs-lookup"><span data-stu-id="33b6d-138">Request</span></span>
<span data-ttu-id="33b6d-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33b6d-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="33b6d-140">応答</span><span class="sxs-lookup"><span data-stu-id="33b6d-140">Response</span></span>
<span data-ttu-id="33b6d-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33b6d-141">The following is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
