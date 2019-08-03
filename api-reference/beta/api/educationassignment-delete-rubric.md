---
title: EducationAssignment から educationRubric を削除する
description: EducationAssignment から educationRubric を削除する
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a6334e24c01db8f32f643f552b1a64cb2c86967d
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173224"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="1d70f-103">EducationAssignment から educationRubric を削除する</span><span class="sxs-lookup"><span data-stu-id="1d70f-103">Remove educationRubric from educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d70f-104">[EducationAssignment](../resources/educationassignment.md)から[educationRubric](../resources/educationrubric.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="1d70f-104">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="1d70f-105">これは、自己 ic 自体を削除するわけではありません。</span><span class="sxs-lookup"><span data-stu-id="1d70f-105">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d70f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d70f-106">Permissions</span></span>

<span data-ttu-id="1d70f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d70f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1d70f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d70f-109">Permission type</span></span>                        | <span data-ttu-id="1d70f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d70f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1d70f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d70f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1d70f-112">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="1d70f-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="1d70f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d70f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d70f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d70f-114">Not supported.</span></span> |
| <span data-ttu-id="1d70f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d70f-115">Application</span></span>                            | <span data-ttu-id="1d70f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d70f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d70f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d70f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1d70f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d70f-118">Request headers</span></span>

| <span data-ttu-id="1d70f-119">名前</span><span class="sxs-lookup"><span data-stu-id="1d70f-119">Name</span></span>          | <span data-ttu-id="1d70f-120">説明</span><span class="sxs-lookup"><span data-stu-id="1d70f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1d70f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d70f-121">Authorization</span></span> | <span data-ttu-id="1d70f-122">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="1d70f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d70f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d70f-123">Request body</span></span>

<span data-ttu-id="1d70f-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1d70f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d70f-125">応答</span><span class="sxs-lookup"><span data-stu-id="1d70f-125">Response</span></span>

<span data-ttu-id="1d70f-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1d70f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d70f-128">例</span><span class="sxs-lookup"><span data-stu-id="1d70f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d70f-129">要求</span><span class="sxs-lookup"><span data-stu-id="1d70f-129">Request</span></span>

<span data-ttu-id="1d70f-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d70f-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```

### <a name="response"></a><span data-ttu-id="1d70f-131">応答</span><span class="sxs-lookup"><span data-stu-id="1d70f-131">Response</span></span>

<span data-ttu-id="1d70f-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d70f-132">The following is an example of the response.</span></span>

> <span data-ttu-id="1d70f-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1d70f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
