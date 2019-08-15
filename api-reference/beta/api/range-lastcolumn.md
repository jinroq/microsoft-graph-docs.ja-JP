---
title: 範囲:LastColumn
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: cdf03dec9d69ddc2d4c4d934de7a375f772f49e2
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412216"
---
# <a name="range-lastcolumn"></a><span data-ttu-id="9c699-103">範囲:LastColumn</span><span class="sxs-lookup"><span data-stu-id="9c699-103">Range: LastColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c699-p101">範囲内の最後の列を取得します。たとえば、"B2:D5" の最後の列は "D2:D5" になります。</span><span class="sxs-lookup"><span data-stu-id="9c699-p101">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="9c699-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9c699-106">Permissions</span></span>
<span data-ttu-id="9c699-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c699-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c699-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9c699-109">Permission type</span></span>      | <span data-ttu-id="9c699-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9c699-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c699-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9c699-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c699-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c699-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9c699-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9c699-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c699-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c699-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9c699-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9c699-115">Application</span></span> | <span data-ttu-id="9c699-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c699-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c699-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9c699-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/LastColumn
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastColumn
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastColumn

```
## <a name="request-headers"></a><span data-ttu-id="9c699-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c699-118">Request headers</span></span>
| <span data-ttu-id="9c699-119">名前</span><span class="sxs-lookup"><span data-stu-id="9c699-119">Name</span></span>       | <span data-ttu-id="9c699-120">説明</span><span class="sxs-lookup"><span data-stu-id="9c699-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9c699-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c699-121">Authorization</span></span>  | <span data-ttu-id="9c699-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9c699-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c699-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9c699-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9c699-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="9c699-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c699-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9c699-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9c699-128">応答</span><span class="sxs-lookup"><span data-stu-id="9c699-128">Response</span></span>

<span data-ttu-id="9c699-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9c699-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c699-130">例</span><span class="sxs-lookup"><span data-stu-id="9c699-130">Example</span></span>
<span data-ttu-id="9c699-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="9c699-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9c699-132">要求</span><span class="sxs-lookup"><span data-stu-id="9c699-132">Request</span></span>
<span data-ttu-id="9c699-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9c699-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9c699-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9c699-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "range_lastcolumn"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/{name}/range/LastColumn
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9c699-135">C#</span><span class="sxs-lookup"><span data-stu-id="9c699-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-lastcolumn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c699-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c699-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-lastcolumn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9c699-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="9c699-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-lastcolumn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9c699-138">応答</span><span class="sxs-lookup"><span data-stu-id="9c699-138">Response</span></span>
<span data-ttu-id="9c699-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9c699-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
