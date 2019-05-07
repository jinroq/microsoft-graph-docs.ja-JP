---
title: 教師を追加する
description: クラスに教師を追加します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6f2c7b9099624f5e8db1cc39657f41d328564423
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616161"
---
# <a name="add-teacher"></a><span data-ttu-id="84971-103">教師を追加する</span><span class="sxs-lookup"><span data-stu-id="84971-103">Add teacher</span></span>

<span data-ttu-id="84971-104">クラスに教師を追加します。</span><span class="sxs-lookup"><span data-stu-id="84971-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="84971-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="84971-105">Permissions</span></span>
<span data-ttu-id="84971-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84971-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84971-108">Permission type</span></span>      | <span data-ttu-id="84971-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="84971-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84971-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84971-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="84971-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84971-111">Not supported.</span></span>  |
|<span data-ttu-id="84971-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84971-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="84971-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84971-113">Not supported.</span></span>  |
|<span data-ttu-id="84971-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84971-114">Application</span></span> | <span data-ttu-id="84971-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84971-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="84971-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84971-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="84971-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84971-117">Request headers</span></span>
| <span data-ttu-id="84971-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84971-118">Header</span></span>       | <span data-ttu-id="84971-119">値</span><span class="sxs-lookup"><span data-stu-id="84971-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="84971-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="84971-120">Authorization</span></span>  | <span data-ttu-id="84971-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="84971-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="84971-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84971-123">Content-Type</span></span>  | <span data-ttu-id="84971-124">application/json</span><span class="sxs-lookup"><span data-stu-id="84971-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84971-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="84971-125">Request body</span></span>
<span data-ttu-id="84971-126">要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="84971-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="84971-127">応答</span><span class="sxs-lookup"><span data-stu-id="84971-127">Response</span></span>
<span data-ttu-id="84971-128">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="84971-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84971-129">例</span><span class="sxs-lookup"><span data-stu-id="84971-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84971-130">要求</span><span class="sxs-lookup"><span data-stu-id="84971-130">Request</span></span>
<span data-ttu-id="84971-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="84971-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="84971-132">応答</span><span class="sxs-lookup"><span data-stu-id="84971-132">Response</span></span>
<span data-ttu-id="84971-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="84971-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="84971-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="84971-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="84971-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="84971-136">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84971-137">Java</span><span class="sxs-lookup"><span data-stu-id="84971-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationclass-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationclass-post-teachers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
