---
title: 送信の一覧表示
description: この割り当てに関連付けられているすべての送信を一覧表示します。 教師は、すべての送信を取得できますが、学生は自分が関連付けられている発信のみを取得できます。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 236c5dc88a50ad537f2142cc3a8e8dc5084c2c5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955649"
---
# <a name="list-submissions"></a><span data-ttu-id="b9c52-104">送信の一覧表示</span><span class="sxs-lookup"><span data-stu-id="b9c52-104">List submissions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9c52-105">この割り当てに関連付けられているすべての送信を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="b9c52-105">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="b9c52-106">教師は、すべての送信を取得できますが、学生は自分が関連付けられている発信のみを取得できます。</span><span class="sxs-lookup"><span data-stu-id="b9c52-106">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9c52-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b9c52-107">Permissions</span></span>
<span data-ttu-id="b9c52-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9c52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c52-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9c52-110">Permission type</span></span>      | <span data-ttu-id="b9c52-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9c52-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9c52-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9c52-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="b9c52-113">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="b9c52-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b9c52-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9c52-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b9c52-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9c52-115">Not supported.</span></span>  |
|<span data-ttu-id="b9c52-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9c52-116">Application</span></span> | <span data-ttu-id="b9c52-117">サポートされません。</span><span class="sxs-lookup"><span data-stu-id="b9c52-117">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b9c52-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9c52-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9c52-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b9c52-119">Optional query parameters</span></span>
<span data-ttu-id="b9c52-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b9c52-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9c52-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9c52-121">Request headers</span></span>
| <span data-ttu-id="b9c52-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9c52-122">Header</span></span>       | <span data-ttu-id="b9c52-123">値</span><span class="sxs-lookup"><span data-stu-id="b9c52-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9c52-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c52-124">Authorization</span></span>  | <span data-ttu-id="b9c52-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b9c52-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9c52-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9c52-127">Request body</span></span>
<span data-ttu-id="b9c52-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b9c52-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b9c52-129">応答</span><span class="sxs-lookup"><span data-stu-id="b9c52-129">Response</span></span>
<span data-ttu-id="b9c52-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSubmission](../resources/educationsubmission.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b9c52-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9c52-131">例</span><span class="sxs-lookup"><span data-stu-id="b9c52-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9c52-132">要求</span><span class="sxs-lookup"><span data-stu-id="b9c52-132">Request</span></span>
<span data-ttu-id="b9c52-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9c52-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="b9c52-134">応答</span><span class="sxs-lookup"><span data-stu-id="b9c52-134">Response</span></span>
<span data-ttu-id="b9c52-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9c52-135">The following is an example of the response.</span></span> 

><span data-ttu-id="b9c52-136">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="b9c52-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b9c52-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b9c52-137">All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
