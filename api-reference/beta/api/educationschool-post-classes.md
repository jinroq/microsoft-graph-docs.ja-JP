---
title: educationClass を educationSchool に追加する
description: 学校にクラスを追加します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 10b68bbad43fb0cc107d76f27f49ff0fd9b9442d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416122"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="f60ba-103">educationClass を educationSchool に追加する</span><span class="sxs-lookup"><span data-stu-id="f60ba-103">Add educationClass to educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f60ba-104">学校にクラスを追加します。</span><span class="sxs-lookup"><span data-stu-id="f60ba-104">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="f60ba-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f60ba-105">Permissions</span></span>
<span data-ttu-id="f60ba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f60ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f60ba-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f60ba-108">Permission type</span></span>      | <span data-ttu-id="f60ba-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f60ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f60ba-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f60ba-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f60ba-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f60ba-111">Not supported.</span></span>  |
|<span data-ttu-id="f60ba-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f60ba-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f60ba-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f60ba-113">Not supported.</span></span>  |
|<span data-ttu-id="f60ba-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f60ba-114">Application</span></span> | <span data-ttu-id="f60ba-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f60ba-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f60ba-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f60ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f60ba-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f60ba-117">Request headers</span></span>
| <span data-ttu-id="f60ba-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f60ba-118">Header</span></span>       | <span data-ttu-id="f60ba-119">値</span><span class="sxs-lookup"><span data-stu-id="f60ba-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f60ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f60ba-120">Authorization</span></span>  | <span data-ttu-id="f60ba-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f60ba-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f60ba-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f60ba-123">Content-Type</span></span>  | <span data-ttu-id="f60ba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f60ba-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f60ba-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f60ba-125">Request body</span></span>
<span data-ttu-id="f60ba-126">要求本文で、[educationClass](../resources/educationclass.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f60ba-126">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f60ba-127">応答</span><span class="sxs-lookup"><span data-stu-id="f60ba-127">Response</span></span>
<span data-ttu-id="f60ba-128">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f60ba-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f60ba-129">例</span><span class="sxs-lookup"><span data-stu-id="f60ba-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f60ba-130">要求</span><span class="sxs-lookup"><span data-stu-id="f60ba-130">Request</span></span>
<span data-ttu-id="f60ba-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f60ba-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f60ba-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f60ba-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f60ba-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f60ba-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f60ba-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="f60ba-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="f60ba-135">C#</span><span class="sxs-lookup"><span data-stu-id="f60ba-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f60ba-136">応答</span><span class="sxs-lookup"><span data-stu-id="f60ba-136">Response</span></span> 
<span data-ttu-id="f60ba-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f60ba-137">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
