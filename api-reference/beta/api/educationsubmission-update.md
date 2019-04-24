---
title: educationsubmission の更新
description: 提出物にグレードとフィードバックを追加します。 この操作を実行できるのは教師だけです。 基本アクセス許可には、学年プロパティへのアクセス権がないため、グレードまたはフィードバックに書き込めないことに注意してください。 この操作では、学年とフィードバックが生徒にリリースされることはありません。 教師は、成績データが学生に返されるように、明示的な release アクションを受ける必要があります。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c420d2c6e512d8fed0d713340fea482b0888ca1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464851"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="1ac12-107">educationsubmission の更新</span><span class="sxs-lookup"><span data-stu-id="1ac12-107">Update educationsubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ac12-108">提出物にグレードとフィードバックを追加します。</span><span class="sxs-lookup"><span data-stu-id="1ac12-108">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="1ac12-109">この操作を実行できるのは教師だけです。</span><span class="sxs-lookup"><span data-stu-id="1ac12-109">Only teachers can perform this operation.</span></span> <span data-ttu-id="1ac12-110">基本アクセス許可には、学年プロパティへのアクセス権がないため、グレードまたはフィードバックに書き込めないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="1ac12-110">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="1ac12-111">この操作では、学年とフィードバックが生徒にリリースされることはありません。</span><span class="sxs-lookup"><span data-stu-id="1ac12-111">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="1ac12-112">教師は、成績データが学生に返されるように、明示的な release アクションを受ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ac12-112">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ac12-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ac12-113">Permissions</span></span>
<span data-ttu-id="1ac12-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ac12-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ac12-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ac12-116">Permission type</span></span>      | <span data-ttu-id="1ac12-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ac12-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ac12-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ac12-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="1ac12-119">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ac12-119">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1ac12-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ac12-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ac12-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ac12-121">Not supported.</span></span>   |
|<span data-ttu-id="1ac12-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ac12-122">Application</span></span> | <span data-ttu-id="1ac12-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ac12-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1ac12-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ac12-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1ac12-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ac12-125">Request headers</span></span>
| <span data-ttu-id="1ac12-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ac12-126">Header</span></span>       | <span data-ttu-id="1ac12-127">値</span><span class="sxs-lookup"><span data-stu-id="1ac12-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ac12-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ac12-128">Authorization</span></span>  | <span data-ttu-id="1ac12-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1ac12-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ac12-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ac12-131">Request body</span></span>
<span data-ttu-id="1ac12-132">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ac12-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1ac12-133">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="1ac12-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1ac12-134">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1ac12-134">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="1ac12-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ac12-135">Property</span></span>     | <span data-ttu-id="1ac12-136">型</span><span class="sxs-lookup"><span data-stu-id="1ac12-136">Type</span></span>   |<span data-ttu-id="1ac12-137">説明</span><span class="sxs-lookup"><span data-stu-id="1ac12-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ac12-138">feedback</span><span class="sxs-lookup"><span data-stu-id="1ac12-138">feedback</span></span>|<span data-ttu-id="1ac12-139">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="1ac12-139">educationFeedback</span></span>||
|<span data-ttu-id="1ac12-140">grade</span><span class="sxs-lookup"><span data-stu-id="1ac12-140">grade</span></span>|<span data-ttu-id="1ac12-141">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="1ac12-141">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="1ac12-142">応答</span><span class="sxs-lookup"><span data-stu-id="1ac12-142">Response</span></span>
<span data-ttu-id="1ac12-143">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[educationSubmission](../resources/educationsubmission.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1ac12-143">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ac12-144">例</span><span class="sxs-lookup"><span data-stu-id="1ac12-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ac12-145">要求</span><span class="sxs-lookup"><span data-stu-id="1ac12-145">Request</span></span>
<span data-ttu-id="1ac12-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ac12-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationsubmission"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7
Content-type: application/json
Content-length: 658

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
      "@odata.type": "microsoft.graph.identitySet"
    },
    "gradedDateTime": "2014-01-01T00:00:00Z",
    "@odata.type": "microsoft.graph.educationAssignmentGrade"
  }
}
```
##### <a name="response"></a><span data-ttu-id="1ac12-147">応答</span><span class="sxs-lookup"><span data-stu-id="1ac12-147">Response</span></span>
<span data-ttu-id="1ac12-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1ac12-148">The following is an example of the response.</span></span> 

><span data-ttu-id="1ac12-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1ac12-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1217

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
          "@odata.type": "microsoft.graph.identitySet"
        },
        "gradedDateTime": "2014-01-01T00:00:00Z",
        "@odata.type": "microsoft.graph.educationAssignmentGrade"
  },
  "id": "850f51b7",
  "recipient": {
    userId:"dsfewsddf",
    "@odata.type": "#microsoft.graph.educationSubmissionRecipient"
  },
  "releasedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "releasedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "String",
  "status": "completed",
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
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
