---
title: 範囲:セル
description: 行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。
ms.openlocfilehash: 641de24869d5a57b08f339b7552d67d07be7b75c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073782"
---
# <a name="range-cell"></a><span data-ttu-id="4a1ae-105">範囲:セル</span><span class="sxs-lookup"><span data-stu-id="4a1ae-105">Range: Cell</span></span>

> <span data-ttu-id="4a1ae-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a1ae-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a1ae-p103">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。以外このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。返されるセルは、範囲の左上のセルを基準に配置されます。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="4a1ae-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a1ae-111">Permissions</span></span>
<span data-ttu-id="4a1ae-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a1ae-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a1ae-114">Permission type</span></span>      | <span data-ttu-id="4a1ae-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a1ae-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a1ae-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a1ae-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4a1ae-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a1ae-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a1ae-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a1ae-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a1ae-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a1ae-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4a1ae-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a1ae-120">Application</span></span> | <span data-ttu-id="4a1ae-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a1ae-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a1ae-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Cell
GET /workbook/worksheets/{id|name}/range(address='<address>')/Cell
GET /workbook/tables/{id|name}/columns/{id|name}/range/Cell

```
## <a name="request-headers"></a><span data-ttu-id="4a1ae-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a1ae-123">Request headers</span></span>
| <span data-ttu-id="4a1ae-124">名前</span><span class="sxs-lookup"><span data-stu-id="4a1ae-124">Name</span></span>       | <span data-ttu-id="4a1ae-125">説明</span><span class="sxs-lookup"><span data-stu-id="4a1ae-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a1ae-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a1ae-126">Authorization</span></span>  | <span data-ttu-id="4a1ae-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a1ae-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4a1ae-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="4a1ae-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a1ae-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a1ae-132">Request body</span></span>
<span data-ttu-id="4a1ae-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4a1ae-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4a1ae-134">Parameter</span></span>    | <span data-ttu-id="4a1ae-135">型</span><span class="sxs-lookup"><span data-stu-id="4a1ae-135">Type</span></span>   |<span data-ttu-id="4a1ae-136">説明</span><span class="sxs-lookup"><span data-stu-id="4a1ae-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a1ae-137">row</span><span class="sxs-lookup"><span data-stu-id="4a1ae-137">row</span></span>|<span data-ttu-id="4a1ae-138">数値</span><span class="sxs-lookup"><span data-stu-id="4a1ae-138">number</span></span>|<span data-ttu-id="4a1ae-p107">取得するセルの行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-p107">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="4a1ae-141">列</span><span class="sxs-lookup"><span data-stu-id="4a1ae-141">column</span></span>|<span data-ttu-id="4a1ae-142">数値</span><span class="sxs-lookup"><span data-stu-id="4a1ae-142">number</span></span>|<span data-ttu-id="4a1ae-p108">取得セルの列番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-p108">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="4a1ae-145">応答</span><span class="sxs-lookup"><span data-stu-id="4a1ae-145">Response</span></span>

<span data-ttu-id="4a1ae-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a1ae-147">例</span><span class="sxs-lookup"><span data-stu-id="4a1ae-147">Example</span></span>
<span data-ttu-id="4a1ae-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4a1ae-149">要求</span><span class="sxs-lookup"><span data-stu-id="4a1ae-149">Request</span></span>
<span data-ttu-id="4a1ae-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="4a1ae-151">応答</span><span class="sxs-lookup"><span data-stu-id="4a1ae-151">Response</span></span>
<span data-ttu-id="4a1ae-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a1ae-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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