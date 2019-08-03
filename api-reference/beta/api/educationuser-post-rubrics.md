---
title: EducationRubric を作成する
description: 新しい educationRubric オブジェクトを作成します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4929ae79aff73971e6095a15ab11bbaa09bf95f4
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173098"
---
# <a name="create-educationrubric"></a><span data-ttu-id="3787d-103">EducationRubric を作成する</span><span class="sxs-lookup"><span data-stu-id="3787d-103">Create educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3787d-104">新しい[educationRubric](../resources/educationrubric.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3787d-104">Create a new [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3787d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3787d-105">Permissions</span></span>

<span data-ttu-id="3787d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3787d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3787d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3787d-108">Permission type</span></span>                        | <span data-ttu-id="3787d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3787d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3787d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3787d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3787d-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="3787d-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="3787d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3787d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3787d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3787d-113">Not supported.</span></span> |
| <span data-ttu-id="3787d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3787d-114">Application</span></span>                            | <span data-ttu-id="3787d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3787d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3787d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3787d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="3787d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3787d-117">Request headers</span></span>

| <span data-ttu-id="3787d-118">名前</span><span class="sxs-lookup"><span data-stu-id="3787d-118">Name</span></span>          | <span data-ttu-id="3787d-119">説明</span><span class="sxs-lookup"><span data-stu-id="3787d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3787d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3787d-120">Authorization</span></span> | <span data-ttu-id="3787d-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="3787d-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3787d-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="3787d-122">Request body</span></span>

<span data-ttu-id="3787d-123">要求本文で、 [educationRubric](../resources/educationrubric.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3787d-123">In the request body, supply a JSON representation of an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3787d-124">応答</span><span class="sxs-lookup"><span data-stu-id="3787d-124">Response</span></span>

<span data-ttu-id="3787d-125">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で新しい[educationRubric](../resources/educationrubric.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3787d-125">If successful, this method returns `201 Created` response code and a new [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3787d-126">例</span><span class="sxs-lookup"><span data-stu-id="3787d-126">Examples</span></span>

### <a name="example-1-posting-a-credit-rubric"></a><span data-ttu-id="3787d-127">例 1: クレジットカードを投稿する</span><span class="sxs-lookup"><span data-stu-id="3787d-127">Example 1: Posting a Credit Rubric</span></span>

#### <a name="request"></a><span data-ttu-id="3787d-128">要求</span><span class="sxs-lookup"><span data-stu-id="3787d-128">Request</span></span>

<span data-ttu-id="3787d-129">次に示すのは、クレジットカードを投稿する要求の例です。これは、ポイントがない場合に使用されます。</span><span class="sxs-lookup"><span data-stu-id="3787d-129">The following is an example of the request to post a credit rubric (a rubric with no points).</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser"
}-->

```http
POST https://graph.microsoft.com/beta/education/me/rubrics
Content-type: application/json

{
    "displayName":"Example Credit Rubric",
    "description":{
        "content":"This is an example of a credit rubric (no points)",
        "contentType":"text"
    },
    "levels":[
        {
            "displayName":"Good",
            "description":{
                "content":"",
                "contentType":"text"
            }
        },
        {
            "displayName":"Poor",
            "description":{
                "content":"",
                "contentType":"text"
            }
        }
    ],
    "qualities":[
        {
            "description":{
                "content":"Argument",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay's argument is persuasive.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay's argument does not make sense.",
                        "contentType":"text"
                    }
                }
            ]
        },
        {
            "description":{
                "content":"Spelling and Grammar",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay uses proper spelling and grammar with few or no errors.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay has numerous errors in spelling and/or grammar.",
                        "contentType":"text"
                    }
                }
            ]
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="3787d-130">応答</span><span class="sxs-lookup"><span data-stu-id="3787d-130">Response</span></span>

<span data-ttu-id="3787d-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3787d-131">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3787d-132">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="3787d-132">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3787d-133">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3787d-133">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Example Credit Rubric",
    "id": "63618139-2e8d-4f56-a762-dd734736816f",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "qualities": [
        {
            "qualityId": "461e866a-4844-4a3f-9a3c-e5464a32acf1",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ccb47c1c-1a01-4027-93d7-f14b9fe86fdd",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "levels": [
        {
            "levelId": "564e68f6-984b-4574-bea7-ffae3c92633f",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f082e35-46e3-4944-baea-ea6c7e36ef37",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ]
}
```

### <a name="example-2-posting-a-points-rubric"></a><span data-ttu-id="3787d-134">例 2: ポイントを投稿する (Ic)</span><span class="sxs-lookup"><span data-stu-id="3787d-134">Example 2: Posting a Points Rubric</span></span>

<span data-ttu-id="3787d-135">次に示すのは、ポイントを使用して、指定されたコレクションを投稿する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3787d-135">The following is an example of the request to post a rubric with points.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationuser"
}-->

```http
POST https://graph.microsoft.com/beta/education/me/rubrics
Content-type: application/json

{
    "displayName":"Example Points Rubric",
    "description":{
        "content":"This is an example of a rubric with points",
        "contentType":"text"
    },
    "levels":[
        {
            "displayName":"Good",
            "description":{
                "content":"",
                "contentType":"text"
            },
            "grading":{
                "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints":2
            }
        },
        {
            "displayName":"Poor",
            "description":{
                "content":"",
                "contentType":"text"
            },
            "grading":{
                "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints":1
            }
        }
    ],
    "qualities":[
        {
            "description":{
                "content":"Argument",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay's argument is persuasive.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay's argument does not make sense.",
                        "contentType":"text"
                    }
                }
            ],
            "weight":50.0
        },
        {
            "description":{
                "content":"Spelling and Grammar",
                "contentType":"text"
            },
            "criteria":[
                {
                    "description":{
                        "content":"The essay uses proper spelling and grammar with few or no errors.",
                        "contentType":"text"
                    }
                },
                {
                    "description":{
                        "content":"The essay has numerous errors in spelling and/or grammar.",
                        "contentType":"text"
                    }
                }
            ],
            "weight":50.0
        }
    ],
    "grading":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGradeType"
    }
}
```

#### <a name="response"></a><span data-ttu-id="3787d-136">応答</span><span class="sxs-lookup"><span data-stu-id="3787d-136">Response</span></span>

<span data-ttu-id="3787d-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3787d-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3787d-138">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="3787d-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3787d-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3787d-139">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Example Points Rubric",
    "id": "bf040af7-a5ff-4abe-a8c8-1bdc532344c2",
    "description": {
        "content": "This is an example of a rubric with points",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "519cd134-c513-40b9-aa71-fdb0d063c084",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 2
            }
        },
        {
            "levelId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 1
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
            "weight": 50.0,
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5e637d79-f26b-4ea6-acd7-73824f0c0967",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "ebdcc27f-d1ec-4aa3-9da7-bd8d7842e3d3",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
            "weight": 50.0,
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5417252a-f810-41eb-9a83-09276a258a08",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "5de220bd-74b9-41a7-85d5-9be7c6cb7933",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->