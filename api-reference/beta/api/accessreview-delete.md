---
title: AccessReview の削除
description: Azure AD access レビュー機能で、accessReview オブジェクトを削除します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6a221127e766e3c2e8e064dea23932800d3bf2e2
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172791"
---
# <a name="delete-accessreview"></a><span data-ttu-id="1a272-103">AccessReview の削除</span><span class="sxs-lookup"><span data-stu-id="1a272-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a272-104">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、 [accessreview](../resources/accessreview.md)オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1a272-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a272-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1a272-105">Permissions</span></span>
<span data-ttu-id="1a272-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a272-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a272-108">Permission type</span></span>                        | <span data-ttu-id="1a272-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a272-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a272-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a272-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a272-111">AccessReview を行って、AccessReview を行います。</span><span class="sxs-lookup"><span data-stu-id="1a272-111">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="1a272-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a272-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a272-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a272-113">Not supported.</span></span> |
|<span data-ttu-id="1a272-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a272-114">Application</span></span>                            | <span data-ttu-id="1a272-115">AccessReview の構成</span><span class="sxs-lookup"><span data-stu-id="1a272-115">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="1a272-116">また、呼び出し元には、 [programcontrol](../resources/programcontrol.md)を削除できるように、すべてのアクセス許可が含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a272-116">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="1a272-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a272-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="1a272-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a272-118">Request headers</span></span>
| <span data-ttu-id="1a272-119">名前</span><span class="sxs-lookup"><span data-stu-id="1a272-119">Name</span></span>         | <span data-ttu-id="1a272-120">型</span><span class="sxs-lookup"><span data-stu-id="1a272-120">Type</span></span>        | <span data-ttu-id="1a272-121">説明</span><span class="sxs-lookup"><span data-stu-id="1a272-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1a272-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a272-122">Authorization</span></span> | <span data-ttu-id="1a272-123">string</span><span class="sxs-lookup"><span data-stu-id="1a272-123">string</span></span> | <span data-ttu-id="1a272-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="1a272-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a272-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a272-126">Request body</span></span>
<span data-ttu-id="1a272-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a272-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1a272-128">応答</span><span class="sxs-lookup"><span data-stu-id="1a272-128">Response</span></span>
<span data-ttu-id="1a272-p103">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1a272-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a272-131">例</span><span class="sxs-lookup"><span data-stu-id="1a272-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a272-132">要求</span><span class="sxs-lookup"><span data-stu-id="1a272-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a272-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1a272-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a272-134">C#</span><span class="sxs-lookup"><span data-stu-id="1a272-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a272-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a272-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a272-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="1a272-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1a272-137">Java</span><span class="sxs-lookup"><span data-stu-id="1a272-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1a272-138">応答</span><span class="sxs-lookup"><span data-stu-id="1a272-138">Response</span></span>
><span data-ttu-id="1a272-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="1a272-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
