---
title: 'workbookChartCollection: 追加'
description: 新しい workbookChart を作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e0f38029688d924b1280e03b557b2d2b76653910
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864148"
---
# <a name="workbookchartcollection-add"></a><span data-ttu-id="2013f-103">workbookChartCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="2013f-103">workbookChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2013f-104">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="2013f-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="2013f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2013f-105">Permissions</span></span>
<span data-ttu-id="2013f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2013f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2013f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2013f-108">Permission type</span></span>      | <span data-ttu-id="2013f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2013f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2013f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2013f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2013f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2013f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2013f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2013f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2013f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2013f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2013f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2013f-114">Application</span></span> | <span data-ttu-id="2013f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2013f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2013f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2013f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="2013f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2013f-117">Request headers</span></span>
| <span data-ttu-id="2013f-118">名前</span><span class="sxs-lookup"><span data-stu-id="2013f-118">Name</span></span>       | <span data-ttu-id="2013f-119">説明</span><span class="sxs-lookup"><span data-stu-id="2013f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2013f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2013f-120">Authorization</span></span>  | <span data-ttu-id="2013f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2013f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2013f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2013f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="2013f-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="2013f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2013f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2013f-126">Request body</span></span>
<span data-ttu-id="2013f-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2013f-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2013f-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2013f-128">Parameter</span></span>    | <span data-ttu-id="2013f-129">型</span><span class="sxs-lookup"><span data-stu-id="2013f-129">Type</span></span>   |<span data-ttu-id="2013f-130">説明</span><span class="sxs-lookup"><span data-stu-id="2013f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2013f-131">type</span><span class="sxs-lookup"><span data-stu-id="2013f-131">type</span></span>|<span data-ttu-id="2013f-132">string</span><span class="sxs-lookup"><span data-stu-id="2013f-132">string</span></span>|<span data-ttu-id="2013f-133">グラフの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="2013f-133">Represents the type of a chart.</span></span>  <span data-ttu-id="2013f-134">使用可能な値は`ColumnClustered`、 `ColumnStacked`、 `ColumnStacked100` `BarClustered` `BarStacked` `BarStacked100` `LineStacked` `PieOfPie` `etc.`、、、、、、、、、、、、です。 `LineStacked100` `LineMarkers` `LineMarkersStacked` `LineMarkersStacked100`</span><span class="sxs-lookup"><span data-stu-id="2013f-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="2013f-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="2013f-135">sourceData</span></span>|<span data-ttu-id="2013f-136">Json</span><span class="sxs-lookup"><span data-stu-id="2013f-136">Json</span></span>|<span data-ttu-id="2013f-137">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2013f-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="2013f-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="2013f-138">seriesBy</span></span>|<span data-ttu-id="2013f-139">string</span><span class="sxs-lookup"><span data-stu-id="2013f-139">string</span></span>|<span data-ttu-id="2013f-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2013f-140">Optional.</span></span> <span data-ttu-id="2013f-141">列や行がグラフのデータ系列として使用される方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="2013f-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="2013f-142">使用可能な値: `Auto`、`Columns`、`Rows`。</span><span class="sxs-lookup"><span data-stu-id="2013f-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="2013f-143">応答</span><span class="sxs-lookup"><span data-stu-id="2013f-143">Response</span></span>

<span data-ttu-id="2013f-144">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[workbookChart](../resources/workbookchart.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2013f-144">If successful, this method returns `200 OK` response code and [workbookChart](../resources/workbookchart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2013f-145">例</span><span class="sxs-lookup"><span data-stu-id="2013f-145">Example</span></span>
<span data-ttu-id="2013f-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2013f-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2013f-147">要求</span><span class="sxs-lookup"><span data-stu-id="2013f-147">Request</span></span>
<span data-ttu-id="2013f-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2013f-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2013f-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2013f-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chartcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add
Content-type: application/json
Content-length: 94

{
  "type": "ColumnStacked",
  "sourceData": "A1:B1",
  "seriesBy": "Auto"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2013f-150">C#</span><span class="sxs-lookup"><span data-stu-id="2013f-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chartcollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2013f-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="2013f-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chartcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2013f-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="2013f-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chartcollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2013f-153">Java</span><span class="sxs-lookup"><span data-stu-id="2013f-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chartcollection-add-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2013f-154">応答</span><span class="sxs-lookup"><span data-stu-id="2013f-154">Response</span></span>
<span data-ttu-id="2013f-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2013f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChart"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "height": 99,
  "left": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
