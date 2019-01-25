---
title: EducationSubmission を取得します。
description: '特定の送信を取得します。 送信オブジェクトは、割り当ての受講者の作業を表します。 リソースに送信は、この作業が関連付けられています。 提出書類が割り当てられている学生だけを参照してくださいでき、提出書類を変更することができます。 教師には、すべての提出書類へのフル アクセスがあります。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d0542bec537b8317a46e98c215768f5228f9a07c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511955"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="7c154-107">EducationSubmission を取得します。</span><span class="sxs-lookup"><span data-stu-id="7c154-107">Get educationSubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c154-108">特定の送信を取得します。</span><span class="sxs-lookup"><span data-stu-id="7c154-108">Retrieve a particular submission.</span></span> <span data-ttu-id="7c154-109">送信オブジェクトは、割り当ての受講者の作業を表します。</span><span class="sxs-lookup"><span data-stu-id="7c154-109">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="7c154-110">リソースに送信は、この作業が関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="7c154-110">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="7c154-111">提出書類が割り当てられている学生だけを参照してくださいでき、提出書類を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="7c154-111">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="7c154-112">教師には、すべての提出書類へのフル アクセスがあります。</span><span class="sxs-lookup"><span data-stu-id="7c154-112">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="7c154-113">グレードおよび教師からのフィードバックもこのオブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="7c154-113">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="7c154-114">教師だけでは、追加したり、成績やフィードバックを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="7c154-114">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="7c154-115">受講者は表示されません、評価やご意見、割り当てが解除されるまで。</span><span class="sxs-lookup"><span data-stu-id="7c154-115">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="7c154-116">基本アクセス権は評価とフィードバックが含まれていないが、それ以外のすべては。</span><span class="sxs-lookup"><span data-stu-id="7c154-116">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c154-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7c154-117">Permissions</span></span>
<span data-ttu-id="7c154-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c154-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c154-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c154-120">Permission type</span></span>      | <span data-ttu-id="7c154-121">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c154-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c154-122">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c154-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="7c154-123">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7c154-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="7c154-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c154-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7c154-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c154-125">Not supported.</span></span>  |
|<span data-ttu-id="7c154-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c154-126">Application</span></span> | <span data-ttu-id="7c154-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c154-127">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7c154-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c154-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7c154-129">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7c154-129">Optional query parameters</span></span>
<span data-ttu-id="7c154-130">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7c154-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7c154-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c154-131">Request headers</span></span>
| <span data-ttu-id="7c154-132">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c154-132">Header</span></span>       | <span data-ttu-id="7c154-133">値</span><span class="sxs-lookup"><span data-stu-id="7c154-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c154-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c154-134">Authorization</span></span>  | <span data-ttu-id="7c154-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7c154-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c154-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c154-137">Request body</span></span>
<span data-ttu-id="7c154-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7c154-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7c154-139">応答</span><span class="sxs-lookup"><span data-stu-id="7c154-139">Response</span></span>
<span data-ttu-id="7c154-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationSubmission](../resources/educationsubmission.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7c154-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7c154-141">例</span><span class="sxs-lookup"><span data-stu-id="7c154-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7c154-142">要求</span><span class="sxs-lookup"><span data-stu-id="7c154-142">Request</span></span>
<span data-ttu-id="7c154-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c154-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="7c154-144">応答</span><span class="sxs-lookup"><span data-stu-id="7c154-144">Response</span></span>
<span data-ttu-id="7c154-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7c154-145">The following is an example of the response.</span></span> 

><span data-ttu-id="7c154-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7c154-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
