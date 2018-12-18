---
title: ボックスの一覧の送信
description: この割り当てに関連付けられているすべての提出書類の一覧を表示します。 教師は、学生はそれらに関連付けられている送信しか取得中に、すべての提出書類を取得できます。
author: dipakboyed
ms.openlocfilehash: ac7bd47b4cbc4549f38239c4a68504bd20b3a2e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308429"
---
# <a name="list-submissions"></a><span data-ttu-id="594a5-104">ボックスの一覧の送信</span><span class="sxs-lookup"><span data-stu-id="594a5-104">List submissions</span></span>

> <span data-ttu-id="594a5-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="594a5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="594a5-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="594a5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="594a5-107">この割り当てに関連付けられているすべての提出書類の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="594a5-107">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="594a5-108">教師は、学生はそれらに関連付けられている送信しか取得中に、すべての提出書類を取得できます。</span><span class="sxs-lookup"><span data-stu-id="594a5-108">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="594a5-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="594a5-109">Permissions</span></span>
<span data-ttu-id="594a5-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="594a5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="594a5-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="594a5-112">Permission type</span></span>      | <span data-ttu-id="594a5-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="594a5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="594a5-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="594a5-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="594a5-115">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="594a5-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="594a5-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="594a5-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="594a5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="594a5-117">Not supported.</span></span>  |
|<span data-ttu-id="594a5-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="594a5-118">Application</span></span> | <span data-ttu-id="594a5-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="594a5-119">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="594a5-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="594a5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="594a5-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="594a5-121">Optional query parameters</span></span>
<span data-ttu-id="594a5-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="594a5-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="594a5-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="594a5-123">Request headers</span></span>
| <span data-ttu-id="594a5-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="594a5-124">Header</span></span>       | <span data-ttu-id="594a5-125">値</span><span class="sxs-lookup"><span data-stu-id="594a5-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="594a5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="594a5-126">Authorization</span></span>  | <span data-ttu-id="594a5-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="594a5-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="594a5-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="594a5-129">Request body</span></span>
<span data-ttu-id="594a5-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="594a5-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="594a5-131">応答</span><span class="sxs-lookup"><span data-stu-id="594a5-131">Response</span></span>
<span data-ttu-id="594a5-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationSubmission](../resources/educationsubmission.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="594a5-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="594a5-133">例</span><span class="sxs-lookup"><span data-stu-id="594a5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="594a5-134">要求</span><span class="sxs-lookup"><span data-stu-id="594a5-134">Request</span></span>
<span data-ttu-id="594a5-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="594a5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="594a5-136">応答</span><span class="sxs-lookup"><span data-stu-id="594a5-136">Response</span></span>
<span data-ttu-id="594a5-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="594a5-137">The following is an example of the response.</span></span> 

><span data-ttu-id="594a5-138">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="594a5-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="594a5-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="594a5-139">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->