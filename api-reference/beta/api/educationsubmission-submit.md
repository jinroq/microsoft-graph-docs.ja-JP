---
title: 'educationSubmission: 送信'
description: 学生が作業を行われ、割り当てで入稿する準備ができなことを示す動作です。 この操作は、受講者のみ取得できます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d1fd41c66e3f54898f6086a9bf14a0b53763df88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915810"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="8e19d-104">educationSubmission: 送信</span><span class="sxs-lookup"><span data-stu-id="8e19d-104">educationSubmission: submit</span></span>

> <span data-ttu-id="8e19d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8e19d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e19d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e19d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e19d-107">学生が作業を行われ、割り当てで入稿する準備ができなことを示す動作です。</span><span class="sxs-lookup"><span data-stu-id="8e19d-107">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="8e19d-108">この操作は、受講者のみ取得できます。</span><span class="sxs-lookup"><span data-stu-id="8e19d-108">This action can only be taken by the student.</span></span> <span data-ttu-id="8e19d-109">「処理中」に「送信」からの提出書類のステータスが変更されます。</span><span class="sxs-lookup"><span data-stu-id="8e19d-109">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="8e19d-110">送信中に、すべてのリソースは、submittedResources バケットにコピーされます。</span><span class="sxs-lookup"><span data-stu-id="8e19d-110">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="8e19d-111">先生はグレーディングの送信済みのリソースの一覧を見ています。</span><span class="sxs-lookup"><span data-stu-id="8e19d-111">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e19d-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8e19d-112">Permissions</span></span>
<span data-ttu-id="8e19d-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e19d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e19d-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e19d-115">Permission type</span></span>      | <span data-ttu-id="8e19d-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e19d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e19d-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e19d-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="8e19d-118">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e19d-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8e19d-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e19d-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8e19d-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e19d-120">Not supported.</span></span>  |
|<span data-ttu-id="8e19d-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e19d-121">Application</span></span> | <span data-ttu-id="8e19d-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e19d-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8e19d-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e19d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="8e19d-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e19d-124">Request headers</span></span>
| <span data-ttu-id="8e19d-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e19d-125">Header</span></span>       | <span data-ttu-id="8e19d-126">値</span><span class="sxs-lookup"><span data-stu-id="8e19d-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e19d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e19d-127">Authorization</span></span>  | <span data-ttu-id="8e19d-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8e19d-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e19d-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e19d-130">Request body</span></span>
<span data-ttu-id="8e19d-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8e19d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e19d-132">応答</span><span class="sxs-lookup"><span data-stu-id="8e19d-132">Response</span></span>
<span data-ttu-id="8e19d-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8e19d-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e19d-135">例</span><span class="sxs-lookup"><span data-stu-id="8e19d-135">Example</span></span>
<span data-ttu-id="8e19d-136">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8e19d-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8e19d-137">要求</span><span class="sxs-lookup"><span data-stu-id="8e19d-137">Request</span></span>
<span data-ttu-id="8e19d-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e19d-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="8e19d-139">応答</span><span class="sxs-lookup"><span data-stu-id="8e19d-139">Response</span></span>
<span data-ttu-id="8e19d-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8e19d-140">The following is an example of the response.</span></span>

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
