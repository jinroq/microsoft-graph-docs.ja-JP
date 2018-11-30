---
title: EducationSubmission を取得します。
description: '特定の送信を取得します。 送信オブジェクトは、割り当ての受講者の作業を表します。 リソースに送信は、この作業が関連付けられています。 提出書類が割り当てられている学生だけを参照してくださいでき、提出書類を変更することができます。 教師には、すべての提出書類へのフル アクセスがあります。 '
ms.openlocfilehash: 016e8d2e04377ec24fa55ad940fb97364786f433
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070264"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="e83e4-107">EducationSubmission を取得します。</span><span class="sxs-lookup"><span data-stu-id="e83e4-107">Get educationSubmission</span></span>

> <span data-ttu-id="e83e4-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e83e4-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e83e4-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e83e4-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e83e4-110">特定の送信を取得します。</span><span class="sxs-lookup"><span data-stu-id="e83e4-110">Retrieve a particular submission.</span></span> <span data-ttu-id="e83e4-111">送信オブジェクトは、割り当ての受講者の作業を表します。</span><span class="sxs-lookup"><span data-stu-id="e83e4-111">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="e83e4-112">リソースに送信は、この作業が関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="e83e4-112">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="e83e4-113">提出書類が割り当てられている学生だけを参照してくださいでき、提出書類を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="e83e4-113">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="e83e4-114">教師には、すべての提出書類へのフル アクセスがあります。</span><span class="sxs-lookup"><span data-stu-id="e83e4-114">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="e83e4-115">グレードおよび教師からのフィードバックもこのオブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="e83e4-115">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="e83e4-116">教師だけでは、追加したり、成績やフィードバックを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="e83e4-116">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="e83e4-117">受講者は表示されません、評価やご意見、割り当てが解除されるまで。</span><span class="sxs-lookup"><span data-stu-id="e83e4-117">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="e83e4-118">基本アクセス権は評価とフィードバックが含まれていないが、それ以外のすべては。</span><span class="sxs-lookup"><span data-stu-id="e83e4-118">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="e83e4-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e83e4-119">Permissions</span></span>
<span data-ttu-id="e83e4-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e83e4-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e83e4-122">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e83e4-122">Permission type</span></span>      | <span data-ttu-id="e83e4-123">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e83e4-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e83e4-124">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e83e4-124">Delegated (work or school account)</span></span> |  <span data-ttu-id="e83e4-125">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e83e4-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="e83e4-126">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e83e4-126">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e83e4-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e83e4-127">Not supported.</span></span>  |
|<span data-ttu-id="e83e4-128">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e83e4-128">Application</span></span> | <span data-ttu-id="e83e4-129">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e83e4-129">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e83e4-130">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e83e4-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e83e4-131">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e83e4-131">Optional query parameters</span></span>
<span data-ttu-id="e83e4-132">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e83e4-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e83e4-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e83e4-133">Request headers</span></span>
| <span data-ttu-id="e83e4-134">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e83e4-134">Header</span></span>       | <span data-ttu-id="e83e4-135">値</span><span class="sxs-lookup"><span data-stu-id="e83e4-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e83e4-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="e83e4-136">Authorization</span></span>  | <span data-ttu-id="e83e4-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e83e4-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e83e4-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="e83e4-139">Request body</span></span>
<span data-ttu-id="e83e4-140">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e83e4-140">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e83e4-141">応答</span><span class="sxs-lookup"><span data-stu-id="e83e4-141">Response</span></span>
<span data-ttu-id="e83e4-142">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationSubmission](../resources/educationsubmission.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e83e4-142">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e83e4-143">例</span><span class="sxs-lookup"><span data-stu-id="e83e4-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e83e4-144">要求</span><span class="sxs-lookup"><span data-stu-id="e83e4-144">Request</span></span>
<span data-ttu-id="e83e4-145">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e83e4-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="e83e4-146">応答</span><span class="sxs-lookup"><span data-stu-id="e83e4-146">Response</span></span>
<span data-ttu-id="e83e4-147">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e83e4-147">The following is an example of the response.</span></span> 

><span data-ttu-id="e83e4-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e83e4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
    "feedback": {
      text: {
        "content": "Good work!",
        "contentType": "Text"
      },
      feedbackDateTime: "2014-01-01T00:00:00Z",
      feedbackBy: {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
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
        "userId": "13015"
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->