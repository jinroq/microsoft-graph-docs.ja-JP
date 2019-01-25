---
title: リストの割り当て
description: 割り当てオブジェクトのリストを取得します。 教師を許可して、クラスのすべての割り当てオブジェクトを参照してください。 受講者は、それらに割り当てられている割り当てだけを参照してください。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7cd47c61d4958d42ce099396147d421a6555041b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519144"
---
# <a name="list-assignments"></a><span data-ttu-id="36ba2-105">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="36ba2-105">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36ba2-106">割り当てオブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="36ba2-106">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="36ba2-107">教師を許可して、クラスのすべての割り当てオブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="36ba2-107">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="36ba2-108">受講者は、それらに割り当てられている割り当てだけを参照してください。</span><span class="sxs-lookup"><span data-stu-id="36ba2-108">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="36ba2-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="36ba2-109">Permissions</span></span>
<span data-ttu-id="36ba2-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36ba2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36ba2-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36ba2-112">Permission type</span></span>      | <span data-ttu-id="36ba2-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="36ba2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36ba2-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36ba2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="36ba2-115">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36ba2-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="36ba2-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36ba2-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="36ba2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36ba2-117">Not supported.</span></span>  |
|<span data-ttu-id="36ba2-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36ba2-118">Application</span></span> | <span data-ttu-id="36ba2-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36ba2-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36ba2-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36ba2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36ba2-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="36ba2-121">Optional query parameters</span></span>
<span data-ttu-id="36ba2-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="36ba2-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36ba2-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36ba2-123">Request headers</span></span>
| <span data-ttu-id="36ba2-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36ba2-124">Header</span></span>       | <span data-ttu-id="36ba2-125">値</span><span class="sxs-lookup"><span data-stu-id="36ba2-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36ba2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="36ba2-126">Authorization</span></span>  | <span data-ttu-id="36ba2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="36ba2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36ba2-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="36ba2-129">Request body</span></span>
<span data-ttu-id="36ba2-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="36ba2-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="36ba2-131">応答</span><span class="sxs-lookup"><span data-stu-id="36ba2-131">Response</span></span>
<span data-ttu-id="36ba2-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationAssignment](../resources/educationassignment.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="36ba2-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36ba2-133">例</span><span class="sxs-lookup"><span data-stu-id="36ba2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36ba2-134">要求</span><span class="sxs-lookup"><span data-stu-id="36ba2-134">Request</span></span>
<span data-ttu-id="36ba2-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36ba2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="36ba2-136">応答</span><span class="sxs-lookup"><span data-stu-id="36ba2-136">Response</span></span>
<span data-ttu-id="36ba2-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="36ba2-137">The following is an example of the response.</span></span> 

><span data-ttu-id="36ba2-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="36ba2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
  "value": [
    {
      "id": "19002",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
