---
title: ワークシート:セル
description: 行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。
ms.openlocfilehash: 5c85bf21e88b6b483abe1631c038e9239d3779d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067928"
---
# <a name="worksheet-cell"></a><span data-ttu-id="c8c38-104">ワークシート:セル</span><span class="sxs-lookup"><span data-stu-id="c8c38-104">Worksheet: Cell</span></span>

> <span data-ttu-id="c8c38-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8c38-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8c38-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8c38-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8c38-p103">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="c8c38-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8c38-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c8c38-109">Permissions</span></span>
<span data-ttu-id="c8c38-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8c38-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c38-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8c38-112">Permission type</span></span>      | <span data-ttu-id="c8c38-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8c38-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8c38-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8c38-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c8c38-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8c38-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8c38-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8c38-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8c38-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8c38-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8c38-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8c38-118">Application</span></span> | <span data-ttu-id="c8c38-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8c38-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8c38-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8c38-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="c8c38-121">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8c38-121">Function parameters</span></span>
<span data-ttu-id="c8c38-122">要求のパスには、次のパラメーターを提供します。</span><span class="sxs-lookup"><span data-stu-id="c8c38-122">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="c8c38-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8c38-123">Parameter</span></span>    | <span data-ttu-id="c8c38-124">型</span><span class="sxs-lookup"><span data-stu-id="c8c38-124">Type</span></span>   |<span data-ttu-id="c8c38-125">説明</span><span class="sxs-lookup"><span data-stu-id="c8c38-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8c38-126">row</span><span class="sxs-lookup"><span data-stu-id="c8c38-126">row</span></span>|<span data-ttu-id="c8c38-127">Int32</span><span class="sxs-lookup"><span data-stu-id="c8c38-127">Int32</span></span>|<span data-ttu-id="c8c38-p105">取得するセルの行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="c8c38-p105">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="c8c38-130">列</span><span class="sxs-lookup"><span data-stu-id="c8c38-130">column</span></span>|<span data-ttu-id="c8c38-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c8c38-131">Int32</span></span>|<span data-ttu-id="c8c38-p106">取得セルの列番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="c8c38-p106">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c8c38-134">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8c38-134">Request headers</span></span>
| <span data-ttu-id="c8c38-135">名前</span><span class="sxs-lookup"><span data-stu-id="c8c38-135">Name</span></span>       | <span data-ttu-id="c8c38-136">説明</span><span class="sxs-lookup"><span data-stu-id="c8c38-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8c38-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8c38-137">Authorization</span></span>  | <span data-ttu-id="c8c38-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c8c38-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8c38-140">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c8c38-140">Workbook-Session-Id</span></span>  | <span data-ttu-id="c8c38-p108">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c8c38-p108">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8c38-143">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8c38-143">Request body</span></span>
<span data-ttu-id="c8c38-144">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c8c38-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8c38-145">応答</span><span class="sxs-lookup"><span data-stu-id="c8c38-145">Response</span></span>

<span data-ttu-id="c8c38-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8c38-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8c38-147">例</span><span class="sxs-lookup"><span data-stu-id="c8c38-147">Example</span></span>
<span data-ttu-id="c8c38-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="c8c38-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c8c38-149">要求</span><span class="sxs-lookup"><span data-stu-id="c8c38-149">Request</span></span>
<span data-ttu-id="c8c38-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8c38-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="c8c38-151">応答</span><span class="sxs-lookup"><span data-stu-id="c8c38-151">Response</span></span>
<span data-ttu-id="c8c38-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8c38-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->