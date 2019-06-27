---
title: 範囲:LastRow
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e49d16493a3e5995cda9cf5b708d53918f892fad
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275370"
---
# <a name="range-lastrow"></a><span data-ttu-id="e9243-103">範囲:LastRow</span><span class="sxs-lookup"><span data-stu-id="e9243-103">Range: LastRow</span></span>

<span data-ttu-id="e9243-p101">範囲内の最後の行を取得します。たとえば、"B2:D5" の最後の行は "B5:D5" になります。</span><span class="sxs-lookup"><span data-stu-id="e9243-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="e9243-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e9243-106">Permissions</span></span>
<span data-ttu-id="e9243-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9243-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9243-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e9243-109">Permission type</span></span>      | <span data-ttu-id="e9243-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e9243-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9243-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e9243-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9243-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9243-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e9243-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e9243-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9243-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9243-114">Not supported.</span></span>    |
|<span data-ttu-id="e9243-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e9243-115">Application</span></span> | <span data-ttu-id="e9243-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9243-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9243-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e9243-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastRow

```
## <a name="request-headers"></a><span data-ttu-id="e9243-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9243-118">Request headers</span></span>
| <span data-ttu-id="e9243-119">名前</span><span class="sxs-lookup"><span data-stu-id="e9243-119">Name</span></span>       | <span data-ttu-id="e9243-120">説明</span><span class="sxs-lookup"><span data-stu-id="e9243-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e9243-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9243-121">Authorization</span></span>  | <span data-ttu-id="e9243-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e9243-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9243-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e9243-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e9243-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e9243-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9243-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e9243-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e9243-128">応答</span><span class="sxs-lookup"><span data-stu-id="e9243-128">Response</span></span>

<span data-ttu-id="e9243-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e9243-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9243-130">例</span><span class="sxs-lookup"><span data-stu-id="e9243-130">Example</span></span>
<span data-ttu-id="e9243-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e9243-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e9243-132">要求</span><span class="sxs-lookup"><span data-stu-id="e9243-132">Request</span></span>
<span data-ttu-id="e9243-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e9243-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastRow
```

##### <a name="response"></a><span data-ttu-id="e9243-134">応答</span><span class="sxs-lookup"><span data-stu-id="e9243-134">Response</span></span>
<span data-ttu-id="e9243-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e9243-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9243-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e9243-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e9243-139">C#</span><span class="sxs-lookup"><span data-stu-id="e9243-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_lastrow-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9243-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9243-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_lastrow-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e9243-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="e9243-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_lastrow-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-lastrow.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
