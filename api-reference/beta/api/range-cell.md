---
title: 範囲:セル
description: 行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ef9888c934a0d85f66c49e062074c2c328cafa13
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915656"
---
# <a name="range-cell"></a><span data-ttu-id="f7847-105">範囲:セル</span><span class="sxs-lookup"><span data-stu-id="f7847-105">Range: Cell</span></span>

> <span data-ttu-id="f7847-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f7847-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7847-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7847-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7847-p103">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。</span><span class="sxs-lookup"><span data-stu-id="f7847-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7847-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7847-111">Permissions</span></span>
<span data-ttu-id="f7847-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7847-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7847-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f7847-114">Permission type</span></span>      | <span data-ttu-id="f7847-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f7847-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7847-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f7847-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f7847-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7847-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7847-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f7847-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7847-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7847-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f7847-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f7847-120">Application</span></span> | <span data-ttu-id="f7847-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7847-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7847-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f7847-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="f7847-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7847-123">Request headers</span></span>
| <span data-ttu-id="f7847-124">名前</span><span class="sxs-lookup"><span data-stu-id="f7847-124">Name</span></span>       | <span data-ttu-id="f7847-125">説明</span><span class="sxs-lookup"><span data-stu-id="f7847-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7847-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7847-126">Authorization</span></span>  | <span data-ttu-id="f7847-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f7847-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7847-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f7847-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="f7847-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f7847-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7847-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="f7847-132">Request body</span></span>
<span data-ttu-id="f7847-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f7847-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7847-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f7847-134">Parameter</span></span>    | <span data-ttu-id="f7847-135">型</span><span class="sxs-lookup"><span data-stu-id="f7847-135">Type</span></span>   |<span data-ttu-id="f7847-136">説明</span><span class="sxs-lookup"><span data-stu-id="f7847-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7847-137">row</span><span class="sxs-lookup"><span data-stu-id="f7847-137">row</span></span>|<span data-ttu-id="f7847-138">number</span><span class="sxs-lookup"><span data-stu-id="f7847-138">number</span></span>|<span data-ttu-id="f7847-p107">取得するセルの行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="f7847-p107">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="f7847-141">列</span><span class="sxs-lookup"><span data-stu-id="f7847-141">column</span></span>|<span data-ttu-id="f7847-142">number</span><span class="sxs-lookup"><span data-stu-id="f7847-142">number</span></span>|<span data-ttu-id="f7847-p108">取得セルの列番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="f7847-p108">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="f7847-145">応答</span><span class="sxs-lookup"><span data-stu-id="f7847-145">Response</span></span>

<span data-ttu-id="f7847-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f7847-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7847-147">例</span><span class="sxs-lookup"><span data-stu-id="f7847-147">Example</span></span>
<span data-ttu-id="f7847-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f7847-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f7847-149">要求</span><span class="sxs-lookup"><span data-stu-id="f7847-149">Request</span></span>
<span data-ttu-id="f7847-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f7847-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Cell
Content-type: application/json
Content-length: 37

{
  "row": {
  },
  "column": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="f7847-151">応答</span><span class="sxs-lookup"><span data-stu-id="f7847-151">Response</span></span>
<span data-ttu-id="f7847-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f7847-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
<!-- {
  "type": "#page.annotation",
  "description": "Range: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
