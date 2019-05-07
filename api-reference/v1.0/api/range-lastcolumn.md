---
title: 範囲:LastColumn
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d8b27aaf4786884bd933613aa97d4723c95a9bd0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33607851"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="1dae8-103">範囲:LastColumn</span><span class="sxs-lookup"><span data-stu-id="1dae8-103">Range: LastColumn</span></span>

<span data-ttu-id="1dae8-p101">範囲内の最後の列を取得します。たとえば、"B2:D5" の最後の列は "D2:D5" になります。</span><span class="sxs-lookup"><span data-stu-id="1dae8-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="1dae8-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1dae8-106">Permissions</span></span>
<span data-ttu-id="1dae8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dae8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dae8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1dae8-109">Permission type</span></span>      | <span data-ttu-id="1dae8-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1dae8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dae8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1dae8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1dae8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1dae8-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1dae8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1dae8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dae8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dae8-114">Not supported.</span></span>    |
|<span data-ttu-id="1dae8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1dae8-115">Application</span></span> | <span data-ttu-id="1dae8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1dae8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dae8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1dae8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/lastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/lastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/lastColumn

```
## <a name="request-headers"></a><span data-ttu-id="1dae8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1dae8-118">Request headers</span></span>
| <span data-ttu-id="1dae8-119">名前</span><span class="sxs-lookup"><span data-stu-id="1dae8-119">Name</span></span>       | <span data-ttu-id="1dae8-120">説明</span><span class="sxs-lookup"><span data-stu-id="1dae8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1dae8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dae8-121">Authorization</span></span>  | <span data-ttu-id="1dae8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1dae8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1dae8-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1dae8-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1dae8-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1dae8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dae8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1dae8-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="1dae8-128">応答</span><span class="sxs-lookup"><span data-stu-id="1dae8-128">Response</span></span>

<span data-ttu-id="1dae8-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1dae8-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dae8-130">例</span><span class="sxs-lookup"><span data-stu-id="1dae8-130">Example</span></span>
<span data-ttu-id="1dae8-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1dae8-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1dae8-132">要求</span><span class="sxs-lookup"><span data-stu-id="1dae8-132">Request</span></span>
<span data-ttu-id="1dae8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1dae8-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/lastColumn
```

##### <a name="response"></a><span data-ttu-id="1dae8-134">応答</span><span class="sxs-lookup"><span data-stu-id="1dae8-134">Response</span></span>
<span data-ttu-id="1dae8-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1dae8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1dae8-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1dae8-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1dae8-139">Visual</span><span class="sxs-lookup"><span data-stu-id="1dae8-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_lastcolumn-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1dae8-140">Java</span><span class="sxs-lookup"><span data-stu-id="1dae8-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_lastcolumn-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/range-lastcolumn.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/range-lastcolumn.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
