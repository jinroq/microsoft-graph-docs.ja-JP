---
title: accessreview を停止する
description: Azure AD access レビュー機能で、現在アクティブな accessreview を停止します。  ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。  (定期的なアクセスレビューが今後のインスタンスを開始しないようにするには、それを更新して、スケジュールされた終了日を変更します)。  アクセスレビューが停止すると、レビュー担当者は入力を行うことができなくなり、アクセスレビューの決定を適用できるようになります。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 070f91faa411fcc6d98db419d1683a7fb6493859
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459488"
---
# <a name="stop-accessreview"></a><span data-ttu-id="0d8f8-106">accessreview を停止する</span><span class="sxs-lookup"><span data-stu-id="0d8f8-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d8f8-107">Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、現在アクティブな[accessreview](../resources/accessreview.md)を停止します。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="0d8f8-108">ターゲットオブジェクトは、1回限りのアクセスレビュー、または定期的なアクセスレビューのインスタンスのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="0d8f8-109">(定期的なアクセスレビューが今後のインスタンスを開始しないようにするには、[それを更新して](accessreview-update.md)、スケジュールされた終了日を変更します)。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="0d8f8-110">アクセスレビューが停止すると、レビュー担当者は入力を行うことができなくなり、アクセスレビューの決定を適用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d8f8-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0d8f8-111">Permissions</span></span>
<span data-ttu-id="0d8f8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d8f8-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d8f8-114">Permission type</span></span>                        | <span data-ttu-id="0d8f8-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d8f8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d8f8-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d8f8-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d8f8-117">accessreview すべて</span><span class="sxs-lookup"><span data-stu-id="0d8f8-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0d8f8-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d8f8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d8f8-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-119">Not supported.</span></span> |
|<span data-ttu-id="0d8f8-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d8f8-120">Application</span></span>                            | <span data-ttu-id="0d8f8-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d8f8-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d8f8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="0d8f8-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d8f8-123">Request headers</span></span>
| <span data-ttu-id="0d8f8-124">名前</span><span class="sxs-lookup"><span data-stu-id="0d8f8-124">Name</span></span>         | <span data-ttu-id="0d8f8-125">型</span><span class="sxs-lookup"><span data-stu-id="0d8f8-125">Type</span></span>        | <span data-ttu-id="0d8f8-126">説明</span><span class="sxs-lookup"><span data-stu-id="0d8f8-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0d8f8-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d8f8-127">Authorization</span></span> | <span data-ttu-id="0d8f8-128">string</span><span class="sxs-lookup"><span data-stu-id="0d8f8-128">string</span></span> | <span data-ttu-id="0d8f8-p104">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d8f8-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d8f8-131">Request body</span></span>
<span data-ttu-id="0d8f8-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0d8f8-133">応答</span><span class="sxs-lookup"><span data-stu-id="0d8f8-133">Response</span></span>
<span data-ttu-id="0d8f8-p105">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d8f8-136">例</span><span class="sxs-lookup"><span data-stu-id="0d8f8-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d8f8-137">要求</span><span class="sxs-lookup"><span data-stu-id="0d8f8-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a><span data-ttu-id="0d8f8-138">応答</span><span class="sxs-lookup"><span data-stu-id="0d8f8-138">Response</span></span>
><span data-ttu-id="0d8f8-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="0d8f8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/accessreview-stop.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
