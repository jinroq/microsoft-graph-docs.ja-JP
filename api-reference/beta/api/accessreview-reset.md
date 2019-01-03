---
title: AccessReview をリセットします。
description: Azure AD アクセスでは、レビュー機能は、現在アクティブな accessReview の決定をリセットします。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。  以前の決定は記録されなくが、校閲者が意思決定を更新するのには続行できます。
ms.openlocfilehash: b633a56926b56b33c509214d7574971056831967
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067683"
---
# <a name="reset-accessreview"></a><span data-ttu-id="18ee4-105">AccessReview をリセットします。</span><span class="sxs-lookup"><span data-stu-id="18ee4-105">Reset accessReview</span></span>

> <span data-ttu-id="18ee4-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18ee4-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18ee4-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18ee4-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18ee4-108">Azure AD では、 [access](../resources/accessreviews-root.md)の機能は、現在アクティブな[accessReview](../resources/accessreview.md)の決定をリセットします。</span><span class="sxs-lookup"><span data-stu-id="18ee4-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="18ee4-109">ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="18ee4-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="18ee4-110">以前の決定は記録されなくが、校閲者が意思決定を更新するのには続行できます。</span><span class="sxs-lookup"><span data-stu-id="18ee4-110">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="18ee4-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="18ee4-111">Permissions</span></span>
<span data-ttu-id="18ee4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18ee4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18ee4-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18ee4-114">Permission type</span></span>                        | <span data-ttu-id="18ee4-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="18ee4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="18ee4-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18ee4-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="18ee4-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18ee4-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="18ee4-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18ee4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18ee4-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18ee4-119">Not supported.</span></span> |
|<span data-ttu-id="18ee4-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18ee4-120">Application</span></span>                            | <span data-ttu-id="18ee4-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18ee4-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18ee4-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18ee4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="18ee4-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18ee4-123">Request headers</span></span>
| <span data-ttu-id="18ee4-124">名前</span><span class="sxs-lookup"><span data-stu-id="18ee4-124">Name</span></span>         | <span data-ttu-id="18ee4-125">型</span><span class="sxs-lookup"><span data-stu-id="18ee4-125">Type</span></span>        | <span data-ttu-id="18ee4-126">説明</span><span class="sxs-lookup"><span data-stu-id="18ee4-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="18ee4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="18ee4-127">Authorization</span></span> | <span data-ttu-id="18ee4-128">string</span><span class="sxs-lookup"><span data-stu-id="18ee4-128">string</span></span> | <span data-ttu-id="18ee4-129">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="18ee4-129">Bearer \{token\}.</span></span> <span data-ttu-id="18ee4-130">必須。</span><span class="sxs-lookup"><span data-stu-id="18ee4-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18ee4-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="18ee4-131">Request body</span></span>
<span data-ttu-id="18ee4-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="18ee4-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="18ee4-133">応答</span><span class="sxs-lookup"><span data-stu-id="18ee4-133">Response</span></span>
<span data-ttu-id="18ee4-p106">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="18ee4-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18ee4-136">例</span><span class="sxs-lookup"><span data-stu-id="18ee4-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18ee4-137">要求</span><span class="sxs-lookup"><span data-stu-id="18ee4-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="18ee4-138">応答</span><span class="sxs-lookup"><span data-stu-id="18ee4-138">Response</span></span>
><span data-ttu-id="18ee4-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="18ee4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->