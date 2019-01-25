---
title: ワークシート:セル
description: 行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4649a361ec46b9fb904cf959608fdee502f05c22
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520558"
---
# <a name="worksheet-cell"></a><span data-ttu-id="19f0b-104">ワークシート:セル</span><span class="sxs-lookup"><span data-stu-id="19f0b-104">Worksheet: Cell</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19f0b-p102">行と列の番号に基づいて、1 つのセルを含んだ範囲オブジェクトを取得します。このセルは、ワークシートのグリッド内であれば、親の範囲の境界の外のセルであってもかまいません。</span><span class="sxs-lookup"><span data-stu-id="19f0b-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>
## <a name="permissions"></a><span data-ttu-id="19f0b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19f0b-107">Permissions</span></span>
<span data-ttu-id="19f0b-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19f0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19f0b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19f0b-110">Permission type</span></span>      | <span data-ttu-id="19f0b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19f0b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19f0b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19f0b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19f0b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19f0b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19f0b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19f0b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19f0b-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19f0b-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19f0b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19f0b-116">Application</span></span> | <span data-ttu-id="19f0b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19f0b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19f0b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19f0b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/Cell(row={row},column={column})

```

## <a name="function-parameters"></a><span data-ttu-id="19f0b-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="19f0b-119">Function parameters</span></span>
<span data-ttu-id="19f0b-120">要求のパスには、次のパラメーターを提供します。</span><span class="sxs-lookup"><span data-stu-id="19f0b-120">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="19f0b-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="19f0b-121">Parameter</span></span>    | <span data-ttu-id="19f0b-122">型</span><span class="sxs-lookup"><span data-stu-id="19f0b-122">Type</span></span>   |<span data-ttu-id="19f0b-123">説明</span><span class="sxs-lookup"><span data-stu-id="19f0b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19f0b-124">row</span><span class="sxs-lookup"><span data-stu-id="19f0b-124">row</span></span>|<span data-ttu-id="19f0b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="19f0b-125">Int32</span></span>|<span data-ttu-id="19f0b-p104">取得するセルの行番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="19f0b-p104">Row number of the cell to be retrieved. Zero-indexed.</span></span>|
|<span data-ttu-id="19f0b-128">列</span><span class="sxs-lookup"><span data-stu-id="19f0b-128">column</span></span>|<span data-ttu-id="19f0b-129">Int32</span><span class="sxs-lookup"><span data-stu-id="19f0b-129">Int32</span></span>|<span data-ttu-id="19f0b-p105">取得セルの列番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="19f0b-p105">Column number of the cell to be retrieved. Zero-indexed.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="19f0b-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19f0b-132">Request headers</span></span>
| <span data-ttu-id="19f0b-133">名前</span><span class="sxs-lookup"><span data-stu-id="19f0b-133">Name</span></span>       | <span data-ttu-id="19f0b-134">説明</span><span class="sxs-lookup"><span data-stu-id="19f0b-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19f0b-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="19f0b-135">Authorization</span></span>  | <span data-ttu-id="19f0b-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19f0b-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19f0b-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="19f0b-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="19f0b-p107">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="19f0b-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19f0b-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="19f0b-141">Request body</span></span>
<span data-ttu-id="19f0b-142">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="19f0b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19f0b-143">応答</span><span class="sxs-lookup"><span data-stu-id="19f0b-143">Response</span></span>

<span data-ttu-id="19f0b-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="19f0b-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19f0b-145">例</span><span class="sxs-lookup"><span data-stu-id="19f0b-145">Example</span></span>
<span data-ttu-id="19f0b-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="19f0b-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="19f0b-147">要求</span><span class="sxs-lookup"><span data-stu-id="19f0b-147">Request</span></span>
<span data-ttu-id="19f0b-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="19f0b-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_cell"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/Cell(row=<row>,column=<column>)
```

##### <a name="response"></a><span data-ttu-id="19f0b-149">応答</span><span class="sxs-lookup"><span data-stu-id="19f0b-149">Response</span></span>
<span data-ttu-id="19f0b-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="19f0b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet: Cell",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/worksheet-cell.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
