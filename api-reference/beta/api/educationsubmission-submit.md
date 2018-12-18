---
title: 'educationSubmission: 送信'
description: 学生が作業を行われ、割り当てで入稿する準備ができなことを示す動作です。 この操作は、受講者のみ取得できます。
author: dipakboyed
ms.openlocfilehash: 25fc24823081c6f148617ad31d0f7b797b0e2a80
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343331"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="843c4-104">educationSubmission: 送信</span><span class="sxs-lookup"><span data-stu-id="843c4-104">educationSubmission: submit</span></span>

> <span data-ttu-id="843c4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="843c4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="843c4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="843c4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="843c4-107">学生が作業を行われ、割り当てで入稿する準備ができなことを示す動作です。</span><span class="sxs-lookup"><span data-stu-id="843c4-107">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="843c4-108">この操作は、受講者のみ取得できます。</span><span class="sxs-lookup"><span data-stu-id="843c4-108">This action can only be taken by the student.</span></span> <span data-ttu-id="843c4-109">「処理中」に「送信」からの提出書類のステータスが変更されます。</span><span class="sxs-lookup"><span data-stu-id="843c4-109">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="843c4-110">送信中に、すべてのリソースは、submittedResources バケットにコピーされます。</span><span class="sxs-lookup"><span data-stu-id="843c4-110">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="843c4-111">先生はグレーディングの送信済みのリソースの一覧を見ています。</span><span class="sxs-lookup"><span data-stu-id="843c4-111">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="843c4-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="843c4-112">Permissions</span></span>
<span data-ttu-id="843c4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="843c4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="843c4-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="843c4-115">Permission type</span></span>      | <span data-ttu-id="843c4-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="843c4-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="843c4-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="843c4-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="843c4-118">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="843c4-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="843c4-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="843c4-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="843c4-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="843c4-120">Not supported.</span></span>  |
|<span data-ttu-id="843c4-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="843c4-121">Application</span></span> | <span data-ttu-id="843c4-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="843c4-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="843c4-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="843c4-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="843c4-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="843c4-124">Request headers</span></span>
| <span data-ttu-id="843c4-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="843c4-125">Header</span></span>       | <span data-ttu-id="843c4-126">値</span><span class="sxs-lookup"><span data-stu-id="843c4-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="843c4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="843c4-127">Authorization</span></span>  | <span data-ttu-id="843c4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="843c4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="843c4-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="843c4-130">Request body</span></span>
<span data-ttu-id="843c4-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="843c4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="843c4-132">応答</span><span class="sxs-lookup"><span data-stu-id="843c4-132">Response</span></span>
<span data-ttu-id="843c4-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="843c4-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="843c4-135">例</span><span class="sxs-lookup"><span data-stu-id="843c4-135">Example</span></span>
<span data-ttu-id="843c4-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="843c4-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="843c4-137">要求</span><span class="sxs-lookup"><span data-stu-id="843c4-137">Request</span></span>
<span data-ttu-id="843c4-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="843c4-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="843c4-139">応答</span><span class="sxs-lookup"><span data-stu-id="843c4-139">Response</span></span>
<span data-ttu-id="843c4-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="843c4-140">The following is an example of the response.</span></span>

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