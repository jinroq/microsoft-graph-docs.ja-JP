---
title: ワークシート:UsedRange
description: 使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 147e5f31487281db9c3ec577a764fa90a9f96ede
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278268"
---
# <a name="worksheet-usedrange"></a><span data-ttu-id="5cdb6-104">ワークシート:UsedRange</span><span class="sxs-lookup"><span data-stu-id="5cdb6-104">Worksheet: UsedRange</span></span>

<span data-ttu-id="5cdb6-p102">使用範囲とは、値または書式設定が割り当たっているすべてのセルを包含する最小の範囲です。ワークシートが空白の場合、この関数は左上のセルを返します。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-p102">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>
## <a name="permissions"></a><span data-ttu-id="5cdb6-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5cdb6-107">Permissions</span></span>
<span data-ttu-id="5cdb6-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cdb6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5cdb6-110">Permission type</span></span>      | <span data-ttu-id="5cdb6-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5cdb6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5cdb6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5cdb6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5cdb6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5cdb6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5cdb6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5cdb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5cdb6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-115">Not supported.</span></span>    |
|<span data-ttu-id="5cdb6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5cdb6-116">Application</span></span> | <span data-ttu-id="5cdb6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5cdb6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5cdb6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/usedRange

```

## <a name="function-parameters"></a><span data-ttu-id="5cdb6-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="5cdb6-119">Function parameters</span></span>
<span data-ttu-id="5cdb6-120">要求 URL には、オプションのパラメーターを指定できます。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-120">In the request URL you may provide optional parameters.</span></span>

| <span data-ttu-id="5cdb6-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="5cdb6-121">Parameter</span></span>    | <span data-ttu-id="5cdb6-122">型</span><span class="sxs-lookup"><span data-stu-id="5cdb6-122">Type</span></span>   |<span data-ttu-id="5cdb6-123">説明</span><span class="sxs-lookup"><span data-stu-id="5cdb6-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cdb6-124">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="5cdb6-124">valuesOnly</span></span>|<span data-ttu-id="5cdb6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cdb6-125">Boolean</span></span>|<span data-ttu-id="5cdb6-p104">省略可能。値の入っているセルのみを使用セルと見なします (書式設定は無視されます)。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-p104">Optional. Considers only cells with values as used cells (ignores formatting).</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5cdb6-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5cdb6-128">Request headers</span></span>
| <span data-ttu-id="5cdb6-129">名前</span><span class="sxs-lookup"><span data-stu-id="5cdb6-129">Name</span></span>       | <span data-ttu-id="5cdb6-130">説明</span><span class="sxs-lookup"><span data-stu-id="5cdb6-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5cdb6-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cdb6-131">Authorization</span></span>  | <span data-ttu-id="5cdb6-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5cdb6-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5cdb6-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="5cdb6-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cdb6-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="5cdb6-137">Request body</span></span>
<span data-ttu-id="5cdb6-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cdb6-139">応答</span><span class="sxs-lookup"><span data-stu-id="5cdb6-139">Response</span></span>

<span data-ttu-id="5cdb6-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cdb6-141">例</span><span class="sxs-lookup"><span data-stu-id="5cdb6-141">Example</span></span>
<span data-ttu-id="5cdb6-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-142">Here is an example that shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5cdb6-143">要求</span><span class="sxs-lookup"><span data-stu-id="5cdb6-143">Request</span></span>
<span data-ttu-id="5cdb6-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange
```

##### <a name="response"></a><span data-ttu-id="5cdb6-145">応答</span><span class="sxs-lookup"><span data-stu-id="5cdb6-145">Response</span></span>
<span data-ttu-id="5cdb6-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5cdb6-149">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5cdb6-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5cdb6-150">C#</span><span class="sxs-lookup"><span data-stu-id="5cdb6-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_usedrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5cdb6-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="5cdb6-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_usedrange-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5cdb6-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="5cdb6-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheet_usedrange-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="5cdb6-153">また、この関数は、省略可能`valuesOnly`なパラメーターを指定して呼び出すこともできます。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-153">Alternatively, this function can be called with the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="5cdb6-154">要求</span><span class="sxs-lookup"><span data-stu-id="5cdb6-154">Request</span></span>
<span data-ttu-id="5cdb6-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-155">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "worksheet_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="5cdb6-156">応答</span><span class="sxs-lookup"><span data-stu-id="5cdb6-156">Response</span></span>
<span data-ttu-id="5cdb6-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5cdb6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5cdb6-160">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5cdb6-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5cdb6-161">C#</span><span class="sxs-lookup"><span data-stu-id="5cdb6-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/worksheet_usedrange_valuesonly-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5cdb6-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="5cdb6-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/worksheet_usedrange_valuesonly-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5cdb6-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="5cdb6-163">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/worksheet_usedrange_valuesonly-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/worksheet-usedrange.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/worksheet-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/worksheet-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/worksheet-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
