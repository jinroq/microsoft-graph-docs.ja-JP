---
title: 'ChartFill: clear'
description: グラフ要素の塗りつぶしの色をクリアします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c8a8f0af0a5cad8a9e347b001beb76024e8ad0d9
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635695"
---
# <a name="chartfill-clear"></a><span data-ttu-id="ced75-103">ChartFill: clear</span><span class="sxs-lookup"><span data-stu-id="ced75-103">ChartFill: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ced75-104">グラフ要素の塗りつぶしの色をクリアします。</span><span class="sxs-lookup"><span data-stu-id="ced75-104">Clear the fill color of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="ced75-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ced75-105">Permissions</span></span>
<span data-ttu-id="ced75-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ced75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ced75-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ced75-108">Permission type</span></span>      | <span data-ttu-id="ced75-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ced75-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ced75-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ced75-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ced75-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ced75-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ced75-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ced75-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ced75-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ced75-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ced75-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ced75-114">Application</span></span> | <span data-ttu-id="ced75-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ced75-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ced75-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ced75-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/title/format/fill/clear
POST /workbook/worksheets/{id|name}/charts/{name}/legend/format/fill/clear

```
## <a name="request-headers"></a><span data-ttu-id="ced75-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ced75-117">Request headers</span></span>
| <span data-ttu-id="ced75-118">名前</span><span class="sxs-lookup"><span data-stu-id="ced75-118">Name</span></span>       | <span data-ttu-id="ced75-119">説明</span><span class="sxs-lookup"><span data-stu-id="ced75-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ced75-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ced75-120">Authorization</span></span>  | <span data-ttu-id="ced75-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ced75-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ced75-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ced75-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ced75-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ced75-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ced75-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ced75-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ced75-127">応答</span><span class="sxs-lookup"><span data-stu-id="ced75-127">Response</span></span>

<span data-ttu-id="ced75-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ced75-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ced75-130">例</span><span class="sxs-lookup"><span data-stu-id="ced75-130">Example</span></span>
<span data-ttu-id="ced75-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ced75-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ced75-132">要求</span><span class="sxs-lookup"><span data-stu-id="ced75-132">Request</span></span>
<span data-ttu-id="ced75-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ced75-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chartfill_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear
```

##### <a name="response"></a><span data-ttu-id="ced75-134">応答</span><span class="sxs-lookup"><span data-stu-id="ced75-134">Response</span></span>
<span data-ttu-id="ced75-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ced75-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ced75-136">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="ced75-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ced75-137">Visual</span><span class="sxs-lookup"><span data-stu-id="ced75-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/chartfill_clear-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ced75-138">Java</span><span class="sxs-lookup"><span data-stu-id="ced75-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/chartfill_clear-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartFill: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartfill-clear.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/chartfill-clear.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
