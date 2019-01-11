---
title: 'ChartCollection: add'
description: 新しいグラフを作成します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 51ad28568abe7445a85f813698736130f04ac48e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892422"
---
# <a name="chartcollection-add"></a><span data-ttu-id="e96aa-103">ChartCollection: add</span><span class="sxs-lookup"><span data-stu-id="e96aa-103">ChartCollection: add</span></span>

> <span data-ttu-id="e96aa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e96aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e96aa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e96aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e96aa-106">新しいグラフを作成します。</span><span class="sxs-lookup"><span data-stu-id="e96aa-106">Creates a new chart.</span></span>
## <a name="permissions"></a><span data-ttu-id="e96aa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e96aa-107">Permissions</span></span>
<span data-ttu-id="e96aa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e96aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e96aa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e96aa-110">Permission type</span></span>      | <span data-ttu-id="e96aa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e96aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e96aa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e96aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e96aa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e96aa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e96aa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e96aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e96aa-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e96aa-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e96aa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e96aa-116">Application</span></span> | <span data-ttu-id="e96aa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e96aa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e96aa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e96aa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/add

```
## <a name="request-headers"></a><span data-ttu-id="e96aa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e96aa-119">Request headers</span></span>
| <span data-ttu-id="e96aa-120">名前</span><span class="sxs-lookup"><span data-stu-id="e96aa-120">Name</span></span>       | <span data-ttu-id="e96aa-121">説明</span><span class="sxs-lookup"><span data-stu-id="e96aa-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e96aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e96aa-122">Authorization</span></span>  | <span data-ttu-id="e96aa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e96aa-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e96aa-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e96aa-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e96aa-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e96aa-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e96aa-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e96aa-128">Request body</span></span>
<span data-ttu-id="e96aa-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e96aa-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e96aa-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e96aa-130">Parameter</span></span>    | <span data-ttu-id="e96aa-131">Type</span><span class="sxs-lookup"><span data-stu-id="e96aa-131">Type</span></span>   |<span data-ttu-id="e96aa-132">説明</span><span class="sxs-lookup"><span data-stu-id="e96aa-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e96aa-133">type</span><span class="sxs-lookup"><span data-stu-id="e96aa-133">type</span></span>|<span data-ttu-id="e96aa-134">文字列</span><span class="sxs-lookup"><span data-stu-id="e96aa-134">string</span></span>|<span data-ttu-id="e96aa-p105">グラフの種類を表します。可能な値は、`ColumnClustered`、`ColumnStacked`、`ColumnStacked100`、`BarClustered`、`BarStacked`、`BarStacked100`、`LineStacked`、`LineStacked100`、`LineMarkers`、`LineMarkersStacked`、`LineMarkersStacked100`、`PieOfPie`、`etc.` です。</span><span class="sxs-lookup"><span data-stu-id="e96aa-p105">Represents the type of a chart.  Possible values are: `ColumnClustered`, `ColumnStacked`, `ColumnStacked100`, `BarClustered`, `BarStacked`, `BarStacked100`, `LineStacked`, `LineStacked100`, `LineMarkers`, `LineMarkersStacked`, `LineMarkersStacked100`, `PieOfPie`, `etc.`.</span></span>|
|<span data-ttu-id="e96aa-137">sourceData</span><span class="sxs-lookup"><span data-stu-id="e96aa-137">sourceData</span></span>|<span data-ttu-id="e96aa-138">文字列</span><span class="sxs-lookup"><span data-stu-id="e96aa-138">string</span></span>|<span data-ttu-id="e96aa-139">データ ソースに対応する Range オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e96aa-139">The Range object corresponding to the source data.</span></span>|
|<span data-ttu-id="e96aa-140">seriesBy</span><span class="sxs-lookup"><span data-stu-id="e96aa-140">seriesBy</span></span>|<span data-ttu-id="e96aa-141">文字列</span><span class="sxs-lookup"><span data-stu-id="e96aa-141">string</span></span>|<span data-ttu-id="e96aa-p106">省略可能。列や行がグラフのデータ系列として使用される方法を指定します。可能な値は、`Auto`、`Columns`、`Rows` です。</span><span class="sxs-lookup"><span data-stu-id="e96aa-p106">Optional. Specifies the way columns or rows are used as data series on the chart.  Possible values are: `Auto`, `Columns`, `Rows`.</span></span>|

## <a name="response"></a><span data-ttu-id="e96aa-145">応答</span><span class="sxs-lookup"><span data-stu-id="e96aa-145">Response</span></span>

<span data-ttu-id="e96aa-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[グラフ](../resources/chart.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e96aa-146">If successful, this method returns `200 OK` response code and [Chart](../resources/chart.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e96aa-147">例</span><span class="sxs-lookup"><span data-stu-id="e96aa-147">Example</span></span>
<span data-ttu-id="e96aa-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e96aa-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e96aa-149">要求</span><span class="sxs-lookup"><span data-stu-id="e96aa-149">Request</span></span>
<span data-ttu-id="e96aa-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e96aa-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e96aa-151">応答</span><span class="sxs-lookup"><span data-stu-id="e96aa-151">Response</span></span>
<span data-ttu-id="e96aa-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e96aa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
