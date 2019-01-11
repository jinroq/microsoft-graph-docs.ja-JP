---
title: AccessReview を停止します。
description: Azure AD のレビュー機能にアクセス、現在アクティブな accessReview を停止します。  ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。  (定期的なアクセス確認が将来のインスタンスを開始しないように、更新のスケジュールされた終了日を変更するのには)。  アクセスの後、停止を確認、レビュー担当者は、入力を与えることが不要になったアクセス レビューの決定を適用することができます。
localization_priority: Normal
ms.openlocfilehash: 57c0473b58b8ca4bbbb4e9f182b7da4582af4c38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860117"
---
# <a name="stop-accessreview"></a><span data-ttu-id="ff3cf-106">AccessReview を停止します。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-106">Stop accessReview</span></span>

> <span data-ttu-id="ff3cf-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff3cf-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff3cf-109">Azure AD[アクセスの確認](../resources/accessreviews-root.md)機能では、現在アクティブな[accessReview](../resources/accessreview.md)を停止します。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-109">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="ff3cf-110">ターゲット オブジェクトは、1 回限りのアクセスの確認、または定期的なアクセス確認のインスタンスのいずれかにできます。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-110">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="ff3cf-111">(防ぐためのアクセス確認を定期的な[更新](accessreview-update.md)のスケジュールされた終了日を変更するのには、将来のインスタンスを開始)。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-111">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="ff3cf-112">アクセスの後、停止を確認、レビュー担当者は、入力を与えることが不要になったアクセス レビューの決定を適用することができます。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-112">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff3cf-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff3cf-113">Permissions</span></span>
<span data-ttu-id="ff3cf-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff3cf-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff3cf-116">Permission type</span></span>                        | <span data-ttu-id="ff3cf-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff3cf-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff3cf-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff3cf-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="ff3cf-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff3cf-119">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="ff3cf-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff3cf-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff3cf-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-121">Not supported.</span></span> |
|<span data-ttu-id="ff3cf-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff3cf-122">Application</span></span>                            | <span data-ttu-id="ff3cf-123">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff3cf-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff3cf-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="ff3cf-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff3cf-125">Request headers</span></span>
| <span data-ttu-id="ff3cf-126">名前</span><span class="sxs-lookup"><span data-stu-id="ff3cf-126">Name</span></span>         | <span data-ttu-id="ff3cf-127">種類</span><span class="sxs-lookup"><span data-stu-id="ff3cf-127">Type</span></span>        | <span data-ttu-id="ff3cf-128">説明</span><span class="sxs-lookup"><span data-stu-id="ff3cf-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ff3cf-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff3cf-129">Authorization</span></span> | <span data-ttu-id="ff3cf-130">string</span><span class="sxs-lookup"><span data-stu-id="ff3cf-130">string</span></span> | <span data-ttu-id="ff3cf-131">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-131">Bearer \{token\}.</span></span> <span data-ttu-id="ff3cf-132">必須。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff3cf-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff3cf-133">Request body</span></span>
<span data-ttu-id="ff3cf-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-134">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="ff3cf-135">応答</span><span class="sxs-lookup"><span data-stu-id="ff3cf-135">Response</span></span>
<span data-ttu-id="ff3cf-p106">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff3cf-138">例</span><span class="sxs-lookup"><span data-stu-id="ff3cf-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff3cf-139">要求</span><span class="sxs-lookup"><span data-stu-id="ff3cf-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="ff3cf-140">応答</span><span class="sxs-lookup"><span data-stu-id="ff3cf-140">Response</span></span>
><span data-ttu-id="ff3cf-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff3cf-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
