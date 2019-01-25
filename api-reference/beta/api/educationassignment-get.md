---
title: EducationAssignment を取得します。
description: " 先生は、クラスのすべての割り当てを確認できます。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eba959dcaf2478f3c49fc0fbb434d7269e37e5ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508371"
---
# <a name="get-educationassignment"></a><span data-ttu-id="fb4d1-103">EducationAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-103">Get educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb4d1-104">プロパティとリレーションシップの割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-104">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="fb4d1-105">受講者はそれに割り当てられた割り当てのみを参照できます。先生は、クラスのすべての割り当てを確認できます。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-105">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb4d1-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fb4d1-106">Permissions</span></span>
<span data-ttu-id="fb4d1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fb4d1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb4d1-109">Permission type</span></span>      | <span data-ttu-id="fb4d1-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb4d1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb4d1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb4d1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fb4d1-112">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fb4d1-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="fb4d1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb4d1-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fb4d1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-114">Not supported.</span></span>  |
|<span data-ttu-id="fb4d1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb4d1-115">Application</span></span> | <span data-ttu-id="fb4d1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fb4d1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb4d1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fb4d1-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fb4d1-118">Optional query parameters</span></span>
<span data-ttu-id="fb4d1-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb4d1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb4d1-120">Request headers</span></span>
| <span data-ttu-id="fb4d1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb4d1-121">Header</span></span>       | <span data-ttu-id="fb4d1-122">値</span><span class="sxs-lookup"><span data-stu-id="fb4d1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fb4d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb4d1-123">Authorization</span></span>  | <span data-ttu-id="fb4d1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb4d1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fb4d1-126">Request body</span></span>
<span data-ttu-id="fb4d1-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb4d1-128">応答</span><span class="sxs-lookup"><span data-stu-id="fb4d1-128">Response</span></span>
<span data-ttu-id="fb4d1-129">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationAssignment](../resources/educationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-129">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fb4d1-130">例</span><span class="sxs-lookup"><span data-stu-id="fb4d1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fb4d1-131">要求</span><span class="sxs-lookup"><span data-stu-id="fb4d1-131">Request</span></span>
<span data-ttu-id="fb4d1-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="fb4d1-133">応答</span><span class="sxs-lookup"><span data-stu-id="fb4d1-133">Response</span></span>
<span data-ttu-id="fb4d1-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-134">The following is an example of the response.</span></span> 

><span data-ttu-id="fb4d1-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="fb4d1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
      "maxPoints": 100
  },
  "instructions": {
    "content": "Answer every question correctly",
    "contentType": "Text"
  },
  "lastModifiedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
