---
title: セッションを更新する
description: 'この API を使用して、既存のブックのセッションを更新します。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f5519d447c8e752a000ee8b260a383fb586cd7be
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278583"
---
# <a name="refresh-session"></a><span data-ttu-id="ae3ab-103">セッションを更新する</span><span class="sxs-lookup"><span data-stu-id="ae3ab-103">Refresh Session</span></span>

<span data-ttu-id="ae3ab-104">この API を使用して、既存のブックのセッションを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ae3ab-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae3ab-105">Permissions</span></span>
<span data-ttu-id="ae3ab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae3ab-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae3ab-108">Permission type</span></span>      | <span data-ttu-id="ae3ab-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae3ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae3ab-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae3ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae3ab-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae3ab-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ae3ab-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae3ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae3ab-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-113">Not supported.</span></span>    |
|<span data-ttu-id="ae3ab-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae3ab-114">Application</span></span> | <span data-ttu-id="ae3ab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae3ab-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae3ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="ae3ab-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae3ab-117">Request headers</span></span>
| <span data-ttu-id="ae3ab-118">名前</span><span class="sxs-lookup"><span data-stu-id="ae3ab-118">Name</span></span>       | <span data-ttu-id="ae3ab-119">説明</span><span class="sxs-lookup"><span data-stu-id="ae3ab-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ae3ab-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae3ab-120">Authorization</span></span>  | <span data-ttu-id="ae3ab-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ae3ab-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="ae3ab-123">workbook-session-id</span></span> | <span data-ttu-id="ae3ab-124">更新するブック セッションの ID</span><span class="sxs-lookup"><span data-stu-id="ae3ab-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae3ab-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae3ab-125">Request body</span></span>
<span data-ttu-id="ae3ab-126">この API は、要求本文を必要としません。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="ae3ab-127">応答</span><span class="sxs-lookup"><span data-stu-id="ae3ab-127">Response</span></span>

<span data-ttu-id="ae3ab-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ae3ab-129">例</span><span class="sxs-lookup"><span data-stu-id="ae3ab-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae3ab-130">要求</span><span class="sxs-lookup"><span data-stu-id="ae3ab-130">Request</span></span>
<span data-ttu-id="ae3ab-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="ae3ab-132">workbook-session-id ヘッダーが必要となることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="ae3ab-133">応答</span><span class="sxs-lookup"><span data-stu-id="ae3ab-133">Response</span></span>
<span data-ttu-id="ae3ab-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ae3ab-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ae3ab-135">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ae3ab-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ae3ab-136">C#</span><span class="sxs-lookup"><span data-stu-id="ae3ab-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/refresh_excel_session-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ae3ab-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ae3ab-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/refresh_excel_session-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ae3ab-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="ae3ab-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/refresh_excel_session-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbook-refreshsession.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/workbook-refreshsession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbook-refreshsession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Warning: refresh_excel_session//api-reference/v1.0/api/workbook-refreshsession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
