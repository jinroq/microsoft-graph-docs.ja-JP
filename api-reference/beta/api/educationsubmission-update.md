---
title: Educationsubmission を更新します。
description: 評価とフィードバックを提出書類に追加します。 教師だけでは、この操作を実行できます。 基本アクセス権はグレードのプロパティへのアクセス権がないと、評価やご意見を書き込むことができませんので注意してください。 このアクションでは、グレードと、受講生受講者へのフィードバックは解放されません。 教師では、受講者に返される成績データの明示的な解放アクションを実行する必要があります。
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 516940f9a6dd43460aa0ceb9b955c41dc89196c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828785"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="5710b-107">Educationsubmission を更新します。</span><span class="sxs-lookup"><span data-stu-id="5710b-107">Update educationsubmission</span></span>

> <span data-ttu-id="5710b-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5710b-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5710b-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5710b-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5710b-110">評価とフィードバックを提出書類に追加します。</span><span class="sxs-lookup"><span data-stu-id="5710b-110">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="5710b-111">教師だけでは、この操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="5710b-111">Only teachers can perform this operation.</span></span> <span data-ttu-id="5710b-112">基本アクセス権はグレードのプロパティへのアクセス権がないと、評価やご意見を書き込むことができませんので注意してください。</span><span class="sxs-lookup"><span data-stu-id="5710b-112">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="5710b-113">このアクションでは、グレードと、受講生受講者へのフィードバックは解放されません。</span><span class="sxs-lookup"><span data-stu-id="5710b-113">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="5710b-114">教師では、受講者に返される成績データの明示的な解放アクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5710b-114">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="5710b-115">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5710b-115">Permissions</span></span>
<span data-ttu-id="5710b-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5710b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5710b-118">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5710b-118">Permission type</span></span>      | <span data-ttu-id="5710b-119">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5710b-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5710b-120">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5710b-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="5710b-121">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5710b-121">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5710b-122">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5710b-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5710b-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5710b-123">Not supported.</span></span>   |
|<span data-ttu-id="5710b-124">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5710b-124">Application</span></span> | <span data-ttu-id="5710b-125">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5710b-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5710b-126">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5710b-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5710b-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5710b-127">Request headers</span></span>
| <span data-ttu-id="5710b-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5710b-128">Header</span></span>       | <span data-ttu-id="5710b-129">値</span><span class="sxs-lookup"><span data-stu-id="5710b-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5710b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5710b-130">Authorization</span></span>  | <span data-ttu-id="5710b-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5710b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5710b-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="5710b-133">Request body</span></span>
<span data-ttu-id="5710b-134">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5710b-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5710b-135">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="5710b-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5710b-136">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="5710b-136">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="5710b-137">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5710b-137">Property</span></span>     | <span data-ttu-id="5710b-138">種類</span><span class="sxs-lookup"><span data-stu-id="5710b-138">Type</span></span>   |<span data-ttu-id="5710b-139">説明</span><span class="sxs-lookup"><span data-stu-id="5710b-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5710b-140">feedback</span><span class="sxs-lookup"><span data-stu-id="5710b-140">feedback</span></span>|<span data-ttu-id="5710b-141">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="5710b-141">educationFeedback</span></span>||
|<span data-ttu-id="5710b-142">grade</span><span class="sxs-lookup"><span data-stu-id="5710b-142">grade</span></span>|<span data-ttu-id="5710b-143">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="5710b-143">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="5710b-144">応答</span><span class="sxs-lookup"><span data-stu-id="5710b-144">Response</span></span>
<span data-ttu-id="5710b-145">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[educationSubmission](../resources/educationsubmission.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5710b-145">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5710b-146">例</span><span class="sxs-lookup"><span data-stu-id="5710b-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5710b-147">要求</span><span class="sxs-lookup"><span data-stu-id="5710b-147">Request</span></span>
<span data-ttu-id="5710b-148">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5710b-148">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5710b-149">応答</span><span class="sxs-lookup"><span data-stu-id="5710b-149">Response</span></span>
<span data-ttu-id="5710b-150">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5710b-150">The following is an example of the response.</span></span> 

><span data-ttu-id="5710b-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5710b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
