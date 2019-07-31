---
title: EducationCategories の追加
description: 既存の educationCategory をこの educationAssignment に追加する
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b5395ab656d0a5e44b4f3a45f7c136009c5bcc61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955793"
---
# <a name="add-educationcategories"></a><span data-ttu-id="f7ecd-103">EducationCategories の追加</span><span class="sxs-lookup"><span data-stu-id="f7ecd-103">Add educationCategories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7ecd-104">この[educationAssignment](../resources/educationassignment.md)に、1つ以上の既存の[educationCategory](../resources/educationcategory.md)オブジェクトを追加します。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-104">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7ecd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7ecd-105">Permissions</span></span>
<span data-ttu-id="f7ecd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7ecd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f7ecd-108">Permission type</span></span>      | <span data-ttu-id="f7ecd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f7ecd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7ecd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f7ecd-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f7ecd-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="f7ecd-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f7ecd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f7ecd-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f7ecd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-113">Not supported.</span></span>  |
|<span data-ttu-id="f7ecd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f7ecd-114">Application</span></span> | <span data-ttu-id="f7ecd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f7ecd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f7ecd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f7ecd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7ecd-117">Request headers</span></span>
| <span data-ttu-id="f7ecd-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7ecd-118">Header</span></span>       | <span data-ttu-id="f7ecd-119">値</span><span class="sxs-lookup"><span data-stu-id="f7ecd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7ecd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7ecd-120">Authorization</span></span>  | <span data-ttu-id="f7ecd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7ecd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7ecd-123">Content-Type</span></span>  | <span data-ttu-id="f7ecd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f7ecd-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7ecd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f7ecd-125">Request body</span></span>
<span data-ttu-id="f7ecd-126">要求本文で、この割り当てに追加する既存の[educationCategory](../resources/educationcategory.md)オブジェクトの odata.id を指定します。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-126">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="f7ecd-127">応答</span><span class="sxs-lookup"><span data-stu-id="f7ecd-127">Response</span></span>
<span data-ttu-id="f7ecd-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f7ecd-129">例</span><span class="sxs-lookup"><span data-stu-id="f7ecd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7ecd-130">要求</span><span class="sxs-lookup"><span data-stu-id="f7ecd-130">Request</span></span>
<span data-ttu-id="f7ecd-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/11021/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
<span data-ttu-id="f7ecd-132">要求本文で、この割り当てに追加する既存の[educationCategory](../resources/educationcategory.md)オブジェクトの odata.id を指定します。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-132">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="f7ecd-133">応答</span><span class="sxs-lookup"><span data-stu-id="f7ecd-133">Response</span></span>
<span data-ttu-id="f7ecd-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-134">The following is an example of the response.</span></span> 

><span data-ttu-id="f7ecd-135">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f7ecd-136">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f7ecd-136">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add educationCategory to educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
