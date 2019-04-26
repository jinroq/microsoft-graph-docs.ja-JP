---
title: 割り当てを一覧表示する
description: すべてのクラスについて、ユーザーに割り当てられている割り当ての一覧を返します。 このユーティリティ名前空間を使用すると、発信者は各クラスの割り当てを要求するのではなく、1回の呼び出しですべての学生の割り当てを検索できます。 割り当てリストには、クラス名前空間内の割り当ての詳細情報を取得するために必要な情報が含まれています。 割り当てに対する他のすべての操作では、クラスの名前空間を使用する必要があります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 566eaa526981a14ab4ce622fbad9b858f5b40ef9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33321964"
---
# <a name="list-assignments"></a><span data-ttu-id="c89da-106">割り当てを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c89da-106">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c89da-107">すべてのクラスについて、ユーザーに割り当てられている割り当ての一覧を返します。</span><span class="sxs-lookup"><span data-stu-id="c89da-107">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="c89da-108">このユーティリティ名前空間を使用すると、発信者は各クラスの割り当てを要求するのではなく、1回の呼び出しですべての学生の割り当てを検索できます。</span><span class="sxs-lookup"><span data-stu-id="c89da-108">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="c89da-109">割り当てリストには、クラス名前空間内の割り当ての詳細情報を取得するために必要な情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c89da-109">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="c89da-110">割り当てに対する他のすべての操作では、クラスの名前空間を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c89da-110">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="c89da-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c89da-111">Permissions</span></span>
<span data-ttu-id="c89da-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c89da-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c89da-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c89da-114">Permission type</span></span>      | <span data-ttu-id="c89da-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c89da-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c89da-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c89da-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c89da-117">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="c89da-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c89da-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c89da-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c89da-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c89da-119">Not supported.</span></span>   |
|<span data-ttu-id="c89da-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c89da-120">Application</span></span> | <span data-ttu-id="c89da-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c89da-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c89da-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c89da-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c89da-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c89da-123">Optional query parameters</span></span>
<span data-ttu-id="c89da-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c89da-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c89da-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c89da-125">Request headers</span></span>
| <span data-ttu-id="c89da-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c89da-126">Header</span></span>       | <span data-ttu-id="c89da-127">値</span><span class="sxs-lookup"><span data-stu-id="c89da-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c89da-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c89da-128">Authorization</span></span>  | <span data-ttu-id="c89da-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c89da-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c89da-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="c89da-131">Request body</span></span>
<span data-ttu-id="c89da-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c89da-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c89da-133">応答</span><span class="sxs-lookup"><span data-stu-id="c89da-133">Response</span></span>
<span data-ttu-id="c89da-134">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationAssignment](../resources/educationassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c89da-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c89da-135">例</span><span class="sxs-lookup"><span data-stu-id="c89da-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c89da-136">要求</span><span class="sxs-lookup"><span data-stu-id="c89da-136">Request</span></span>
<span data-ttu-id="c89da-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c89da-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="c89da-138">応答</span><span class="sxs-lookup"><span data-stu-id="c89da-138">Response</span></span>
<span data-ttu-id="c89da-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c89da-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c89da-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c89da-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
