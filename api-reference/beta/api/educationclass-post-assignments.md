---
title: EducationAssignment を作成します。
description: '新しい割り当てを作成します。 クラスで教師だけでは、割り当てを作成できます。 割り当ては、エントリの公開が呼び出されるまで、受講者は、割り当てが表示されないことを意味する下書きの状態で起動します。  '
ms.openlocfilehash: 9a6af2a0c0689ca2118ce4d06a55d7b27a70a4ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068651"
---
# <a name="create-educationassignment"></a><span data-ttu-id="34fb7-105">EducationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="34fb7-105">Create educationAssignment</span></span>

> <span data-ttu-id="34fb7-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34fb7-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34fb7-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34fb7-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34fb7-108">新しい割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="34fb7-108">Creates a new assignment.</span></span> <span data-ttu-id="34fb7-109">クラスで教師だけでは、割り当てを作成できます。</span><span class="sxs-lookup"><span data-stu-id="34fb7-109">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="34fb7-110">割り当ては、エントリの公開が呼び出されるまで、受講者は、割り当てが表示されないことを意味する下書きの状態で起動します。</span><span class="sxs-lookup"><span data-stu-id="34fb7-110">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="34fb7-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34fb7-111">Permissions</span></span>
<span data-ttu-id="34fb7-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34fb7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34fb7-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34fb7-114">Permission type</span></span>      | <span data-ttu-id="34fb7-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34fb7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34fb7-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34fb7-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="34fb7-117">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34fb7-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="34fb7-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34fb7-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="34fb7-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34fb7-119">Not supported.</span></span>  |
|<span data-ttu-id="34fb7-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34fb7-120">Application</span></span> | <span data-ttu-id="34fb7-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34fb7-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="34fb7-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34fb7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="34fb7-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34fb7-123">Request headers</span></span>
| <span data-ttu-id="34fb7-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34fb7-124">Header</span></span>       | <span data-ttu-id="34fb7-125">値</span><span class="sxs-lookup"><span data-stu-id="34fb7-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34fb7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="34fb7-126">Authorization</span></span>  | <span data-ttu-id="34fb7-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="34fb7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="34fb7-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34fb7-129">Content-Type</span></span>  | <span data-ttu-id="34fb7-130">application/json</span><span class="sxs-lookup"><span data-stu-id="34fb7-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34fb7-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="34fb7-131">Request body</span></span>
<span data-ttu-id="34fb7-132">要求の本文には、 [educationAssignment](../resources/educationassignment.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="34fb7-132">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="34fb7-133">応答</span><span class="sxs-lookup"><span data-stu-id="34fb7-133">Response</span></span>
<span data-ttu-id="34fb7-134">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文内の[educationAssignment](../resources/educationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="34fb7-134">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34fb7-135">例</span><span class="sxs-lookup"><span data-stu-id="34fb7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34fb7-136">要求</span><span class="sxs-lookup"><span data-stu-id="34fb7-136">Request</span></span>
<span data-ttu-id="34fb7-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34fb7-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignment_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignments
Content-type: application/json
Content-length: 279

{ 
  "dueDateTime": "2014-02-01T00:00:00Z",
  "displayName": "Midterm 1",
    "instructions":  {
      "contentType": "Text",
      "content": "Read chapters 1 through 3"
    },
      "grading": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "assignTo": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentClassRecipient"
      },
      "status":"draft",
      "allowStudentsToAddResourcesToSubmission": true
}
```
<span data-ttu-id="34fb7-138">要求の本文には、 [educationAssignment](../resources/educationassignment.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="34fb7-138">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="34fb7-139">応答</span><span class="sxs-lookup"><span data-stu-id="34fb7-139">Response</span></span>
<span data-ttu-id="34fb7-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34fb7-140">The following is an example of the response.</span></span> 

><span data-ttu-id="34fb7-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="34fb7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 279

{
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "2014-02-01T00:00:00Z",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-02-01T00:00:00Z",
  "classId": "11018",
  "createdBy": {
      "application": null,
      "device": null,
      "user": {
          "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
          "displayName": null
      }
  },
  "createdDateTime": "2014-02-01T00:00:00Z",
  "displayName": "published",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "grading": {
    "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
    "maxPoints": 100
  },
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "lastModifiedBy": {
      "application": null,
      "device": null,
      "user": {
          "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
          "displayName": null
      }
  },
  "lastModifiedDateTime": "2014-02-01T00:00:00Z",
  "status": "published"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->