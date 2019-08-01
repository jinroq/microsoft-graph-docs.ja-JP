---
title: AccessReview をリセットする
description: Azure AD access レビュー機能で、現在アクティブな accessReview の決定をリセットします。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  以前の決定は記録されなくなりますが、レビューアーは引き続き決定を更新できます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 871b1bd777413e07b451fe7e889c69fcf183f62b
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049555"
---
# <a name="reset-accessreview"></a><span data-ttu-id="28aae-105">AccessReview をリセットする</span><span class="sxs-lookup"><span data-stu-id="28aae-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28aae-106">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、現在アクティブな[accessreview](../resources/accessreview.md)の決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="28aae-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="28aae-107">ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="28aae-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="28aae-108">以前の決定は記録されなくなりますが、レビューアーは引き続き決定を更新できます。</span><span class="sxs-lookup"><span data-stu-id="28aae-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="28aae-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="28aae-109">Permissions</span></span>
<span data-ttu-id="28aae-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28aae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28aae-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28aae-112">Permission type</span></span>                        | <span data-ttu-id="28aae-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="28aae-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="28aae-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28aae-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="28aae-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28aae-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="28aae-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28aae-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28aae-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28aae-117">Not supported.</span></span> |
|<span data-ttu-id="28aae-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28aae-118">Application</span></span>                            | <span data-ttu-id="28aae-119">AccessReview の構成</span><span class="sxs-lookup"><span data-stu-id="28aae-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="28aae-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28aae-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="28aae-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28aae-121">Request headers</span></span>
| <span data-ttu-id="28aae-122">名前</span><span class="sxs-lookup"><span data-stu-id="28aae-122">Name</span></span>         | <span data-ttu-id="28aae-123">型</span><span class="sxs-lookup"><span data-stu-id="28aae-123">Type</span></span>        | <span data-ttu-id="28aae-124">説明</span><span class="sxs-lookup"><span data-stu-id="28aae-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="28aae-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="28aae-125">Authorization</span></span> | <span data-ttu-id="28aae-126">string</span><span class="sxs-lookup"><span data-stu-id="28aae-126">string</span></span> | <span data-ttu-id="28aae-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="28aae-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28aae-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="28aae-129">Request body</span></span>
<span data-ttu-id="28aae-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="28aae-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="28aae-131">応答</span><span class="sxs-lookup"><span data-stu-id="28aae-131">Response</span></span>
<span data-ttu-id="28aae-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="28aae-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28aae-134">例</span><span class="sxs-lookup"><span data-stu-id="28aae-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28aae-135">要求</span><span class="sxs-lookup"><span data-stu-id="28aae-135">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28aae-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="28aae-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28aae-137">C#</span><span class="sxs-lookup"><span data-stu-id="28aae-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28aae-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="28aae-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28aae-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="28aae-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="28aae-140">Java</span><span class="sxs-lookup"><span data-stu-id="28aae-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reset-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28aae-141">応答</span><span class="sxs-lookup"><span data-stu-id="28aae-141">Response</span></span>
><span data-ttu-id="28aae-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="28aae-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
