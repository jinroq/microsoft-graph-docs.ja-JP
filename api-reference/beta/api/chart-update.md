---
title: Update chart
description: グラフ オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e668b8d9d6184398729ed5079be27f75ae5d3e03
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572886"
---
# <a name="update-chart"></a><span data-ttu-id="17880-103">Update chart</span><span class="sxs-lookup"><span data-stu-id="17880-103">Update chart</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17880-104">グラフ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="17880-104">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="17880-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="17880-105">Permissions</span></span>
<span data-ttu-id="17880-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17880-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17880-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="17880-108">Permission type</span></span>      | <span data-ttu-id="17880-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="17880-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17880-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="17880-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17880-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17880-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="17880-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="17880-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17880-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="17880-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="17880-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="17880-114">Application</span></span> | <span data-ttu-id="17880-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17880-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17880-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17880-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="17880-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17880-117">Optional request headers</span></span>
| <span data-ttu-id="17880-118">名前</span><span class="sxs-lookup"><span data-stu-id="17880-118">Name</span></span>       | <span data-ttu-id="17880-119">説明</span><span class="sxs-lookup"><span data-stu-id="17880-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="17880-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="17880-120">Authorization</span></span>  | <span data-ttu-id="17880-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="17880-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17880-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="17880-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="17880-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="17880-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17880-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="17880-126">Request body</span></span>
<span data-ttu-id="17880-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="17880-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="17880-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17880-130">Property</span></span>     | <span data-ttu-id="17880-131">型</span><span class="sxs-lookup"><span data-stu-id="17880-131">Type</span></span>   |<span data-ttu-id="17880-132">説明</span><span class="sxs-lookup"><span data-stu-id="17880-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17880-133">height</span><span class="sxs-lookup"><span data-stu-id="17880-133">height</span></span>|<span data-ttu-id="17880-134">double</span><span class="sxs-lookup"><span data-stu-id="17880-134">double</span></span>|<span data-ttu-id="17880-135">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="17880-135">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="17880-136">left</span><span class="sxs-lookup"><span data-stu-id="17880-136">left</span></span>|<span data-ttu-id="17880-137">double</span><span class="sxs-lookup"><span data-stu-id="17880-137">double</span></span>|<span data-ttu-id="17880-138">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="17880-138">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="17880-139">name</span><span class="sxs-lookup"><span data-stu-id="17880-139">name</span></span>|<span data-ttu-id="17880-140">文字列</span><span class="sxs-lookup"><span data-stu-id="17880-140">string</span></span>|<span data-ttu-id="17880-141"> グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="17880-141">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="17880-142">top</span><span class="sxs-lookup"><span data-stu-id="17880-142">top</span></span>|<span data-ttu-id="17880-143">double</span><span class="sxs-lookup"><span data-stu-id="17880-143">double</span></span>|<span data-ttu-id="17880-144">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="17880-144">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="17880-145">width</span><span class="sxs-lookup"><span data-stu-id="17880-145">width</span></span>|<span data-ttu-id="17880-146">double</span><span class="sxs-lookup"><span data-stu-id="17880-146">double</span></span>|<span data-ttu-id="17880-147">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="17880-147">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="17880-148">応答</span><span class="sxs-lookup"><span data-stu-id="17880-148">Response</span></span>

<span data-ttu-id="17880-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookChart](../resources/chart.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="17880-149">If successful, this method returns a `200 OK` response code and updated [WorkbookChart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17880-150">例</span><span class="sxs-lookup"><span data-stu-id="17880-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17880-151">要求</span><span class="sxs-lookup"><span data-stu-id="17880-151">Request</span></span>
<span data-ttu-id="17880-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="17880-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
##### <a name="response"></a><span data-ttu-id="17880-153">応答</span><span class="sxs-lookup"><span data-stu-id="17880-153">Response</span></span>
<span data-ttu-id="17880-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="17880-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chart-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
