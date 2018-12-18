---
title: 'ChartCollection: add'
description: 新しいグラフを作成します。
author: lumine2008
ms.openlocfilehash: 704afc9890e3921c69cdd7b746c0e362c4627511
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325551"
---
# <a name="chartcollection-add"></a><span data-ttu-id="0e038-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="0e038-103">ChartCollection: add</span></span>

> <span data-ttu-id="0e038-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e038-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e038-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e038-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e038-106">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="0e038-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="0e038-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0e038-107">Permissions</span></span>
<span data-ttu-id="0e038-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e038-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e038-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e038-110">Permission type</span></span>      | <span data-ttu-id="0e038-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e038-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e038-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e038-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e038-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e038-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e038-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0e038-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e038-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e038-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0e038-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e038-116">Application</span></span> | <span data-ttu-id="0e038-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e038-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e038-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e038-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="0e038-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e038-119">Request headers</span></span>
| <span data-ttu-id="0e038-120">名前</span><span class="sxs-lookup"><span data-stu-id="0e038-120">Name</span></span>       | <span data-ttu-id="0e038-121">説明</span><span class="sxs-lookup"><span data-stu-id="0e038-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0e038-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e038-122">Authorization</span></span>  | <span data-ttu-id="0e038-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0e038-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e038-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0e038-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="0e038-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0e038-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e038-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e038-128">Request body</span></span>
<span data-ttu-id="0e038-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0e038-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0e038-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0e038-130">Parameter</span></span>    | <span data-ttu-id="0e038-131">種類</span><span class="sxs-lookup"><span data-stu-id="0e038-131">Type</span></span>   |<span data-ttu-id="0e038-132">説明</span><span class="sxs-lookup"><span data-stu-id="0e038-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e038-133">type</span><span class="sxs-lookup"><span data-stu-id="0e038-133">type</span></span>|<span data-ttu-id="0e038-134">string</span><span class="sxs-lookup"><span data-stu-id="0e038-134">string</span></span>|<span data-ttu-id="0e038-p105">グラフの種類を表します。可能な値は、`ColumnClustered`、`ColumnStacked`、`ColumnStacked100`、`BarClustered`、`BarStacked`、`BarStacked100`、`LineStacked`、`LineStacked100`、`LineMarkers`、`LineMarkersStacked`、`LineMarkersStacked100`、`PieOfPie`、`etc.` です。</span><span class="sxs-lookup"><span data-stu-id="0e038-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="0e038-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="0e038-137">sourceData</span></span>|<span data-ttu-id="0e038-138">string</span><span class="sxs-lookup"><span data-stu-id="0e038-138">string</span></span>|<span data-ttu-id="0e038-139">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0e038-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="0e038-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="0e038-140">seriesBy</span></span>|<span data-ttu-id="0e038-141">文字列</span><span class="sxs-lookup"><span data-stu-id="0e038-141">string</span></span>|<span data-ttu-id="0e038-p106">省略可能。列や行がグラフのデータ系列として使用される方法を指定します。可能な値は、`Auto`、`Columns`、`Rows` です。</span><span class="sxs-lookup"><span data-stu-id="0e038-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="0e038-145">応答</span><span class="sxs-lookup"><span data-stu-id="0e038-145">Response</span></span>

<span data-ttu-id="0e038-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[グラフ](../resources/chart.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0e038-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e038-147">例</span><span class="sxs-lookup"><span data-stu-id="0e038-147">Example</span></span>
<span data-ttu-id="0e038-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0e038-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0e038-149">要求</span><span class="sxs-lookup"><span data-stu-id="0e038-149">Request</span></span>
<span data-ttu-id="0e038-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0e038-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0e038-151">応答</span><span class="sxs-lookup"><span data-stu-id="0e038-151">Response</span></span>
<span data-ttu-id="0e038-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0e038-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chart"
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
