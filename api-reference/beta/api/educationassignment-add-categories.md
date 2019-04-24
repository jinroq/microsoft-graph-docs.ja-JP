---
title: educationCategories の追加
description: 既存の educationCategory をこの educationAssignment に追加する
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d5fbf5d6db4ade6e44f65c256879c535d2e2a0e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458335"
---
# <a name="add-educationcategories"></a><span data-ttu-id="2cfb6-103">educationCategories の追加</span><span class="sxs-lookup"><span data-stu-id="2cfb6-103">Add educationCategories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cfb6-104">この[educationAssignment](../resources/educationassignment.md)に、1つ以上の既存の[educationCategory](../resources/educationcategory.md)オブジェクトを追加します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-104">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2cfb6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2cfb6-105">Permissions</span></span>
<span data-ttu-id="2cfb6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cfb6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2cfb6-108">Permission type</span></span>      | <span data-ttu-id="2cfb6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2cfb6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cfb6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2cfb6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2cfb6-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="2cfb6-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2cfb6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2cfb6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2cfb6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-113">Not supported.</span></span>  |
|<span data-ttu-id="2cfb6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2cfb6-114">Application</span></span> | <span data-ttu-id="2cfb6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="2cfb6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2cfb6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2cfb6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cfb6-117">Request headers</span></span>
| <span data-ttu-id="2cfb6-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cfb6-118">Header</span></span>       | <span data-ttu-id="2cfb6-119">値</span><span class="sxs-lookup"><span data-stu-id="2cfb6-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2cfb6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cfb6-120">Authorization</span></span>  | <span data-ttu-id="2cfb6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2cfb6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2cfb6-123">Content-Type</span></span>  | <span data-ttu-id="2cfb6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2cfb6-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2cfb6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2cfb6-125">Request body</span></span>
<span data-ttu-id="2cfb6-126">要求本文で、この割り当てに追加する既存の[educationCategory](../resources/educationcategory.md)オブジェクトの odata.id を指定します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-126">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="2cfb6-127">応答</span><span class="sxs-lookup"><span data-stu-id="2cfb6-127">Response</span></span>
<span data-ttu-id="2cfb6-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cfb6-129">例</span><span class="sxs-lookup"><span data-stu-id="2cfb6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cfb6-130">要求</span><span class="sxs-lookup"><span data-stu-id="2cfb6-130">Request</span></span>
<span data-ttu-id="2cfb6-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="2cfb6-132">要求本文で、この割り当てに追加する既存の[educationCategory](../resources/educationcategory.md)オブジェクトの odata.id を指定します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-132">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="2cfb6-133">応答</span><span class="sxs-lookup"><span data-stu-id="2cfb6-133">Response</span></span>
<span data-ttu-id="2cfb6-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-134">The following is an example of the response.</span></span> 

><span data-ttu-id="2cfb6-135">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2cfb6-136">すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2cfb6-136">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-add-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
