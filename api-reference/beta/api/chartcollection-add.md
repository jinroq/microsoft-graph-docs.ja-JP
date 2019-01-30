---
title: 'ChartCollection: add'
description: 新しいグラフを作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cdb3ff01b0741f0f1a4a0bff22e3a8e3dc32335c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642157"
---
# <a name="chartcollection-add"></a><span data-ttu-id="f0f38-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="f0f38-103">ChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0f38-104">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="f0f38-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0f38-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f0f38-105">Permissions</span></span>
<span data-ttu-id="f0f38-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0f38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0f38-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0f38-108">Permission type</span></span>      | <span data-ttu-id="f0f38-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0f38-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0f38-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0f38-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f0f38-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0f38-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0f38-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0f38-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0f38-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0f38-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f0f38-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0f38-114">Application</span></span> | <span data-ttu-id="f0f38-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0f38-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0f38-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0f38-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="f0f38-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0f38-117">Request headers</span></span>
| <span data-ttu-id="f0f38-118">名前</span><span class="sxs-lookup"><span data-stu-id="f0f38-118">Name</span></span>       | <span data-ttu-id="f0f38-119">説明</span><span class="sxs-lookup"><span data-stu-id="f0f38-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f0f38-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0f38-120">Authorization</span></span>  | <span data-ttu-id="f0f38-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f0f38-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0f38-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f0f38-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="f0f38-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f0f38-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f38-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0f38-126">Request body</span></span>
<span data-ttu-id="f0f38-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f0f38-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f0f38-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f0f38-128">Parameter</span></span>    | <span data-ttu-id="f0f38-129">型</span><span class="sxs-lookup"><span data-stu-id="f0f38-129">Type</span></span>   |<span data-ttu-id="f0f38-130">説明</span><span class="sxs-lookup"><span data-stu-id="f0f38-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0f38-131">type</span><span class="sxs-lookup"><span data-stu-id="f0f38-131">type</span></span>|<span data-ttu-id="f0f38-132">string</span><span class="sxs-lookup"><span data-stu-id="f0f38-132">string</span></span>|<span data-ttu-id="f0f38-p104">グラフの種類を表します。可能な値は、`ColumnClustered`、`ColumnStacked`、`ColumnStacked100`、`BarClustered`、`BarStacked`、`BarStacked100`、`LineStacked`、`LineStacked100`、`LineMarkers`、`LineMarkersStacked`、`LineMarkersStacked100`、`PieOfPie`、`etc.` です。</span><span class="sxs-lookup"><span data-stu-id="f0f38-p104">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="f0f38-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="f0f38-135">sourceData</span></span>|<span data-ttu-id="f0f38-136">string</span><span class="sxs-lookup"><span data-stu-id="f0f38-136">string</span></span>|<span data-ttu-id="f0f38-137">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f0f38-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="f0f38-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="f0f38-138">seriesBy</span></span>|<span data-ttu-id="f0f38-139">文字列</span><span class="sxs-lookup"><span data-stu-id="f0f38-139">string</span></span>|<span data-ttu-id="f0f38-p105">省略可能。列や行がグラフのデータ系列として使用される方法を指定します。可能な値は、`Auto`、`Columns`、`Rows` です。</span><span class="sxs-lookup"><span data-stu-id="f0f38-p105">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="f0f38-143">応答</span><span class="sxs-lookup"><span data-stu-id="f0f38-143">Response</span></span>

<span data-ttu-id="f0f38-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[グラフ](../resources/chart.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0f38-144">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f38-145">例</span><span class="sxs-lookup"><span data-stu-id="f0f38-145">Example</span></span>
<span data-ttu-id="f0f38-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="f0f38-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f0f38-147">要求</span><span class="sxs-lookup"><span data-stu-id="f0f38-147">Request</span></span>
<span data-ttu-id="f0f38-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0f38-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f0f38-149">応答</span><span class="sxs-lookup"><span data-stu-id="f0f38-149">Response</span></span>
<span data-ttu-id="f0f38-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0f38-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chartcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
