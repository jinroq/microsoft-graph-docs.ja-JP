---
title: ワークシート:セル
description: 行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 553a09f0619fb16d0e9ee7c1ac9fe8dfac4a3b14
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987307"
---
# <a name="worksheet-cell"></a><span data-ttu-id="8a51a-104">ワークシート:セル</span><span class="sxs-lookup"><span data-stu-id="8a51a-104">Worksheet: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a51a-p102">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="8a51a-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="8a51a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a51a-107">Permissions</span></span>
<span data-ttu-id="8a51a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a51a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a51a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a51a-110">Permission type</span></span>      | <span data-ttu-id="8a51a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a51a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a51a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a51a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a51a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a51a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a51a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a51a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a51a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8a51a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8a51a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a51a-116">Application</span></span> | <span data-ttu-id="8a51a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a51a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a51a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a51a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="8a51a-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a51a-119">Function parameters</span></span>
<span data-ttu-id="8a51a-120">要求パスに、次のパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="8a51a-120">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="8a51a-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a51a-121">Parameter</span></span>    | <span data-ttu-id="8a51a-122">型</span><span class="sxs-lookup"><span data-stu-id="8a51a-122">Type</span></span>   |<span data-ttu-id="8a51a-123">説明</span><span class="sxs-lookup"><span data-stu-id="8a51a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a51a-124">row</span><span class="sxs-lookup"><span data-stu-id="8a51a-124">row</span></span>|<span data-ttu-id="8a51a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="8a51a-125">Int32</span></span>|<span data-ttu-id="8a51a-p104">取得するセルの行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="8a51a-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="8a51a-128">column</span><span class="sxs-lookup"><span data-stu-id="8a51a-128">column</span></span>|<span data-ttu-id="8a51a-129">Int32</span><span class="sxs-lookup"><span data-stu-id="8a51a-129">Int32</span></span>|<span data-ttu-id="8a51a-130">取得セルの列番号。</span><span class="sxs-lookup"><span data-stu-id="8a51a-130">Column number of the cell to be retrieved.</span></span> <span data-ttu-id="8a51a-131">0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="8a51a-131">Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="8a51a-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a51a-132">Request headers</span></span>
| <span data-ttu-id="8a51a-133">名前</span><span class="sxs-lookup"><span data-stu-id="8a51a-133">Name</span></span>       | <span data-ttu-id="8a51a-134">説明</span><span class="sxs-lookup"><span data-stu-id="8a51a-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a51a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a51a-135">Authorization</span></span>  | <span data-ttu-id="8a51a-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a51a-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8a51a-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8a51a-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="8a51a-p107">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8a51a-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a51a-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a51a-141">Request body</span></span>
<span data-ttu-id="8a51a-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a51a-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a51a-143">応答</span><span class="sxs-lookup"><span data-stu-id="8a51a-143">Response</span></span>

<span data-ttu-id="8a51a-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/workbookrange.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8a51a-144">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a51a-145">例</span><span class="sxs-lookup"><span data-stu-id="8a51a-145">Example</span></span>
<span data-ttu-id="8a51a-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="8a51a-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a51a-147">要求</span><span class="sxs-lookup"><span data-stu-id="8a51a-147">Request</span></span>
<span data-ttu-id="8a51a-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a51a-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="8a51a-149">応答</span><span class="sxs-lookup"><span data-stu-id="8a51a-149">Response</span></span>
<span data-ttu-id="8a51a-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a51a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "cellCount": 1,
  "columnCount": 1,
  "columnIndex": 3,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
