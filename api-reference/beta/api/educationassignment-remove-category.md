---
title: EducationCategory の削除
description: 既存の educationCategory をこの educationAssignment から削除します。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: deb55b14c40acb25b366eec140cbc433e9ee203d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955666"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="430f9-103">EducationCategory の削除</span><span class="sxs-lookup"><span data-stu-id="430f9-103">Remove educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="430f9-104">[EducationAssignment](../resources/educationassignment.md)から[educationCategory](../resources/educationcategory.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="430f9-104">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="430f9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="430f9-105">Permissions</span></span>
<span data-ttu-id="430f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="430f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="430f9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="430f9-108">Permission type</span></span>      | <span data-ttu-id="430f9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="430f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="430f9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="430f9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="430f9-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="430f9-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="430f9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="430f9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="430f9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="430f9-113">Not supported.</span></span>  |
|<span data-ttu-id="430f9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="430f9-114">Application</span></span> | <span data-ttu-id="430f9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="430f9-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="430f9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="430f9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="430f9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="430f9-117">Request headers</span></span>
| <span data-ttu-id="430f9-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="430f9-118">Header</span></span>       | <span data-ttu-id="430f9-119">値</span><span class="sxs-lookup"><span data-stu-id="430f9-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="430f9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="430f9-120">Authorization</span></span>  | <span data-ttu-id="430f9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="430f9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="430f9-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="430f9-123">Content-Type</span></span>  | <span data-ttu-id="430f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="430f9-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="430f9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="430f9-125">Request body</span></span>
<span data-ttu-id="430f9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="430f9-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="430f9-127">応答</span><span class="sxs-lookup"><span data-stu-id="430f9-127">Response</span></span>
<span data-ttu-id="430f9-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="430f9-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="430f9-129">例</span><span class="sxs-lookup"><span data-stu-id="430f9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="430f9-130">要求</span><span class="sxs-lookup"><span data-stu-id="430f9-130">Request</span></span>
<span data-ttu-id="430f9-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="430f9-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="430f9-132">応答</span><span class="sxs-lookup"><span data-stu-id="430f9-132">Response</span></span>
<span data-ttu-id="430f9-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="430f9-133">The following is an example of the response.</span></span> 

><span data-ttu-id="430f9-134">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="430f9-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="430f9-135">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="430f9-135">All of the properties will be returned from an actual call.</span></span>


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
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
