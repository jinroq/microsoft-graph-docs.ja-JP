---
title: educationAssignment を作成する
description: '新しい割り当てを作成します。 クラス内の教師のみが、割り当てを作成できます。 割り当ては下書き状態で開始します。これは、発行が呼び出されるまで、学生に割り当てが表示されないことを意味します。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: bac79b8f85eb6141b5159ac5dc7acbf067bf571c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457803"
---
# <a name="create-educationassignment"></a><span data-ttu-id="c787c-105">educationAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="c787c-105">Create educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c787c-106">新しい割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="c787c-106">Creates a new assignment.</span></span> <span data-ttu-id="c787c-107">クラス内の教師のみが、割り当てを作成できます。</span><span class="sxs-lookup"><span data-stu-id="c787c-107">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="c787c-108">割り当ては下書き状態で開始します。これは、発行が呼び出されるまで、学生に割り当てが表示されないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="c787c-108">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c787c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c787c-109">Permissions</span></span>
<span data-ttu-id="c787c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c787c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c787c-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c787c-112">Permission type</span></span>      | <span data-ttu-id="c787c-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c787c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c787c-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c787c-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="c787c-115">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="c787c-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c787c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c787c-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c787c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c787c-117">Not supported.</span></span>  |
|<span data-ttu-id="c787c-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c787c-118">Application</span></span> | <span data-ttu-id="c787c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c787c-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c787c-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c787c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="c787c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c787c-121">Request headers</span></span>
| <span data-ttu-id="c787c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c787c-122">Header</span></span>       | <span data-ttu-id="c787c-123">値</span><span class="sxs-lookup"><span data-stu-id="c787c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c787c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c787c-124">Authorization</span></span>  | <span data-ttu-id="c787c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c787c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c787c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c787c-127">Content-Type</span></span>  | <span data-ttu-id="c787c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c787c-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c787c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c787c-129">Request body</span></span>
<span data-ttu-id="c787c-130">要求本文で、 [educationAssignment](../resources/educationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c787c-130">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c787c-131">応答</span><span class="sxs-lookup"><span data-stu-id="c787c-131">Response</span></span>
<span data-ttu-id="c787c-132">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[educationAssignment](../resources/educationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c787c-132">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c787c-133">例</span><span class="sxs-lookup"><span data-stu-id="c787c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c787c-134">要求</span><span class="sxs-lookup"><span data-stu-id="c787c-134">Request</span></span>
<span data-ttu-id="c787c-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c787c-135">The following is an example of the request.</span></span>
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
      "contentType": "text",
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
<span data-ttu-id="c787c-136">要求本文で、 [educationAssignment](../resources/educationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c787c-136">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c787c-137">応答</span><span class="sxs-lookup"><span data-stu-id="c787c-137">Response</span></span>
<span data-ttu-id="c787c-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c787c-138">The following is an example of the response.</span></span> 

><span data-ttu-id="c787c-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c787c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "contentType": "text",
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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-post-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
