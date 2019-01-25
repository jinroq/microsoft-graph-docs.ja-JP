---
title: 'educationSubmission: unsubmit'
description: 'アクション起動された後、割り当ての送信時に、受講生受講者が要求していることを示します。 この操作は、受講者のみ取得できます。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e8ce4c5d4bf68dca22f686a1b3647c67d7836bed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513509"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="75115-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="75115-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75115-105">アクション起動された後、割り当ての送信時に、受講生受講者が要求していることを示します。</span><span class="sxs-lookup"><span data-stu-id="75115-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="75115-106">この操作は、受講者のみ取得できます。</span><span class="sxs-lookup"><span data-stu-id="75115-106">This action can only be taken by the student.</span></span> <span data-ttu-id="75115-107">「送信」からの提出書類のステータスを変更すると、「処理中」にこのされます。</span><span class="sxs-lookup"><span data-stu-id="75115-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="75115-108">送信中に、すべてのリソースからコピーされます submittedResources workingResources バケットにします。</span><span class="sxs-lookup"><span data-stu-id="75115-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="75115-109">先生はグレーディングの作業中のリソースの一覧を見ています。</span><span class="sxs-lookup"><span data-stu-id="75115-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="75115-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="75115-110">Permissions</span></span>
<span data-ttu-id="75115-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75115-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75115-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75115-113">Permission type</span></span>      | <span data-ttu-id="75115-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="75115-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75115-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75115-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="75115-116">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75115-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="75115-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75115-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="75115-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75115-118">Not supported.</span></span>  |
|<span data-ttu-id="75115-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75115-119">Application</span></span> | <span data-ttu-id="75115-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75115-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="75115-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75115-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="75115-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75115-122">Request headers</span></span>
| <span data-ttu-id="75115-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75115-123">Header</span></span>       | <span data-ttu-id="75115-124">値</span><span class="sxs-lookup"><span data-stu-id="75115-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="75115-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="75115-125">Authorization</span></span>  | <span data-ttu-id="75115-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="75115-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="75115-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="75115-128">Request body</span></span>
<span data-ttu-id="75115-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="75115-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75115-130">応答</span><span class="sxs-lookup"><span data-stu-id="75115-130">Response</span></span>
<span data-ttu-id="75115-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="75115-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75115-133">例</span><span class="sxs-lookup"><span data-stu-id="75115-133">Example</span></span>
<span data-ttu-id="75115-134">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="75115-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="75115-135">要求</span><span class="sxs-lookup"><span data-stu-id="75115-135">Request</span></span>
<span data-ttu-id="75115-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="75115-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="75115-137">応答</span><span class="sxs-lookup"><span data-stu-id="75115-137">Response</span></span>
<span data-ttu-id="75115-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="75115-138">The following is an example of the response.</span></span>

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
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
