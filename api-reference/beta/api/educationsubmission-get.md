---
title: educationSubmission を取得する
description: '特定の送信を取得します。 送信オブジェクトは、割り当てに対する学生の作業を表します。 送信に関連付けられているリソースは、この作業を表します。 提出物が割り当てられている受講者のみが、提出物を表示および変更できます。 教師は、すべての送信にフルアクセスできます。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 97cdc45c8af271d0996ea5edabf145f239162210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325177"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="f517c-107">educationSubmission を取得する</span><span class="sxs-lookup"><span data-stu-id="f517c-107">Get educationSubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f517c-108">特定の送信を取得します。</span><span class="sxs-lookup"><span data-stu-id="f517c-108">Retrieve a particular submission.</span></span> <span data-ttu-id="f517c-109">送信オブジェクトは、割り当てに対する学生の作業を表します。</span><span class="sxs-lookup"><span data-stu-id="f517c-109">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="f517c-110">送信に関連付けられているリソースは、この作業を表します。</span><span class="sxs-lookup"><span data-stu-id="f517c-110">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="f517c-111">提出物が割り当てられている受講者のみが、提出物を表示および変更できます。</span><span class="sxs-lookup"><span data-stu-id="f517c-111">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="f517c-112">教師は、すべての送信にフルアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f517c-112">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="f517c-113">教師からの評価とフィードバックも、このオブジェクトの一部です。</span><span class="sxs-lookup"><span data-stu-id="f517c-113">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="f517c-114">教師のみが、成績とフィードバックを追加または変更できます。</span><span class="sxs-lookup"><span data-stu-id="f517c-114">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="f517c-115">課題がリリースされるまで、学生には成績またはフィードバックは表示されません。</span><span class="sxs-lookup"><span data-stu-id="f517c-115">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="f517c-116">基本的なアクセス許可には、成績とフィードバックは含まれませんが、それ以外はすべて含まれます。</span><span class="sxs-lookup"><span data-stu-id="f517c-116">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="f517c-117">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f517c-117">Permissions</span></span>
<span data-ttu-id="f517c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f517c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f517c-120">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f517c-120">Permission type</span></span>      | <span data-ttu-id="f517c-121">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f517c-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f517c-122">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f517c-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="f517c-123">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="f517c-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="f517c-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f517c-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f517c-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f517c-125">Not supported.</span></span>  |
|<span data-ttu-id="f517c-126">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f517c-126">Application</span></span> | <span data-ttu-id="f517c-127">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f517c-127">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f517c-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f517c-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f517c-129">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f517c-129">Optional query parameters</span></span>
<span data-ttu-id="f517c-130">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f517c-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f517c-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f517c-131">Request headers</span></span>
| <span data-ttu-id="f517c-132">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f517c-132">Header</span></span>       | <span data-ttu-id="f517c-133">値</span><span class="sxs-lookup"><span data-stu-id="f517c-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f517c-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f517c-134">Authorization</span></span>  | <span data-ttu-id="f517c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f517c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f517c-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="f517c-137">Request body</span></span>
<span data-ttu-id="f517c-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f517c-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f517c-139">応答</span><span class="sxs-lookup"><span data-stu-id="f517c-139">Response</span></span>
<span data-ttu-id="f517c-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSubmission](../resources/educationsubmission.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f517c-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f517c-141">例</span><span class="sxs-lookup"><span data-stu-id="f517c-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f517c-142">要求</span><span class="sxs-lookup"><span data-stu-id="f517c-142">Request</span></span>
<span data-ttu-id="f517c-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f517c-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="f517c-144">応答</span><span class="sxs-lookup"><span data-stu-id="f517c-144">Response</span></span>
<span data-ttu-id="f517c-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f517c-145">The following is an example of the response.</span></span> 

><span data-ttu-id="f517c-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f517c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
