---
title: 'ChartCollection: add'
description: 新しいグラフを作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f552e4d8f0c8dc9f1257baf02ebe7a449c98a348
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572116"
---
# <a name="chartcollection-add"></a><span data-ttu-id="144e2-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="144e2-103">ChartCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="144e2-104">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="144e2-104">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="144e2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="144e2-105">Permissions</span></span>
<span data-ttu-id="144e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="144e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="144e2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="144e2-108">Permission type</span></span>      | <span data-ttu-id="144e2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="144e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="144e2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="144e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="144e2-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="144e2-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="144e2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="144e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="144e2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="144e2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="144e2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="144e2-114">Application</span></span> | <span data-ttu-id="144e2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="144e2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="144e2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="144e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="144e2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="144e2-117">Request headers</span></span>
| <span data-ttu-id="144e2-118">名前</span><span class="sxs-lookup"><span data-stu-id="144e2-118">Name</span></span>       | <span data-ttu-id="144e2-119">説明</span><span class="sxs-lookup"><span data-stu-id="144e2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="144e2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="144e2-120">Authorization</span></span>  | <span data-ttu-id="144e2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="144e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="144e2-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="144e2-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="144e2-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="144e2-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="144e2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="144e2-126">Request body</span></span>
<span data-ttu-id="144e2-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="144e2-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="144e2-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="144e2-128">Parameter</span></span>    | <span data-ttu-id="144e2-129">型</span><span class="sxs-lookup"><span data-stu-id="144e2-129">Type</span></span>   |<span data-ttu-id="144e2-130">説明</span><span class="sxs-lookup"><span data-stu-id="144e2-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="144e2-131">type</span><span class="sxs-lookup"><span data-stu-id="144e2-131">type</span></span>|<span data-ttu-id="144e2-132">文字列</span><span class="sxs-lookup"><span data-stu-id="144e2-132">string</span></span>|<span data-ttu-id="144e2-133">グラフの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="144e2-133">Represents the type of a chart.</span></span>  <span data-ttu-id="144e2-134">可能な値: `ColumnClustered`、 `ColumnStacked`、 `ColumnStacked100`、 `BarClustered`、 `BarStacked`、 `BarStacked100`、 `LineStacked`、 `LineStacked100`、 `LineMarkers`、 `LineMarkersStacked`、 `LineMarkersStacked100`、 `PieOfPie`、 `etc.`。</span><span class="sxs-lookup"><span data-stu-id="144e2-134">The possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="144e2-135">sourceData</span><span class="sxs-lookup"><span data-stu-id="144e2-135">sourceData</span></span>|<span data-ttu-id="144e2-136">Json</span><span class="sxs-lookup"><span data-stu-id="144e2-136">Json</span></span>|<span data-ttu-id="144e2-137">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="144e2-137">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="144e2-138">seriesBy</span><span class="sxs-lookup"><span data-stu-id="144e2-138">seriesBy</span></span>|<span data-ttu-id="144e2-139">文字列</span><span class="sxs-lookup"><span data-stu-id="144e2-139">string</span></span>|<span data-ttu-id="144e2-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="144e2-140">Optional.</span></span> <span data-ttu-id="144e2-141">方法の列または行がグラフのデータ系列として使用されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="144e2-141">Specifies the way columns or rows are used as data series on the chart.</span></span>  <span data-ttu-id="144e2-142">可能な値: `Auto`、 `Columns`、 `Rows`。</span><span class="sxs-lookup"><span data-stu-id="144e2-142">The possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="144e2-143">応答</span><span class="sxs-lookup"><span data-stu-id="144e2-143">Response</span></span>

<span data-ttu-id="144e2-144">かどうかは成功すると、このメソッドを返します`200 OK`応答コードおよび応答の本文に[WorkbookChart](../resources/chart.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="144e2-144">If successful, this method returns `200 OK` response code and [WorkbookChart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="144e2-145">例</span><span class="sxs-lookup"><span data-stu-id="144e2-145">Example</span></span>
<span data-ttu-id="144e2-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="144e2-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="144e2-147">要求</span><span class="sxs-lookup"><span data-stu-id="144e2-147">Request</span></span>
<span data-ttu-id="144e2-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="144e2-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="144e2-149">応答</span><span class="sxs-lookup"><span data-stu-id="144e2-149">Response</span></span>
<span data-ttu-id="144e2-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="144e2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/chartcollection-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
