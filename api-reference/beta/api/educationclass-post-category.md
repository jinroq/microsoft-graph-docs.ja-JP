---
title: educationCategory を作成する
description: 新しいカテゴリを作成します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 453e8c03c40966aedeaf58a4f441f7c16500d9a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457782"
---
# <a name="create-educationcategory"></a><span data-ttu-id="a8573-103">educationCategory を作成する</span><span class="sxs-lookup"><span data-stu-id="a8573-103">Create educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8573-104">[educationClass](../resources/educationclass.md)に新しい[educationCategory](../resources/educationcategory.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="a8573-104">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8573-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a8573-105">Permissions</span></span>
<span data-ttu-id="a8573-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8573-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8573-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8573-108">Permission type</span></span>      | <span data-ttu-id="a8573-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8573-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8573-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8573-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a8573-111">EduAssignments の読み取り/書き込みの EduAssignments</span><span class="sxs-lookup"><span data-stu-id="a8573-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a8573-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8573-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a8573-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8573-113">Not supported.</span></span>  |
|<span data-ttu-id="a8573-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8573-114">Application</span></span> | <span data-ttu-id="a8573-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8573-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a8573-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8573-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="a8573-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8573-117">Request headers</span></span>
| <span data-ttu-id="a8573-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8573-118">Header</span></span>       | <span data-ttu-id="a8573-119">値</span><span class="sxs-lookup"><span data-stu-id="a8573-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8573-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8573-120">Authorization</span></span>  | <span data-ttu-id="a8573-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a8573-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a8573-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8573-123">Content-Type</span></span>  | <span data-ttu-id="a8573-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a8573-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8573-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8573-125">Request body</span></span>
<span data-ttu-id="a8573-126">要求本文で、 [educationCategory](../resources/educationcategory.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8573-126">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a8573-127">応答</span><span class="sxs-lookup"><span data-stu-id="a8573-127">Response</span></span>
<span data-ttu-id="a8573-128">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[educationCategory](../resources/educationcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a8573-128">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8573-129">例</span><span class="sxs-lookup"><span data-stu-id="a8573-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8573-130">要求</span><span class="sxs-lookup"><span data-stu-id="a8573-130">Request</span></span>
<span data-ttu-id="a8573-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a8573-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignmentCategories
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
<span data-ttu-id="a8573-132">要求本文で、 [educationCategory](../resources/educationcategory.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8573-132">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="a8573-133">応答</span><span class="sxs-lookup"><span data-stu-id="a8573-133">Response</span></span>
<span data-ttu-id="a8573-134">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a8573-134">The following is an example of the response.</span></span> 

><span data-ttu-id="a8573-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a8573-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 85

{
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-post-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
