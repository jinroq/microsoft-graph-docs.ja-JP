---
title: EducationAssignment を取得します。
description: " 先生は、クラスのすべての割り当てを確認できます。"
author: dipakboyed
ms.openlocfilehash: 384f99a48340e51c6d919b96471f31c9fbff27a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341910"
---
# <a name="get-educationassignment"></a><span data-ttu-id="d185d-103">EducationAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="d185d-103">Get educationAssignment</span></span>

> <span data-ttu-id="d185d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d185d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d185d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d185d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d185d-106">プロパティとリレーションシップの割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="d185d-106">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="d185d-107">受講者はそれに割り当てられた割り当てのみを参照できます。先生は、クラスのすべての割り当てを確認できます。</span><span class="sxs-lookup"><span data-stu-id="d185d-107">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="d185d-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d185d-108">Permissions</span></span>
<span data-ttu-id="d185d-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d185d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d185d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d185d-111">Permission type</span></span>      | <span data-ttu-id="d185d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d185d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d185d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d185d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d185d-114">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d185d-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="d185d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d185d-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d185d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d185d-116">Not supported.</span></span>  |
|<span data-ttu-id="d185d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d185d-117">Application</span></span> | <span data-ttu-id="d185d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d185d-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="d185d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d185d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d185d-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d185d-120">Optional query parameters</span></span>
<span data-ttu-id="d185d-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d185d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d185d-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d185d-122">Request headers</span></span>
| <span data-ttu-id="d185d-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d185d-123">Header</span></span>       | <span data-ttu-id="d185d-124">値</span><span class="sxs-lookup"><span data-stu-id="d185d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d185d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d185d-125">Authorization</span></span>  | <span data-ttu-id="d185d-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d185d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d185d-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d185d-128">Request body</span></span>
<span data-ttu-id="d185d-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d185d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d185d-130">応答</span><span class="sxs-lookup"><span data-stu-id="d185d-130">Response</span></span>
<span data-ttu-id="d185d-131">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationAssignment](../resources/educationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d185d-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d185d-132">例</span><span class="sxs-lookup"><span data-stu-id="d185d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d185d-133">要求</span><span class="sxs-lookup"><span data-stu-id="d185d-133">Request</span></span>
<span data-ttu-id="d185d-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d185d-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="d185d-135">応答</span><span class="sxs-lookup"><span data-stu-id="d185d-135">Response</span></span>
<span data-ttu-id="d185d-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d185d-136">The following is an example of the response.</span></span> 

><span data-ttu-id="d185d-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d185d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->