---
title: EducationAssignment を作成する
description: '新しい割り当てを作成します。 クラス内の教師のみが、割り当てを作成できます。 割り当ては下書き状態で開始します。これは、発行が呼び出されるまで、学生に割り当てが表示されないことを意味します。  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f8f4b7fe917b9366f852b6fe0b620754890705a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955364"
---
# <a name="create-educationassignment"></a><span data-ttu-id="4958f-105">EducationAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="4958f-105">Create educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4958f-106">新しい割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="4958f-106">Creates a new assignment.</span></span> <span data-ttu-id="4958f-107">クラス内の教師のみが、割り当てを作成できます。</span><span class="sxs-lookup"><span data-stu-id="4958f-107">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="4958f-108">割り当ては下書き状態で開始します。これは、発行が呼び出されるまで、学生に割り当てが表示されないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="4958f-108">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="4958f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4958f-109">Permissions</span></span>
<span data-ttu-id="4958f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4958f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4958f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4958f-112">Permission type</span></span>      | <span data-ttu-id="4958f-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4958f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4958f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4958f-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="4958f-115">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="4958f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4958f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4958f-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4958f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4958f-117">Not supported.</span></span>  |
|<span data-ttu-id="4958f-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4958f-118">Application</span></span> | <span data-ttu-id="4958f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4958f-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4958f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4958f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="4958f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4958f-121">Request headers</span></span>
| <span data-ttu-id="4958f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4958f-122">Header</span></span>       | <span data-ttu-id="4958f-123">値</span><span class="sxs-lookup"><span data-stu-id="4958f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4958f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4958f-124">Authorization</span></span>  | <span data-ttu-id="4958f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4958f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4958f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4958f-127">Content-Type</span></span>  | <span data-ttu-id="4958f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4958f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4958f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="4958f-129">Request body</span></span>
<span data-ttu-id="4958f-130">要求本文で、 [educationAssignment](../resources/educationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4958f-130">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="4958f-131">応答</span><span class="sxs-lookup"><span data-stu-id="4958f-131">Response</span></span>
<span data-ttu-id="4958f-132">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[educationAssignment](../resources/educationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4958f-132">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4958f-133">例</span><span class="sxs-lookup"><span data-stu-id="4958f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4958f-134">要求</span><span class="sxs-lookup"><span data-stu-id="4958f-134">Request</span></span>
<span data-ttu-id="4958f-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4958f-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="4958f-136">要求本文で、 [educationAssignment](../resources/educationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4958f-136">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="4958f-137">応答</span><span class="sxs-lookup"><span data-stu-id="4958f-137">Response</span></span>
<span data-ttu-id="4958f-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4958f-138">The following is an example of the response.</span></span> 

><span data-ttu-id="4958f-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4958f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
