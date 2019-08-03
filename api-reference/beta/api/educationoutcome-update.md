---
title: EducationOutcome の更新
description: EducationOutcome オブジェクトのプロパティを更新します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2c7b85d3456927e6a63f61f11722dfe8eccf270e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173182"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="89389-103">Educationoutcome の更新</span><span class="sxs-lookup"><span data-stu-id="89389-103">Update educationoutcome</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89389-104">[EducationOutcome](../resources/educationoutcome.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="89389-104">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89389-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89389-105">Permissions</span></span>

<span data-ttu-id="89389-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89389-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89389-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89389-108">Permission type</span></span>                        | <span data-ttu-id="89389-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89389-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89389-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89389-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="89389-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="89389-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="89389-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89389-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89389-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89389-113">Not supported.</span></span> |
| <span data-ttu-id="89389-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89389-114">Application</span></span>                            | <span data-ttu-id="89389-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89389-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89389-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89389-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="89389-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89389-117">Request headers</span></span>

| <span data-ttu-id="89389-118">名前</span><span class="sxs-lookup"><span data-stu-id="89389-118">Name</span></span>       | <span data-ttu-id="89389-119">説明</span><span class="sxs-lookup"><span data-stu-id="89389-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="89389-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="89389-120">Authorization</span></span> | <span data-ttu-id="89389-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="89389-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="89389-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="89389-122">Request body</span></span>

<span data-ttu-id="89389-123">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="89389-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="89389-124">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="89389-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="89389-125">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="89389-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="89389-126">EducationOutcome オブジェクトは、次の派生型のいずれかになります。 **educationPointsOutcome**、 **educationFeedbackOutcome**、または**educationRubricOutcome**。</span><span class="sxs-lookup"><span data-stu-id="89389-126">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="89389-127">パッチが適用されている結果の種類に関連する特定のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="89389-127">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="89389-128">すべての派生結果の種類には、その種類の結果に適した正規のプロパティと "発行済み" プロパティがあります。たとえば、**ポイント**と**publishedpoints**、**フィードバック**、 **publishedpoints**などです。</span><span class="sxs-lookup"><span data-stu-id="89389-128">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="89389-129">"発行済み" プロパティは更新しません。内部で使用します。</span><span class="sxs-lookup"><span data-stu-id="89389-129">Do not update the "published" property; it is for internal use.</span></span> <span data-ttu-id="89389-130">たとえば、 **educationPointsOutcome**にポイントを割り当てるには、 **points**プロパティを更新します。ただし、 **publishedpoints**は更新しません。</span><span class="sxs-lookup"><span data-stu-id="89389-130">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but do not update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="89389-131">応答</span><span class="sxs-lookup"><span data-stu-id="89389-131">Response</span></span>

<span data-ttu-id="89389-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[educationOutcome](../resources/educationoutcome.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89389-132">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89389-133">例</span><span class="sxs-lookup"><span data-stu-id="89389-133">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="89389-134">例 1: フィードバック結果を更新する</span><span class="sxs-lookup"><span data-stu-id="89389-134">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="89389-135">要求</span><span class="sxs-lookup"><span data-stu-id="89389-135">Request</span></span>

<span data-ttu-id="89389-136">フィードバック結果を更新する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89389-136">The following is an example of the request for updating a feedback outcome.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationfeedbackoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationFeedbackOutcome",
    "feedback":{
        "text":{
            "content":"This is feedback for the assignment as a whole.",
            "contentType":"text"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="89389-137">応答</span><span class="sxs-lookup"><span data-stu-id="89389-137">Response</span></span>

<span data-ttu-id="89389-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89389-138">The following is an example of the response.</span></span>

> <span data-ttu-id="89389-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="89389-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFeedbackOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
    "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
    "lastModifiedBy": {
        "user": {
            "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
        }
    },
    "feedback": {
        "feedbackDateTime": "2019-07-31T21:10:30.3231461Z",
        "text": {
            "content": "This is feedback for the assignment as a whole.",
            "contentType": "text"
        },
        "feedbackBy": {
            "user": {
                "id": "9391878d-903c-406c-bb1c-0f17d00fd878",
            }
        }
    }
}
```

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="89389-141">例 2: 点の結果を更新する</span><span class="sxs-lookup"><span data-stu-id="89389-141">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="89389-142">要求</span><span class="sxs-lookup"><span data-stu-id="89389-142">Request</span></span>

<span data-ttu-id="89389-143">次に示すのは、ポイントの結果を更新する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89389-143">The following is an example of the request for updating a points outcome.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationpointsoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "points":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGrade",
        "points":85.0
    }
}
```

#### <a name="response"></a><span data-ttu-id="89389-144">応答</span><span class="sxs-lookup"><span data-stu-id="89389-144">Response</span></span>

<span data-ttu-id="89389-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89389-145">The following is an example of the response.</span></span>

> <span data-ttu-id="89389-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="89389-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPointsOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "id":"ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
    "lastModifiedBy":{
        "user":{
            "id":"9391878d-903c-406c-bb1c-0f17d00fd878"
        }
    },
    "points":{
        "gradedDateTime":"2019-07-15T22:35:48.2429387Z",
        "points":85.0,
        "gradedBy":{
            "user":{
                "id":"9391878d-903c-406c-bb1c-0f17d00fd878"
            }
        }
    }
}
```

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="89389-148">例 3: 更新プログラムを更新する</span><span class="sxs-lookup"><span data-stu-id="89389-148">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="89389-149">要求</span><span class="sxs-lookup"><span data-stu-id="89389-149">Request</span></span>

<span data-ttu-id="89389-150">次に示すのは、このような場合に、このような結果を更新する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89389-150">The following is an example of the request for updating a rubric outcome.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationRubricOutcome",
    "rubricQualityFeedback":[
        {
            "qualityId":"9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "feedback":{
                "content":"This is feedback specific to the first quality of the rubric.",
                "contentType":"text"
            }
        },
        {
            "qualityId":"d2331fb2-2761-402e-8de6-93e0afaa076e",
            "feedback":{
                "content":"This is feedback specific to the second quality of the rubric.",
                "contentType":"text"
            }
        }
    ],
    "rubricQualitySelectedLevels":[
        {
            "qualityId":"9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "columnId":"4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        {
            "qualityId":"d2331fb2-2761-402e-8de6-93e0afaa076e",
            "columnId":"aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="89389-151">応答</span><span class="sxs-lookup"><span data-stu-id="89389-151">Response</span></span>

<span data-ttu-id="89389-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89389-152">The following is an example of the response.</span></span>

> <span data-ttu-id="89389-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="89389-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPointsOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.type": "#microsoft.graph.educationRubricOutcome",
    "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
    "rubricQualityFeedback": [
        {
            "qualityId": "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "feedback": {
                "content": "This is feedback specific to the first quality of the rubric.",
                "contentType": "text"
            }
        },
        {
            "qualityId": "d2331fb2-2761-402e-8de6-93e0afaa076e",
            "feedback": {
                "content": "This is feedback specific to the second quality of the rubric.",
                "contentType": "text"
            }
        }
    ],
    "rubricQualitySelectedLevels": [
        {
            "qualityId": "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "columnId": "4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        {
            "qualityId": "d2331fb2-2761-402e-8de6-93e0afaa076e",
            "columnId": "aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    ]
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationoutcome",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
