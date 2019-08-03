---
title: EducationRubric の更新
description: EducationRubric オブジェクトのプロパティを更新します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c1c900084c0410f583621b43b145ccd9934c820b
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173140"
---
# <a name="update-educationrubric"></a><span data-ttu-id="aed32-103">EducationRubric の更新</span><span class="sxs-lookup"><span data-stu-id="aed32-103">Update educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aed32-104">[EducationRubric](../resources/educationrubric.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aed32-104">Update the properties of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="aed32-105">割り当てに関連付けられている割り当て (`PATCH /education/me/assignments/{id}/rubric`) を更新することは、割り当てが発行される前にのみ可能であり、更新されたもの`/education/users/{id}/rubrics`は、実際には、その下に存在する元のアカウントになります。</span><span class="sxs-lookup"><span data-stu-id="aed32-105">Updating a rubric attached to an assignment (`PATCH /education/me/assignments/{id}/rubric`) is only possible before the assignment is published, and what is updated is actually the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="aed32-106">割り当てが発行されると、その特定の割り当てに関連付けられている、保存期間の不変コピーが作成されます。</span><span class="sxs-lookup"><span data-stu-id="aed32-106">After the assignment is published, an immutable copy of the rubric is made that is attached to that specific assignment.</span></span> <span data-ttu-id="aed32-107">この場合、 [GET/education/me/assignments/{id}/rubric](educationrubric-get.md)を使用して取得できますが、更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="aed32-107">That rubric can be retrieved using [GET /education/me/assignments/{id}/rubric](educationrubric-get.md), but it cannot be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="aed32-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aed32-108">Permissions</span></span>

<span data-ttu-id="aed32-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aed32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aed32-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aed32-111">Permission type</span></span>                        | <span data-ttu-id="aed32-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aed32-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aed32-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aed32-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="aed32-114">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="aed32-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="aed32-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aed32-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aed32-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aed32-116">Not supported.</span></span> |
| <span data-ttu-id="aed32-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aed32-117">Application</span></span>                            | <span data-ttu-id="aed32-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aed32-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aed32-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aed32-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me/rubrics/{id}
PATCH /education/me/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="aed32-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aed32-120">Request headers</span></span>

| <span data-ttu-id="aed32-121">名前</span><span class="sxs-lookup"><span data-stu-id="aed32-121">Name</span></span>       | <span data-ttu-id="aed32-122">説明</span><span class="sxs-lookup"><span data-stu-id="aed32-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="aed32-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aed32-123">Authorization</span></span> | <span data-ttu-id="aed32-124">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="aed32-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="aed32-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="aed32-125">Request body</span></span>

<span data-ttu-id="aed32-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="aed32-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="aed32-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="aed32-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="aed32-128">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="aed32-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="aed32-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aed32-129">Property</span></span>     | <span data-ttu-id="aed32-130">型</span><span class="sxs-lookup"><span data-stu-id="aed32-130">Type</span></span>        | <span data-ttu-id="aed32-131">説明</span><span class="sxs-lookup"><span data-stu-id="aed32-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aed32-132">description</span><span class="sxs-lookup"><span data-stu-id="aed32-132">description</span></span>|<span data-ttu-id="aed32-133">Microsoft.outlookservices.itembody</span><span class="sxs-lookup"><span data-stu-id="aed32-133">itemBody</span></span>|<span data-ttu-id="aed32-134">このテンプレートの説明。</span><span class="sxs-lookup"><span data-stu-id="aed32-134">The description of this rubric.</span></span>|
|<span data-ttu-id="aed32-135">displayName</span><span class="sxs-lookup"><span data-stu-id="aed32-135">displayName</span></span>|<span data-ttu-id="aed32-136">String</span><span class="sxs-lookup"><span data-stu-id="aed32-136">String</span></span>|<span data-ttu-id="aed32-137">この名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="aed32-137">The name of this rubric.</span></span>|
|<span data-ttu-id="aed32-138">変化</span><span class="sxs-lookup"><span data-stu-id="aed32-138">grading</span></span>|<span data-ttu-id="aed32-139">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="aed32-139">educationAssignmentGradeType</span></span>|<span data-ttu-id="aed32-140">このテンプレートがポイントしているかどうか。</span><span class="sxs-lookup"><span data-stu-id="aed32-140">Whether this rubric has points or not.</span></span>|
|<span data-ttu-id="aed32-141">高度</span><span class="sxs-lookup"><span data-stu-id="aed32-141">levels</span></span>|<span data-ttu-id="aed32-142">プリンシパルコレクション</span><span class="sxs-lookup"><span data-stu-id="aed32-142">rubricLevel collection</span></span>|<span data-ttu-id="aed32-143">このテンプレートを構成するレベルのコレクション。</span><span class="sxs-lookup"><span data-stu-id="aed32-143">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="aed32-144">満たし</span><span class="sxs-lookup"><span data-stu-id="aed32-144">qualities</span></span>|<span data-ttu-id="aed32-145">の最高品質のコレクション</span><span class="sxs-lookup"><span data-stu-id="aed32-145">rubricQuality collection</span></span>|<span data-ttu-id="aed32-146">このテンプレートを構成する品質のコレクション。</span><span class="sxs-lookup"><span data-stu-id="aed32-146">The collection of qualities making up this rubric.</span></span>|

## <a name="response"></a><span data-ttu-id="aed32-147">応答</span><span class="sxs-lookup"><span data-stu-id="aed32-147">Response</span></span>

<span data-ttu-id="aed32-148">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[educationRubric](../resources/educationrubric.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aed32-148">If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aed32-149">例</span><span class="sxs-lookup"><span data-stu-id="aed32-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aed32-150">要求</span><span class="sxs-lookup"><span data-stu-id="aed32-150">Request</span></span>

<span data-ttu-id="aed32-151">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aed32-151">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationrubric"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/rubrics/{id}
Content-type: application/json

{
  "displayName": "Example Credit Rubric after display name patch"
}
```

### <a name="response"></a><span data-ttu-id="aed32-152">応答</span><span class="sxs-lookup"><span data-stu-id="aed32-152">Response</span></span>

<span data-ttu-id="aed32-153">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aed32-153">The following is an example of the response.</span></span>

> <span data-ttu-id="aed32-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="aed32-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "displayName": "Example Credit Rubric after display name patch",
    "id": "c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f2e4b0f-508e-4005-984b-17e061bc5377",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "dc79dcbf-b536-4797-9c5b-902f28129fd0",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "7e087062-ac25-4629-8386-a946350936db",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "12276eb2-122c-4ad2-ba92-335ea798c88e",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
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
  "description": "Update educationrubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
