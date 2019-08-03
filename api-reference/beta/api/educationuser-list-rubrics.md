---
title: リストを表示する (ics)
description: Educationrubric オブジェクトのリストを取得します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ce8c30cc09d1ba46a76351614df1e3d925c83877
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173105"
---
# <a name="list-rubrics"></a><span data-ttu-id="9e06a-103">リストを表示する (ics)</span><span class="sxs-lookup"><span data-stu-id="9e06a-103">List rubrics</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e06a-104">[EducationRubric](../resources/educationrubric.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="9e06a-104">Retrieve a list of [educationRubric](../resources/educationrubric.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e06a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9e06a-105">Permissions</span></span>

<span data-ttu-id="9e06a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e06a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e06a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e06a-108">Permission type</span></span>                        | <span data-ttu-id="9e06a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e06a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e06a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e06a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e06a-111">EduAssignments、EduAssignments、EduAssignments、および EduAssignments の読み取り/書き込みの基本</span><span class="sxs-lookup"><span data-stu-id="9e06a-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="9e06a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e06a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e06a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e06a-113">Not supported.</span></span> |
| <span data-ttu-id="9e06a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e06a-114">Application</span></span>                            | <span data-ttu-id="9e06a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e06a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e06a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e06a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics
```

## <a name="request-headers"></a><span data-ttu-id="9e06a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e06a-117">Request headers</span></span>

| <span data-ttu-id="9e06a-118">名前</span><span class="sxs-lookup"><span data-stu-id="9e06a-118">Name</span></span>      |<span data-ttu-id="9e06a-119">説明</span><span class="sxs-lookup"><span data-stu-id="9e06a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e06a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e06a-120">Authorization</span></span> | <span data-ttu-id="9e06a-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="9e06a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e06a-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e06a-122">Request body</span></span>

<span data-ttu-id="9e06a-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9e06a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e06a-124">応答</span><span class="sxs-lookup"><span data-stu-id="9e06a-124">Response</span></span>

<span data-ttu-id="9e06a-125">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationRubric](../resources/educationrubric.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9e06a-125">If successful, this method returns a `200 OK` response code and a collection of [educationRubric](../resources/educationrubric.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e06a-126">例</span><span class="sxs-lookup"><span data-stu-id="9e06a-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e06a-127">要求</span><span class="sxs-lookup"><span data-stu-id="9e06a-127">Request</span></span>

<span data-ttu-id="9e06a-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9e06a-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rubrics"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/rubrics
```

### <a name="response"></a><span data-ttu-id="9e06a-129">応答</span><span class="sxs-lookup"><span data-stu-id="9e06a-129">Response</span></span>

<span data-ttu-id="9e06a-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9e06a-130">The following is an example of the response.</span></span>

> <span data-ttu-id="9e06a-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9e06a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
        {
            "displayName":"Example Credit Rubric",
            "id":"c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
            "description":{
                "content":"This is an example of a credit rubric (no points)",
                "contentType":"text"
            },
            "levels":[
                {
                    "levelId":"dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
                    "displayName":"Good",
                    "description":{
                        "content":"",
                        "contentType":"text"
                    }
                },
                {
                    "levelId":"3f2e4b0f-508e-4005-984b-17e061bc5377",
                    "displayName":"Poor",
                    "description":{
                        "content":"",
                        "contentType":"text"
                    }
                }
            ],
            "qualities":[
                {
                    "qualityId":"dc79dcbf-b536-4797-9c5b-902f28129fd0",
                    "description":{
                        "content":"Argument",
                        "contentType":"text"
                    },
                    "criteria":[
                        {
                            "id":"8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                            "description":{
                                "content":"The essay's argument is persuasive.",
                                "contentType":"text"
                            }
                        },
                        {
                            "id":"4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                            "description":{
                                "content":"The essay's argument does not make sense.",
                                "contentType":"text"
                            }
                        }
                    ]
                },
                {
                    "qualityId":"7e087062-ac25-4629-8386-a946350936db",
                    "description":{
                        "content":"Spelling and Grammar",
                        "contentType":"text"
                    },
                    "criteria":[
                        {
                            "id":"12276eb2-122c-4ad2-ba92-335ea798c88e",
                            "description":{
                                "content":"The essay uses proper spelling and grammar with few or no errors.",
                                "contentType":"text"
                            }
                        },
                        {
                            "id":"3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                            "description":{
                                "content":"The essay has numerous errors in spelling and/or grammar.",
                                "contentType":"text"
                            }
                        }
                    ]
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
  "description": "List rubrics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
