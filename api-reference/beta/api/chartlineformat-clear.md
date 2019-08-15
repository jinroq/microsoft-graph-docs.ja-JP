---
title: 'ChartLineFormat: clear'
description: グラフ要素の線の書式をクリアします。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 603f13dd75b88df34fa788e876b68ebd08c437f6
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418377"
---
# <a name="chartlineformat-clear"></a><span data-ttu-id="6a2ba-103">ChartLineFormat: clear</span><span class="sxs-lookup"><span data-stu-id="6a2ba-103">ChartLineFormat: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a2ba-104">グラフ要素の線の書式をクリアします。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-104">Clear the line format of a chart element.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a2ba-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a2ba-105">Permissions</span></span>
<span data-ttu-id="6a2ba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a2ba-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a2ba-108">Permission type</span></span>      | <span data-ttu-id="6a2ba-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a2ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a2ba-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a2ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a2ba-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a2ba-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6a2ba-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a2ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a2ba-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6a2ba-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6a2ba-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a2ba-114">Application</span></span> | <span data-ttu-id="6a2ba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a2ba-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a2ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/categoryaxis/format/line/clear
POST /workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/majorgridlines/format/line/clear

```
## <a name="request-headers"></a><span data-ttu-id="6a2ba-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a2ba-117">Request headers</span></span>
| <span data-ttu-id="6a2ba-118">名前</span><span class="sxs-lookup"><span data-stu-id="6a2ba-118">Name</span></span>       | <span data-ttu-id="6a2ba-119">説明</span><span class="sxs-lookup"><span data-stu-id="6a2ba-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6a2ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a2ba-120">Authorization</span></span>  | <span data-ttu-id="6a2ba-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6a2ba-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6a2ba-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6a2ba-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a2ba-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a2ba-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="6a2ba-127">応答</span><span class="sxs-lookup"><span data-stu-id="6a2ba-127">Response</span></span>

<span data-ttu-id="6a2ba-p104">成功した場合、このメソッドは `200 OK` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a2ba-130">例</span><span class="sxs-lookup"><span data-stu-id="6a2ba-130">Example</span></span>
<span data-ttu-id="6a2ba-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6a2ba-132">要求</span><span class="sxs-lookup"><span data-stu-id="6a2ba-132">Request</span></span>
<span data-ttu-id="6a2ba-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a2ba-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6a2ba-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartlineformat_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a2ba-135">C#</span><span class="sxs-lookup"><span data-stu-id="6a2ba-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartlineformat-clear-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a2ba-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a2ba-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartlineformat-clear-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a2ba-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="6a2ba-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartlineformat-clear-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6a2ba-138">応答</span><span class="sxs-lookup"><span data-stu-id="6a2ba-138">Response</span></span>
<span data-ttu-id="6a2ba-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6a2ba-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLineFormat: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
