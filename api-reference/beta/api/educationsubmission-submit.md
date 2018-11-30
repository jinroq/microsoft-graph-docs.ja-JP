---
title: 'educationSubmission: 送信'
description: . 送信中に、すべてのリソースは、submittedResources バケットにコピーされます。 先生はグレーディングの送信済みのリソースの一覧を見ています。
ms.openlocfilehash: 566948278ffacb1169842c49aa11c78cba0a5f3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068234"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="d723b-105">educationSubmission: 送信</span><span class="sxs-lookup"><span data-stu-id="d723b-105">educationSubmission: submit</span></span>

> <span data-ttu-id="d723b-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d723b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d723b-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d723b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d723b-108">学生が作業を行われ、割り当てで入稿する準備ができなことを示す動作です。</span><span class="sxs-lookup"><span data-stu-id="d723b-108">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="d723b-109">この操作は、受講者のみ取得できます。</span><span class="sxs-lookup"><span data-stu-id="d723b-109">This action can only be taken by the student.</span></span> <span data-ttu-id="d723b-110">「処理中」に「送信」からの提出書類のステータスが変更されます。</span><span class="sxs-lookup"><span data-stu-id="d723b-110">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="d723b-111">送信中に、すべてのリソースは、submittedResources バケットにコピーされます。</span><span class="sxs-lookup"><span data-stu-id="d723b-111">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="d723b-112">先生はグレーディングの送信済みのリソースの一覧を見ています。</span><span class="sxs-lookup"><span data-stu-id="d723b-112">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="d723b-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d723b-113">Permissions</span></span>
<span data-ttu-id="d723b-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d723b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d723b-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d723b-116">Permission type</span></span>      | <span data-ttu-id="d723b-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d723b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d723b-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d723b-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="d723b-119">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d723b-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d723b-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d723b-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d723b-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d723b-121">Not supported.</span></span>  |
|<span data-ttu-id="d723b-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d723b-122">Application</span></span> | <span data-ttu-id="d723b-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d723b-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d723b-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d723b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="d723b-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d723b-125">Request headers</span></span>
| <span data-ttu-id="d723b-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d723b-126">Header</span></span>       | <span data-ttu-id="d723b-127">値</span><span class="sxs-lookup"><span data-stu-id="d723b-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d723b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="d723b-128">Authorization</span></span>  | <span data-ttu-id="d723b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d723b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d723b-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="d723b-131">Request body</span></span>
<span data-ttu-id="d723b-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d723b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d723b-133">応答</span><span class="sxs-lookup"><span data-stu-id="d723b-133">Response</span></span>
<span data-ttu-id="d723b-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d723b-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d723b-136">例</span><span class="sxs-lookup"><span data-stu-id="d723b-136">Example</span></span>
<span data-ttu-id="d723b-137">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="d723b-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d723b-138">要求</span><span class="sxs-lookup"><span data-stu-id="d723b-138">Request</span></span>
<span data-ttu-id="d723b-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d723b-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="d723b-140">応答</span><span class="sxs-lookup"><span data-stu-id="d723b-140">Response</span></span>
<span data-ttu-id="d723b-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d723b-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->