---
title: 割り当てを一覧表示する
description: assignment オブジェクトのリストを取得します。 教師は、クラスのすべての assignment オブジェクトを表示することができます。 受講者には、割り当てられている割り当てのみが表示されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7cd47c61d4958d42ce099396147d421a6555041b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457873"
---
# <a name="list-assignments"></a><span data-ttu-id="61def-105">割り当てを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="61def-105">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61def-106">assignment オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="61def-106">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="61def-107">教師は、クラスのすべての assignment オブジェクトを表示することができます。</span><span class="sxs-lookup"><span data-stu-id="61def-107">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="61def-108">受講者には、割り当てられている割り当てのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="61def-108">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="61def-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="61def-109">Permissions</span></span>
<span data-ttu-id="61def-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61def-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61def-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61def-112">Permission type</span></span>      | <span data-ttu-id="61def-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="61def-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61def-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61def-114">Delegated (work or school account)</span></span> | <span data-ttu-id="61def-115">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="61def-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="61def-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61def-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="61def-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61def-117">Not supported.</span></span>  |
|<span data-ttu-id="61def-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61def-118">Application</span></span> | <span data-ttu-id="61def-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61def-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="61def-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61def-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="61def-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="61def-121">Optional query parameters</span></span>
<span data-ttu-id="61def-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="61def-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61def-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61def-123">Request headers</span></span>
| <span data-ttu-id="61def-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61def-124">Header</span></span>       | <span data-ttu-id="61def-125">値</span><span class="sxs-lookup"><span data-stu-id="61def-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="61def-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="61def-126">Authorization</span></span>  | <span data-ttu-id="61def-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="61def-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="61def-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="61def-129">Request body</span></span>
<span data-ttu-id="61def-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="61def-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="61def-131">応答</span><span class="sxs-lookup"><span data-stu-id="61def-131">Response</span></span>
<span data-ttu-id="61def-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationAssignment](../resources/educationassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="61def-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61def-133">例</span><span class="sxs-lookup"><span data-stu-id="61def-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="61def-134">要求</span><span class="sxs-lookup"><span data-stu-id="61def-134">Request</span></span>
<span data-ttu-id="61def-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61def-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="61def-136">応答</span><span class="sxs-lookup"><span data-stu-id="61def-136">Response</span></span>
<span data-ttu-id="61def-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="61def-137">The following is an example of the response.</span></span> 

><span data-ttu-id="61def-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="61def-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
