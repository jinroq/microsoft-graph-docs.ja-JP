---
title: EducationRubric を educationAssignment に接続する
description: 既存の educationRubric オブジェクトを educationAssignment に添付します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 50d3cdd61578cb2ae2474a7b58220caf2b94463b
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173189"
---
# <a name="create-educationrubric"></a><span data-ttu-id="66697-103">EducationRubric を作成する</span><span class="sxs-lookup"><span data-stu-id="66697-103">Create educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66697-104">既存の[educationRubric](../resources/educationrubric.md)オブジェクトを[educationAssignment](../resources/educationassignment.md)に添付します。</span><span class="sxs-lookup"><span data-stu-id="66697-104">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="66697-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66697-105">Permissions</span></span>

<span data-ttu-id="66697-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66697-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66697-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66697-108">Permission type</span></span>                        | <span data-ttu-id="66697-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66697-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="66697-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66697-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="66697-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="66697-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="66697-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66697-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66697-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66697-113">Not supported.</span></span> |
| <span data-ttu-id="66697-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66697-114">Application</span></span>                            | <span data-ttu-id="66697-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66697-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66697-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66697-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="66697-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66697-117">Request headers</span></span>

| <span data-ttu-id="66697-118">名前</span><span class="sxs-lookup"><span data-stu-id="66697-118">Name</span></span>          | <span data-ttu-id="66697-119">説明</span><span class="sxs-lookup"><span data-stu-id="66697-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="66697-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="66697-120">Authorization</span></span> | <span data-ttu-id="66697-121">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="66697-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="66697-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="66697-122">Request body</span></span>

<span data-ttu-id="66697-123">要求本文で、既存の[educationRubric](../resources/educationrubric.md)オブジェクトの OData ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="66697-123">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66697-124">応答</span><span class="sxs-lookup"><span data-stu-id="66697-124">Response</span></span>

<span data-ttu-id="66697-p102">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="66697-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="66697-127">例</span><span class="sxs-lookup"><span data-stu-id="66697-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="66697-128">要求</span><span class="sxs-lookup"><span data-stu-id="66697-128">Request</span></span>

<span data-ttu-id="66697-129">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66697-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationassignment"
}-->

```http
PUT https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
}
```

### <a name="response"></a><span data-ttu-id="66697-130">応答</span><span class="sxs-lookup"><span data-stu-id="66697-130">Response</span></span>

<span data-ttu-id="66697-131">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66697-131">The following is an example of the response.</span></span>

> <span data-ttu-id="66697-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="66697-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 204 No Content
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
