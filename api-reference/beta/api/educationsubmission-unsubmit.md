---
title: 'educationSubmission: unsubmit'
description: 'アクション起動された後、割り当ての送信時に、受講生受講者が要求していることを示します。 この操作は、受講者のみ取得できます。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fc17216800c39f0a094ba5f8d9f281394ba7e2de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945469"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="ae089-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="ae089-104">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="ae089-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae089-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae089-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae089-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae089-107">アクション起動された後、割り当ての送信時に、受講生受講者が要求していることを示します。</span><span class="sxs-lookup"><span data-stu-id="ae089-107">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="ae089-108">この操作は、受講者のみ取得できます。</span><span class="sxs-lookup"><span data-stu-id="ae089-108">This action can only be taken by the student.</span></span> <span data-ttu-id="ae089-109">「送信」からの提出書類のステータスを変更すると、「処理中」にこのされます。</span><span class="sxs-lookup"><span data-stu-id="ae089-109">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="ae089-110">送信中に、すべてのリソースからコピーされます submittedResources workingResources バケットにします。</span><span class="sxs-lookup"><span data-stu-id="ae089-110">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="ae089-111">先生はグレーディングの作業中のリソースの一覧を見ています。</span><span class="sxs-lookup"><span data-stu-id="ae089-111">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae089-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae089-112">Permissions</span></span>
<span data-ttu-id="ae089-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae089-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae089-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae089-115">Permission type</span></span>      | <span data-ttu-id="ae089-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae089-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae089-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae089-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="ae089-118">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae089-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ae089-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae089-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ae089-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae089-120">Not supported.</span></span>  |
|<span data-ttu-id="ae089-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae089-121">Application</span></span> | <span data-ttu-id="ae089-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae089-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ae089-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae089-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="ae089-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae089-124">Request headers</span></span>
| <span data-ttu-id="ae089-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae089-125">Header</span></span>       | <span data-ttu-id="ae089-126">値</span><span class="sxs-lookup"><span data-stu-id="ae089-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ae089-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae089-127">Authorization</span></span>  | <span data-ttu-id="ae089-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae089-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae089-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae089-130">Request body</span></span>
<span data-ttu-id="ae089-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae089-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae089-132">応答</span><span class="sxs-lookup"><span data-stu-id="ae089-132">Response</span></span>
<span data-ttu-id="ae089-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ae089-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae089-135">例</span><span class="sxs-lookup"><span data-stu-id="ae089-135">Example</span></span>
<span data-ttu-id="ae089-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="ae089-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ae089-137">要求</span><span class="sxs-lookup"><span data-stu-id="ae089-137">Request</span></span>
<span data-ttu-id="ae089-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ae089-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="ae089-139">応答</span><span class="sxs-lookup"><span data-stu-id="ae089-139">Response</span></span>
<span data-ttu-id="ae089-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ae089-140">The following is an example of the response.</span></span>

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
