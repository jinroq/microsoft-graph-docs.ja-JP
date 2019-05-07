---
title: 範囲:UsedRange
description: 指定した範囲オブジェクトのうち使用されている範囲を返します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 97ea9cd720b38b774aa262eee53a1457bc2c842d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607943"
---
# <a name="range-usedrange"></a><span data-ttu-id="ed28a-103">範囲:UsedRange</span><span class="sxs-lookup"><span data-stu-id="ed28a-103">Range: UsedRange</span></span>

<span data-ttu-id="ed28a-104">指定した範囲オブジェクトのうち使用されている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="ed28a-104">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ed28a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ed28a-105">Permissions</span></span>
<span data-ttu-id="ed28a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed28a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed28a-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed28a-108">Permission type</span></span>      | <span data-ttu-id="ed28a-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed28a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed28a-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed28a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ed28a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed28a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ed28a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed28a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed28a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed28a-113">Not supported.</span></span>    |
|<span data-ttu-id="ed28a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed28a-114">Application</span></span> | <span data-ttu-id="ed28a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed28a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed28a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed28a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/usedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/usedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/usedRange

```
## <a name="request-headers"></a><span data-ttu-id="ed28a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed28a-117">Request headers</span></span>
| <span data-ttu-id="ed28a-118">名前</span><span class="sxs-lookup"><span data-stu-id="ed28a-118">Name</span></span>       | <span data-ttu-id="ed28a-119">説明</span><span class="sxs-lookup"><span data-stu-id="ed28a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ed28a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed28a-120">Authorization</span></span>  | <span data-ttu-id="ed28a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ed28a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed28a-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ed28a-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ed28a-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="ed28a-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="ed28a-126">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed28a-126">Path parameters</span></span>
| <span data-ttu-id="ed28a-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="ed28a-127">Parameter</span></span>    | <span data-ttu-id="ed28a-128">型</span><span class="sxs-lookup"><span data-stu-id="ed28a-128">Type</span></span>   |<span data-ttu-id="ed28a-129">説明</span><span class="sxs-lookup"><span data-stu-id="ed28a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed28a-130">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="ed28a-130">valuesOnly</span></span>|<span data-ttu-id="ed28a-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="ed28a-131">boolean</span></span>|<span data-ttu-id="ed28a-p104">省略可能。値の入っているセルのみを使用セルと見なします。</span><span class="sxs-lookup"><span data-stu-id="ed28a-p104">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="ed28a-134">応答</span><span class="sxs-lookup"><span data-stu-id="ed28a-134">Response</span></span>

<span data-ttu-id="ed28a-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ed28a-135">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed28a-136">例</span><span class="sxs-lookup"><span data-stu-id="ed28a-136">Example</span></span>
<span data-ttu-id="ed28a-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="ed28a-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ed28a-138">要求</span><span class="sxs-lookup"><span data-stu-id="ed28a-138">Request</span></span>
<span data-ttu-id="ed28a-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed28a-139">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange
```

##### <a name="response"></a><span data-ttu-id="ed28a-140">応答</span><span class="sxs-lookup"><span data-stu-id="ed28a-140">Response</span></span>
<span data-ttu-id="ed28a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ed28a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ed28a-144">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="ed28a-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ed28a-145">Visual</span><span class="sxs-lookup"><span data-stu-id="ed28a-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_usedrange-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed28a-146">Java</span><span class="sxs-lookup"><span data-stu-id="ed28a-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_usedrange-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="ed28a-147">省略可能`valuesOnly`なパラメーターを指定する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ed28a-147">Here is an example specifying the optional `valuesOnly` parameter.</span></span>

##### <a name="request"></a><span data-ttu-id="ed28a-148">要求</span><span class="sxs-lookup"><span data-stu-id="ed28a-148">Request</span></span>
<span data-ttu-id="ed28a-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ed28a-149">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_usedrange_valuesonly"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)
```

##### <a name="response"></a><span data-ttu-id="ed28a-150">応答</span><span class="sxs-lookup"><span data-stu-id="ed28a-150">Response</span></span>

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
  "cellCount": 90,
  "columnCount": 90,
  "columnIndex": 90,
  "valueTypes": "valueTypes-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ed28a-151">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="ed28a-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ed28a-152">Visual</span><span class="sxs-lookup"><span data-stu-id="ed28a-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_usedrange_valuesonly-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed28a-153">Java</span><span class="sxs-lookup"><span data-stu-id="ed28a-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_usedrange_valuesonly-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-usedrange.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
