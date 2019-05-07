---
title: セッションを閉じる
description: 'この API を使用して、既存のブック セッションを閉じます。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4c348690e0fbe8942ddea31102adc02c08707036
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33600723"
---
# <a name="close-session"></a><span data-ttu-id="7be3c-103">セッションを閉じる</span><span class="sxs-lookup"><span data-stu-id="7be3c-103">Close Session</span></span>

<span data-ttu-id="7be3c-104">この API を使用して、既存のブック セッションを閉じます。</span><span class="sxs-lookup"><span data-stu-id="7be3c-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7be3c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7be3c-105">Permissions</span></span>
<span data-ttu-id="7be3c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7be3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7be3c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7be3c-108">Permission type</span></span>      | <span data-ttu-id="7be3c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7be3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7be3c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7be3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7be3c-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7be3c-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7be3c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7be3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7be3c-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7be3c-113">Not supported.</span></span>    |
|<span data-ttu-id="7be3c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7be3c-114">Application</span></span> | <span data-ttu-id="7be3c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7be3c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7be3c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7be3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="7be3c-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7be3c-117">Request headers</span></span>
| <span data-ttu-id="7be3c-118">名前</span><span class="sxs-lookup"><span data-stu-id="7be3c-118">Name</span></span>       | <span data-ttu-id="7be3c-119">説明</span><span class="sxs-lookup"><span data-stu-id="7be3c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7be3c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7be3c-120">Authorization</span></span>  | <span data-ttu-id="7be3c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7be3c-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="7be3c-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7be3c-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7be3c-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7be3c-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="7be3c-126">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="7be3c-126">workbook-session-id</span></span> | <span data-ttu-id="7be3c-127">閉じるブック セッションの ID</span><span class="sxs-lookup"><span data-stu-id="7be3c-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="7be3c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7be3c-128">Request body</span></span>
<span data-ttu-id="7be3c-129">この API は、要求本文を必要としません。</span><span class="sxs-lookup"><span data-stu-id="7be3c-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="7be3c-130">応答</span><span class="sxs-lookup"><span data-stu-id="7be3c-130">Response</span></span>

<span data-ttu-id="7be3c-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7be3c-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7be3c-132">例</span><span class="sxs-lookup"><span data-stu-id="7be3c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7be3c-133">要求</span><span class="sxs-lookup"><span data-stu-id="7be3c-133">Request</span></span>
<span data-ttu-id="7be3c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7be3c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="7be3c-135">workbook-session-id ヘッダーが必要となることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="7be3c-135">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="7be3c-136">応答</span><span class="sxs-lookup"><span data-stu-id="7be3c-136">Response</span></span>
<span data-ttu-id="7be3c-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7be3c-137">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7be3c-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="7be3c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7be3c-139">Visual</span><span class="sxs-lookup"><span data-stu-id="7be3c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/close_excel_session-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7be3c-140">Java</span><span class="sxs-lookup"><span data-stu-id="7be3c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/close_excel_session-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/workbook-closesession.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
