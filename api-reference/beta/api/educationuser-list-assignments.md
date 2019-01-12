---
title: リストの割り当て
description: クラスのすべてのユーザーに割り当てられている割り当ての一覧を返します。 このユーティリティの名前空間は、呼び出し元が各クラスからの割り当てを要求することのではなく、1 回の呼び出しで、学生のすべての割り当てを検索できます。 クラスの名前空間内での割り当ての詳細な情報を取得するために必要な割り当ての一覧が含まれます。 割り当ての他のすべての操作は、クラスの名前空間を使用してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0366a159e3e28e9ad3933ec4d1eea6799c1f65c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940842"
---
# <a name="list-assignments"></a><span data-ttu-id="5c165-106">リストの割り当て</span><span class="sxs-lookup"><span data-stu-id="5c165-106">List assignments</span></span>

> <span data-ttu-id="5c165-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c165-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c165-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c165-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c165-109">クラスのすべてのユーザーに割り当てられている割り当ての一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="5c165-109">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="5c165-110">このユーティリティの名前空間は、呼び出し元が各クラスからの割り当てを要求することのではなく、1 回の呼び出しで、学生のすべての割り当てを検索できます。</span><span class="sxs-lookup"><span data-stu-id="5c165-110">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="5c165-111">クラスの名前空間内での割り当ての詳細な情報を取得するために必要な割り当ての一覧が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5c165-111">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="5c165-112">割り当ての他のすべての操作は、クラスの名前空間を使用してください。</span><span class="sxs-lookup"><span data-stu-id="5c165-112">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c165-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5c165-113">Permissions</span></span>
<span data-ttu-id="5c165-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c165-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c165-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c165-116">Permission type</span></span>      | <span data-ttu-id="5c165-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c165-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c165-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c165-118">Delegated (work or school account)</span></span> | <span data-ttu-id="5c165-119">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c165-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5c165-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c165-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c165-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c165-121">Not supported.</span></span>   |
|<span data-ttu-id="5c165-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c165-122">Application</span></span> | <span data-ttu-id="5c165-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c165-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5c165-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c165-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c165-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5c165-125">Optional query parameters</span></span>
<span data-ttu-id="5c165-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5c165-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c165-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c165-127">Request headers</span></span>
| <span data-ttu-id="5c165-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c165-128">Header</span></span>       | <span data-ttu-id="5c165-129">値</span><span class="sxs-lookup"><span data-stu-id="5c165-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c165-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c165-130">Authorization</span></span>  | <span data-ttu-id="5c165-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5c165-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c165-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c165-133">Request body</span></span>
<span data-ttu-id="5c165-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5c165-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5c165-135">応答</span><span class="sxs-lookup"><span data-stu-id="5c165-135">Response</span></span>
<span data-ttu-id="5c165-136">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationAssignment](../resources/educationassignment.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5c165-136">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c165-137">例</span><span class="sxs-lookup"><span data-stu-id="5c165-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c165-138">要求</span><span class="sxs-lookup"><span data-stu-id="5c165-138">Request</span></span>
<span data-ttu-id="5c165-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c165-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="5c165-140">応答</span><span class="sxs-lookup"><span data-stu-id="5c165-140">Response</span></span>
<span data-ttu-id="5c165-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c165-141">The following is an example of the response.</span></span> 

><span data-ttu-id="5c165-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5c165-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "assignDateTime": "2014-01-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-01-01T00:00:00Z",
      "classId": "11010",
      "createdBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "createdDateTime": "2014-01-01T00:00:00Z",
      "displayName": "Assignment 1",
      "dueDateTime": "2014-01-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "content": "Answer every question correctly",
        "contentType": "Text"
      },
      "lastModifiedBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "lastModifiedDateTime": "2014-01-01T00:00:00Z",
      "status": "assigned"
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
