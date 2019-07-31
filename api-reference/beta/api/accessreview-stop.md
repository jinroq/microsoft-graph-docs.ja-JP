---
title: AccessReview を停止する
description: Azure AD access レビュー機能で、現在アクティブな accessReview を停止します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  (定期的なアクセスレビューが今後のインスタンスを開始しないようにするには、それを更新して、スケジュールされた終了日を変更します)。  アクセスレビューが停止すると、レビュー担当者は入力を行うことができなくなり、アクセスレビューの決定を適用できるようになります。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fd62615a3ed1adc51e1f497b58ed1834bfc0d07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945943"
---
# <a name="stop-accessreview"></a><span data-ttu-id="d2746-106">AccessReview を停止する</span><span class="sxs-lookup"><span data-stu-id="d2746-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2746-107">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、現在アクティブな[accessreview](../resources/accessreview.md)を停止します。</span><span class="sxs-lookup"><span data-stu-id="d2746-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="d2746-108">ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="d2746-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="d2746-109">(定期的なアクセスレビューが今後のインスタンスを開始しないようにするには、[それを更新して](accessreview-update.md)、スケジュールされた終了日を変更します)。</span><span class="sxs-lookup"><span data-stu-id="d2746-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="d2746-110">アクセスレビューが停止すると、レビュー担当者は入力を行うことができなくなり、アクセスレビューの決定を適用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="d2746-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2746-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2746-111">Permissions</span></span>
<span data-ttu-id="d2746-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2746-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2746-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2746-114">Permission type</span></span>                        | <span data-ttu-id="d2746-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2746-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2746-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2746-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2746-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2746-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d2746-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2746-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2746-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2746-119">Not supported.</span></span> |
|<span data-ttu-id="d2746-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2746-120">Application</span></span>                            | <span data-ttu-id="d2746-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2746-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d2746-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2746-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="d2746-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2746-123">Request headers</span></span>
| <span data-ttu-id="d2746-124">名前</span><span class="sxs-lookup"><span data-stu-id="d2746-124">Name</span></span>         | <span data-ttu-id="d2746-125">型</span><span class="sxs-lookup"><span data-stu-id="d2746-125">Type</span></span>        | <span data-ttu-id="d2746-126">説明</span><span class="sxs-lookup"><span data-stu-id="d2746-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d2746-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2746-127">Authorization</span></span> | <span data-ttu-id="d2746-128">string</span><span class="sxs-lookup"><span data-stu-id="d2746-128">string</span></span> | <span data-ttu-id="d2746-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2746-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2746-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2746-131">Request body</span></span>
<span data-ttu-id="d2746-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2746-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d2746-133">応答</span><span class="sxs-lookup"><span data-stu-id="d2746-133">Response</span></span>
<span data-ttu-id="d2746-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d2746-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2746-136">例</span><span class="sxs-lookup"><span data-stu-id="d2746-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2746-137">要求</span><span class="sxs-lookup"><span data-stu-id="d2746-137">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d2746-138">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d2746-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2746-139">C#</span><span class="sxs-lookup"><span data-stu-id="d2746-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2746-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2746-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2746-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="d2746-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2746-142">Java</span><span class="sxs-lookup"><span data-stu-id="d2746-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2746-143">応答</span><span class="sxs-lookup"><span data-stu-id="d2746-143">Response</span></span>
><span data-ttu-id="d2746-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d2746-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
