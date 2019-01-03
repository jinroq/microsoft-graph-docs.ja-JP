---
title: リストの割り当て
description: 割り当てオブジェクトのリストを取得します。 教師を許可して、クラスのすべての割り当てオブジェクトを参照してください。 受講者は、それらに割り当てられている割り当てだけを参照してください。
author: mmast-msft
ms.openlocfilehash: c7fbab429b238a0ae7f1814066eedfe793096f02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361405"
---
# <a name="list-assignments"></a><span data-ttu-id="cbb14-105">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="cbb14-105">List assignments</span></span>

> <span data-ttu-id="cbb14-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cbb14-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbb14-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbb14-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbb14-108">割り当てオブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="cbb14-108">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="cbb14-109">教師を許可して、クラスのすべての割り当てオブジェクトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbb14-109">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="cbb14-110">受講者は、それらに割り当てられている割り当てだけを参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbb14-110">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbb14-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cbb14-111">Permissions</span></span>
<span data-ttu-id="cbb14-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbb14-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbb14-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cbb14-114">Permission type</span></span>      | <span data-ttu-id="cbb14-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cbb14-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbb14-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cbb14-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cbb14-117">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbb14-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="cbb14-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cbb14-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cbb14-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbb14-119">Not supported.</span></span>  |
|<span data-ttu-id="cbb14-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cbb14-120">Application</span></span> | <span data-ttu-id="cbb14-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbb14-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cbb14-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cbb14-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cbb14-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="cbb14-123">Optional query parameters</span></span>
<span data-ttu-id="cbb14-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cbb14-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbb14-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbb14-125">Request headers</span></span>
| <span data-ttu-id="cbb14-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbb14-126">Header</span></span>       | <span data-ttu-id="cbb14-127">値</span><span class="sxs-lookup"><span data-stu-id="cbb14-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cbb14-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbb14-128">Authorization</span></span>  | <span data-ttu-id="cbb14-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cbb14-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cbb14-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="cbb14-131">Request body</span></span>
<span data-ttu-id="cbb14-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cbb14-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cbb14-133">応答</span><span class="sxs-lookup"><span data-stu-id="cbb14-133">Response</span></span>
<span data-ttu-id="cbb14-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationAssignment](../resources/educationassignment.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="cbb14-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbb14-135">例</span><span class="sxs-lookup"><span data-stu-id="cbb14-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbb14-136">要求</span><span class="sxs-lookup"><span data-stu-id="cbb14-136">Request</span></span>
<span data-ttu-id="cbb14-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cbb14-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="cbb14-138">応答</span><span class="sxs-lookup"><span data-stu-id="cbb14-138">Response</span></span>
<span data-ttu-id="cbb14-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cbb14-139">The following is an example of the response.</span></span> 

><span data-ttu-id="cbb14-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="cbb14-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->