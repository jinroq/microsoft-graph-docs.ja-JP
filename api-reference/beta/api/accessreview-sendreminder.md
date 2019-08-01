---
title: SendReminder accessReview
description: 'Azure AD access レビュー機能で、現在アクティブな accessReview のレビュー担当者に通知を送信します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7e2176554bd2ed59312c2743f314e16954ff10f2
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049562"
---
# <a name="sendreminder-accessreview"></a><span data-ttu-id="44ccc-104">SendReminder accessReview</span><span class="sxs-lookup"><span data-stu-id="44ccc-104">SendReminder accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44ccc-105">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、現在アクティブな[accessreview](../resources/accessreview.md)のレビュー担当者に通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="44ccc-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, send a reminder to the reviewers of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="44ccc-106">ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="44ccc-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span> 

## <a name="permissions"></a><span data-ttu-id="44ccc-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44ccc-107">Permissions</span></span>
<span data-ttu-id="44ccc-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44ccc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44ccc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44ccc-110">Permission type</span></span>                        | <span data-ttu-id="44ccc-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44ccc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="44ccc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44ccc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="44ccc-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44ccc-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="44ccc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44ccc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44ccc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44ccc-115">Not supported.</span></span> |
|<span data-ttu-id="44ccc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44ccc-116">Application</span></span>                            | <span data-ttu-id="44ccc-117">AccessReview の構成</span><span class="sxs-lookup"><span data-stu-id="44ccc-117">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="44ccc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44ccc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/sendReminder()
```
## <a name="request-headers"></a><span data-ttu-id="44ccc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44ccc-119">Request headers</span></span>
| <span data-ttu-id="44ccc-120">名前</span><span class="sxs-lookup"><span data-stu-id="44ccc-120">Name</span></span>         | <span data-ttu-id="44ccc-121">型</span><span class="sxs-lookup"><span data-stu-id="44ccc-121">Type</span></span>        | <span data-ttu-id="44ccc-122">説明</span><span class="sxs-lookup"><span data-stu-id="44ccc-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="44ccc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44ccc-123">Authorization</span></span> | <span data-ttu-id="44ccc-124">string</span><span class="sxs-lookup"><span data-stu-id="44ccc-124">string</span></span> | <span data-ttu-id="44ccc-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="44ccc-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44ccc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="44ccc-127">Request body</span></span>
<span data-ttu-id="44ccc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44ccc-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="44ccc-129">応答</span><span class="sxs-lookup"><span data-stu-id="44ccc-129">Response</span></span>
<span data-ttu-id="44ccc-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="44ccc-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44ccc-132">例</span><span class="sxs-lookup"><span data-stu-id="44ccc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44ccc-133">要求</span><span class="sxs-lookup"><span data-stu-id="44ccc-133">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44ccc-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="44ccc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44ccc-135">C#</span><span class="sxs-lookup"><span data-stu-id="44ccc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44ccc-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="44ccc-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44ccc-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="44ccc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="44ccc-138">Java</span><span class="sxs-lookup"><span data-stu-id="44ccc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="44ccc-139">応答</span><span class="sxs-lookup"><span data-stu-id="44ccc-139">Response</span></span>
><span data-ttu-id="44ccc-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="44ccc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
