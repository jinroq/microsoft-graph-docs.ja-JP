---
title: 'educationSubmission: 送信'
description: 学生が作業を行われ、割り当てで入稿する準備ができなことを示す動作です。 この操作は、受講者のみ取得できます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3f67e5b07ed1093ee63e9b6fdf7647fa6891dacc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510772"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="c3982-104">educationSubmission: 送信</span><span class="sxs-lookup"><span data-stu-id="c3982-104">educationSubmission: submit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3982-105">学生が作業を行われ、割り当てで入稿する準備ができなことを示す動作です。</span><span class="sxs-lookup"><span data-stu-id="c3982-105">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="c3982-106">この操作は、受講者のみ取得できます。</span><span class="sxs-lookup"><span data-stu-id="c3982-106">This action can only be taken by the student.</span></span> <span data-ttu-id="c3982-107">「処理中」に「送信」からの提出書類のステータスが変更されます。</span><span class="sxs-lookup"><span data-stu-id="c3982-107">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="c3982-108">送信中に、すべてのリソースは、submittedResources バケットにコピーされます。</span><span class="sxs-lookup"><span data-stu-id="c3982-108">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="c3982-109">先生はグレーディングの送信済みのリソースの一覧を見ています。</span><span class="sxs-lookup"><span data-stu-id="c3982-109">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3982-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3982-110">Permissions</span></span>
<span data-ttu-id="c3982-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3982-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3982-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3982-113">Permission type</span></span>      | <span data-ttu-id="c3982-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3982-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3982-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3982-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="c3982-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3982-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c3982-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3982-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c3982-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3982-118">Not supported.</span></span>  |
|<span data-ttu-id="c3982-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3982-119">Application</span></span> | <span data-ttu-id="c3982-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3982-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c3982-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3982-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="c3982-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3982-122">Request headers</span></span>
| <span data-ttu-id="c3982-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3982-123">Header</span></span>       | <span data-ttu-id="c3982-124">値</span><span class="sxs-lookup"><span data-stu-id="c3982-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3982-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3982-125">Authorization</span></span>  | <span data-ttu-id="c3982-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3982-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3982-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3982-128">Request body</span></span>
<span data-ttu-id="c3982-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3982-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3982-130">応答</span><span class="sxs-lookup"><span data-stu-id="c3982-130">Response</span></span>
<span data-ttu-id="c3982-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="c3982-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3982-133">例</span><span class="sxs-lookup"><span data-stu-id="c3982-133">Example</span></span>
<span data-ttu-id="c3982-134">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c3982-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c3982-135">要求</span><span class="sxs-lookup"><span data-stu-id="c3982-135">Request</span></span>
<span data-ttu-id="c3982-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c3982-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="c3982-137">応答</span><span class="sxs-lookup"><span data-stu-id="c3982-137">Response</span></span>
<span data-ttu-id="c3982-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c3982-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-submit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
