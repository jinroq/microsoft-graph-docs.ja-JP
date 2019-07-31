---
title: EducationAssignment を取得する
description: " 教師は、クラス内のすべての割り当てを表示できます。"
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 22db7dc1c85de37c991078ba4c7b718c2e2dbc52
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955668"
---
# <a name="get-educationassignment"></a><span data-ttu-id="f7f0c-103">EducationAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="f7f0c-103">Get educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7f0c-104">割り当てのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-104">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="f7f0c-105">受講者に割り当てられている割り当てのみ表示できます。教師は、クラス内のすべての割り当てを表示できます。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-105">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7f0c-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7f0c-106">Permissions</span></span>
<span data-ttu-id="f7f0c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f7f0c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f7f0c-109">Permission type</span></span>      | <span data-ttu-id="f7f0c-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f7f0c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7f0c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f7f0c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7f0c-112">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="f7f0c-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="f7f0c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f7f0c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f7f0c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-114">Not supported.</span></span>  |
|<span data-ttu-id="f7f0c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f7f0c-115">Application</span></span> | <span data-ttu-id="f7f0c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f7f0c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f7f0c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7f0c-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f7f0c-118">Optional query parameters</span></span>
<span data-ttu-id="f7f0c-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7f0c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7f0c-120">Request headers</span></span>
| <span data-ttu-id="f7f0c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7f0c-121">Header</span></span>       | <span data-ttu-id="f7f0c-122">値</span><span class="sxs-lookup"><span data-stu-id="f7f0c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7f0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7f0c-123">Authorization</span></span>  | <span data-ttu-id="f7f0c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7f0c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f7f0c-126">Request body</span></span>
<span data-ttu-id="f7f0c-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7f0c-128">応答</span><span class="sxs-lookup"><span data-stu-id="f7f0c-128">Response</span></span>
<span data-ttu-id="f7f0c-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationAssignment](../resources/educationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-129">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7f0c-130">例</span><span class="sxs-lookup"><span data-stu-id="f7f0c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7f0c-131">要求</span><span class="sxs-lookup"><span data-stu-id="f7f0c-131">Request</span></span>
<span data-ttu-id="f7f0c-132">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="f7f0c-133">応答</span><span class="sxs-lookup"><span data-stu-id="f7f0c-133">Response</span></span>
<span data-ttu-id="f7f0c-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-134">The following is an example of the response.</span></span> 

><span data-ttu-id="f7f0c-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f7f0c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
