---
title: Get educationRubric が educationAssignment に添付されています。
description: EducationAssignment に添付されている educaitonRubric を取得します (存在する場合)。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9448b671ce656e8c88e3681490a2486d10885c7d
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173196"
---
# <a name="get-educationrubric-attached-to-educationassignment"></a><span data-ttu-id="7057a-103">Get educationRubric が educationAssignment に添付されています。</span><span class="sxs-lookup"><span data-stu-id="7057a-103">Get educationRubric attached to educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7057a-104">[EducationAssignment](../resources/educationassignment.md)に添付されている[educationRubric](../resources/educationrubric.md)オブジェクトがある場合は、それを取得します。</span><span class="sxs-lookup"><span data-stu-id="7057a-104">Get the [educationRubric](../resources/educationrubric.md) object attached to an [educationAssignment](../resources/educationassignment.md), if one exists.</span></span>

## <a name="permissions"></a><span data-ttu-id="7057a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7057a-105">Permissions</span></span>

<span data-ttu-id="7057a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7057a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7057a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7057a-108">Permission type</span></span>                        | <span data-ttu-id="7057a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7057a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7057a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7057a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7057a-111">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="7057a-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="7057a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7057a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7057a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7057a-113">Not supported.</span></span> |
| <span data-ttu-id="7057a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7057a-114">Application</span></span>                            | <span data-ttu-id="7057a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7057a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7057a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7057a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="7057a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7057a-117">Request headers</span></span>

| <span data-ttu-id="7057a-118">名前</span><span class="sxs-lookup"><span data-stu-id="7057a-118">Name</span></span>      |<span data-ttu-id="7057a-119">説明</span><span class="sxs-lookup"><span data-stu-id="7057a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7057a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7057a-120">Authorization</span></span> | <span data-ttu-id="7057a-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="7057a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7057a-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="7057a-122">Request body</span></span>

<span data-ttu-id="7057a-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7057a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7057a-124">応答</span><span class="sxs-lookup"><span data-stu-id="7057a-124">Response</span></span>

<span data-ttu-id="7057a-125">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationRubric](../resources/educationrubric.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7057a-125">If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7057a-126">例</span><span class="sxs-lookup"><span data-stu-id="7057a-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7057a-127">要求</span><span class="sxs-lookup"><span data-stu-id="7057a-127">Request</span></span>

<span data-ttu-id="7057a-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7057a-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rubric"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric
```

### <a name="response"></a><span data-ttu-id="7057a-129">応答</span><span class="sxs-lookup"><span data-stu-id="7057a-129">Response</span></span>

<span data-ttu-id="7057a-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7057a-130">The following is an example of the response.</span></span>

> <span data-ttu-id="7057a-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7057a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
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
  "description": "List rubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
