---
title: 結果の一覧表示
description: Educationoutcome オブジェクトのリストを取得します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7f7827576fbe6719e8a131af465a6ca61c686090
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173112"
---
# <a name="list-outcomes"></a><span data-ttu-id="913b9-103">結果の一覧表示</span><span class="sxs-lookup"><span data-stu-id="913b9-103">List outcomes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="913b9-104">[EducationOutcome](../resources/educationoutcome.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="913b9-104">Retrieve a list of [educationOutcome](../resources/educationoutcome.md) objects.</span></span>  <span data-ttu-id="913b9-105">結果には、 **educationPointsOutcome**、 **EducationFeedbackOutcome**、および**educationRubricOutcome**の3つの種類があります。</span><span class="sxs-lookup"><span data-stu-id="913b9-105">There are three types of outcomes: **educationPointsOutcome**, **educationFeedbackOutcome**, and **educationRubricOutcome**.</span></span>

<span data-ttu-id="913b9-106">(ポイント値を持たず、EducationFeedbackOutcome bric を使用しない) クレジット課題の送信には、 [](../resources/educationpointsoutcome.md)があります。</span><span class="sxs-lookup"><span data-stu-id="913b9-106">A submission for a credit assignment (one that has no point value and no rubric) will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span></span> <span data-ttu-id="913b9-107">( [EducationPointsOutcome](../resources/educationpointsoutcome.md)が返される場合もありますが、その結果は無視されます)。</span><span class="sxs-lookup"><span data-stu-id="913b9-107">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="913b9-108">ポイントの割り当て (ポイント値が割り当てられているもの) の送信には、 [educationFeedbackOutcome](../resources/educationpointsoutcome.md)と[educationPointsOutcome](../resources/educationpointsoutcome.md)の両方が含まれます。</span><span class="sxs-lookup"><span data-stu-id="913b9-108">A submission for a points assignment (one that has a point value assigned) will have both an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationPointsOutcome](../resources/educationpointsoutcome.md).</span></span>

<span data-ttu-id="913b9-109">付与されている割り当てに対しては、 [educationFeedbackOutcome](../resources/educationpointsoutcome.md)と[educationRubricOutcome](../resources/educationrubricoutcome.md)を使用しています (ポイントはありません)、割り当ての送信。</span><span class="sxs-lookup"><span data-stu-id="913b9-109">A submission for an assignment with an attached rubric, if the rubric is a credit rubric (no points), will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span> <span data-ttu-id="913b9-110">( [EducationPointsOutcome](../resources/educationpointsoutcome.md)が返される場合もありますが、その結果は無視されます)。</span><span class="sxs-lookup"><span data-stu-id="913b9-110">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="913b9-111">付与されている割り当てに対して、指定されている場合は、 [educationFeedbackOutcome](../resources/educationpointsoutcome.md)が含まれている場合は、[educationPointsOutcome] (../resources/educationpointsoutcome.md、および[educationRubricOutcome](../resources/educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="913b9-111">A submission for an assignment with an attached rubric, if the rubric is a points rubric, will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md), an [educationPointsOutcome](../resources/educationpointsoutcome.md, and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span>

<span data-ttu-id="913b9-112">すべての結果の種類には、その結果の種類に適した、正規の、公開されたプロパティがあります。たとえば、**ポイント**と**publishedpoints**、**フィードバック**、 **publishedpoints**などです。</span><span class="sxs-lookup"><span data-stu-id="913b9-112">All outcome types have a regular and a published property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span>  <span data-ttu-id="913b9-113">正規プロパティは、教師によって更新された最新の値です。発行されたプロパティは、生徒に返された最新の値です。</span><span class="sxs-lookup"><span data-stu-id="913b9-113">The regular property is the most recent value updated by the teacher; the published property is the most recent value returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="913b9-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="913b9-114">Permissions</span></span>

<span data-ttu-id="913b9-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="913b9-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="913b9-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="913b9-117">Permission type</span></span>                        | <span data-ttu-id="913b9-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="913b9-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="913b9-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="913b9-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="913b9-120">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="913b9-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="913b9-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="913b9-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="913b9-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="913b9-122">Not supported.</span></span> |
| <span data-ttu-id="913b9-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="913b9-123">Application</span></span>                            | <span data-ttu-id="913b9-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="913b9-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="913b9-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="913b9-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```

## <a name="request-headers"></a><span data-ttu-id="913b9-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="913b9-126">Request headers</span></span>

| <span data-ttu-id="913b9-127">名前</span><span class="sxs-lookup"><span data-stu-id="913b9-127">Name</span></span>      |<span data-ttu-id="913b9-128">説明</span><span class="sxs-lookup"><span data-stu-id="913b9-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="913b9-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="913b9-129">Authorization</span></span> | <span data-ttu-id="913b9-130">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="913b9-130">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="913b9-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="913b9-131">Request body</span></span>

<span data-ttu-id="913b9-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="913b9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="913b9-133">応答</span><span class="sxs-lookup"><span data-stu-id="913b9-133">Response</span></span>

<span data-ttu-id="913b9-134">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationOutcome](../resources/educationoutcome.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="913b9-134">If successful, this method returns a `200 OK` response code and a collection of [educationOutcome](../resources/educationoutcome.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="913b9-135">例</span><span class="sxs-lookup"><span data-stu-id="913b9-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="913b9-136">要求</span><span class="sxs-lookup"><span data-stu-id="913b9-136">Request</span></span>

<span data-ttu-id="913b9-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="913b9-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes
```

### <a name="response"></a><span data-ttu-id="913b9-138">応答</span><span class="sxs-lookup"><span data-stu-id="913b9-138">Response</span></span>

<span data-ttu-id="913b9-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="913b9-139">The following is an example of the response.</span></span>

> <span data-ttu-id="913b9-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="913b9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationOutcome",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
            "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
            "feedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedFeedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationPointsOutcome",
            "id": "ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
            "points": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedPoints": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationRubricOutcome",
            "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
            "rubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "rubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
                }
            ],
            "publishedRubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "publishedRubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List outcomes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
