---
title: Educationsubmission を更新します。
description: 評価とフィードバックを提出書類に追加します。 教師だけでは、この操作を実行できます。 基本アクセス権はグレードのプロパティへのアクセス権がないと、評価やご意見を書き込むことができませんので注意してください。 このアクションでは、グレードと、受講生受講者へのフィードバックは解放されません。 教師では、受講者に返される成績データの明示的な解放アクションを実行する必要があります。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c420d2c6e512d8fed0d713340fea482b0888ca1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526117"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="19438-107">Educationsubmission を更新します。</span><span class="sxs-lookup"><span data-stu-id="19438-107">Update educationsubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19438-108">評価とフィードバックを提出書類に追加します。</span><span class="sxs-lookup"><span data-stu-id="19438-108">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="19438-109">教師だけでは、この操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="19438-109">Only teachers can perform this operation.</span></span> <span data-ttu-id="19438-110">基本アクセス権はグレードのプロパティへのアクセス権がないと、評価やご意見を書き込むことができませんので注意してください。</span><span class="sxs-lookup"><span data-stu-id="19438-110">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="19438-111">このアクションでは、グレードと、受講生受講者へのフィードバックは解放されません。</span><span class="sxs-lookup"><span data-stu-id="19438-111">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="19438-112">教師では、受講者に返される成績データの明示的な解放アクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="19438-112">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="19438-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19438-113">Permissions</span></span>
<span data-ttu-id="19438-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19438-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19438-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19438-116">Permission type</span></span>      | <span data-ttu-id="19438-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19438-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19438-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19438-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="19438-119">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19438-119">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="19438-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19438-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19438-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19438-121">Not supported.</span></span>   |
|<span data-ttu-id="19438-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19438-122">Application</span></span> | <span data-ttu-id="19438-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19438-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="19438-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19438-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="19438-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19438-125">Request headers</span></span>
| <span data-ttu-id="19438-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19438-126">Header</span></span>       | <span data-ttu-id="19438-127">値</span><span class="sxs-lookup"><span data-stu-id="19438-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="19438-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="19438-128">Authorization</span></span>  | <span data-ttu-id="19438-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19438-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="19438-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="19438-131">Request body</span></span>
<span data-ttu-id="19438-132">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="19438-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="19438-133">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="19438-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="19438-134">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="19438-134">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="19438-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19438-135">Property</span></span>     | <span data-ttu-id="19438-136">型</span><span class="sxs-lookup"><span data-stu-id="19438-136">Type</span></span>   |<span data-ttu-id="19438-137">説明</span><span class="sxs-lookup"><span data-stu-id="19438-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19438-138">feedback</span><span class="sxs-lookup"><span data-stu-id="19438-138">feedback</span></span>|<span data-ttu-id="19438-139">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="19438-139">educationFeedback</span></span>||
|<span data-ttu-id="19438-140">grade</span><span class="sxs-lookup"><span data-stu-id="19438-140">grade</span></span>|<span data-ttu-id="19438-141">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="19438-141">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="19438-142">応答</span><span class="sxs-lookup"><span data-stu-id="19438-142">Response</span></span>
<span data-ttu-id="19438-143">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[educationSubmission](../resources/educationsubmission.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="19438-143">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19438-144">例</span><span class="sxs-lookup"><span data-stu-id="19438-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19438-145">要求</span><span class="sxs-lookup"><span data-stu-id="19438-145">Request</span></span>
<span data-ttu-id="19438-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19438-146">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="19438-147">応答</span><span class="sxs-lookup"><span data-stu-id="19438-147">Response</span></span>
<span data-ttu-id="19438-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19438-148">The following is an example of the response.</span></span> 

><span data-ttu-id="19438-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="19438-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
