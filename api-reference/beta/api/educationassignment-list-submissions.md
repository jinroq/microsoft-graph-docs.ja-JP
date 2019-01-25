---
title: ボックスの一覧の送信
description: この割り当てに関連付けられているすべての提出書類の一覧を表示します。 教師は、学生はそれらに関連付けられている送信しか取得中に、すべての提出書類を取得できます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47088cb7a4290827ce75e35d3ac705b31addefac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510639"
---
# <a name="list-submissions"></a><span data-ttu-id="abe76-104">ボックスの一覧の送信</span><span class="sxs-lookup"><span data-stu-id="abe76-104">List submissions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe76-105">この割り当てに関連付けられているすべての提出書類の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="abe76-105">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="abe76-106">教師は、学生はそれらに関連付けられている送信しか取得中に、すべての提出書類を取得できます。</span><span class="sxs-lookup"><span data-stu-id="abe76-106">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="abe76-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="abe76-107">Permissions</span></span>
<span data-ttu-id="abe76-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abe76-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abe76-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abe76-110">Permission type</span></span>      | <span data-ttu-id="abe76-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="abe76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abe76-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="abe76-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="abe76-113">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="abe76-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="abe76-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="abe76-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="abe76-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abe76-115">Not supported.</span></span>  |
|<span data-ttu-id="abe76-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abe76-116">Application</span></span> | <span data-ttu-id="abe76-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abe76-117">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="abe76-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="abe76-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="abe76-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="abe76-119">Optional query parameters</span></span>
<span data-ttu-id="abe76-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="abe76-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abe76-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abe76-121">Request headers</span></span>
| <span data-ttu-id="abe76-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abe76-122">Header</span></span>       | <span data-ttu-id="abe76-123">値</span><span class="sxs-lookup"><span data-stu-id="abe76-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="abe76-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="abe76-124">Authorization</span></span>  | <span data-ttu-id="abe76-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="abe76-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="abe76-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="abe76-127">Request body</span></span>
<span data-ttu-id="abe76-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="abe76-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="abe76-129">応答</span><span class="sxs-lookup"><span data-stu-id="abe76-129">Response</span></span>
<span data-ttu-id="abe76-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationSubmission](../resources/educationsubmission.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="abe76-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="abe76-131">例</span><span class="sxs-lookup"><span data-stu-id="abe76-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="abe76-132">要求</span><span class="sxs-lookup"><span data-stu-id="abe76-132">Request</span></span>
<span data-ttu-id="abe76-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="abe76-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="abe76-134">応答</span><span class="sxs-lookup"><span data-stu-id="abe76-134">Response</span></span>
<span data-ttu-id="abe76-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="abe76-135">The following is an example of the response.</span></span> 

><span data-ttu-id="abe76-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="abe76-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="abe76-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="abe76-137">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "feedback": {
        "text": {
          "content": "Good work!",
          "contentType": "Text"
        },
        "feedbackDateTime": "2014-01-01T00:00:00Z",
        "feedbackBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
        },
        "@odata.type": "microsoft.graph.educationFeedback"
        },
      "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
        "gradedDateTime": "2014-01-01T00:00:00Z"
      },
      "id": "33223",
      "recipient": {
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-submissions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
