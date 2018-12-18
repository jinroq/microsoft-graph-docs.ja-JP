---
title: Update chart
description: グラフ オブジェクトのプロパティを更新します。
author: lumine2008
ms.openlocfilehash: 086d4a2ea0ce823ace141df0d5576af732bf8c0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328183"
---
# <a name="update-chart"></a><span data-ttu-id="4d389-103">Update chart</span><span class="sxs-lookup"><span data-stu-id="4d389-103">Update chart</span></span>

> <span data-ttu-id="4d389-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4d389-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d389-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d389-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d389-106">グラフ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4d389-106">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d389-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d389-107">Permissions</span></span>
<span data-ttu-id="4d389-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d389-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d389-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d389-110">Permission type</span></span>      | <span data-ttu-id="4d389-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d389-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d389-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d389-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4d389-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d389-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d389-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d389-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d389-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4d389-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4d389-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d389-116">Application</span></span> | <span data-ttu-id="4d389-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d389-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d389-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d389-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="4d389-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d389-119">Optional request headers</span></span>
| <span data-ttu-id="4d389-120">名前</span><span class="sxs-lookup"><span data-stu-id="4d389-120">Name</span></span>       | <span data-ttu-id="4d389-121">説明</span><span class="sxs-lookup"><span data-stu-id="4d389-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4d389-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d389-122">Authorization</span></span>  | <span data-ttu-id="4d389-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4d389-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d389-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4d389-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4d389-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="4d389-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d389-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d389-128">Request body</span></span>
<span data-ttu-id="4d389-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4d389-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4d389-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d389-132">Property</span></span>     | <span data-ttu-id="4d389-133">種類</span><span class="sxs-lookup"><span data-stu-id="4d389-133">Type</span></span>   |<span data-ttu-id="4d389-134">説明</span><span class="sxs-lookup"><span data-stu-id="4d389-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d389-135">height</span><span class="sxs-lookup"><span data-stu-id="4d389-135">height</span></span>|<span data-ttu-id="4d389-136">double</span><span class="sxs-lookup"><span data-stu-id="4d389-136">double</span></span>|<span data-ttu-id="4d389-137">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="4d389-137">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="4d389-138">left</span><span class="sxs-lookup"><span data-stu-id="4d389-138">left</span></span>|<span data-ttu-id="4d389-139">double</span><span class="sxs-lookup"><span data-stu-id="4d389-139">double</span></span>|<span data-ttu-id="4d389-140">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="4d389-140">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="4d389-141">name</span><span class="sxs-lookup"><span data-stu-id="4d389-141">name</span></span>|<span data-ttu-id="4d389-142">文字列</span><span class="sxs-lookup"><span data-stu-id="4d389-142">string</span></span>|<span data-ttu-id="4d389-143"> グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="4d389-143">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="4d389-144">top</span><span class="sxs-lookup"><span data-stu-id="4d389-144">top</span></span>|<span data-ttu-id="4d389-145">double</span><span class="sxs-lookup"><span data-stu-id="4d389-145">double</span></span>|<span data-ttu-id="4d389-146">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="4d389-146">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="4d389-147">width</span><span class="sxs-lookup"><span data-stu-id="4d389-147">width</span></span>|<span data-ttu-id="4d389-148">double</span><span class="sxs-lookup"><span data-stu-id="4d389-148">double</span></span>|<span data-ttu-id="4d389-149">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="4d389-149">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="4d389-150">応答</span><span class="sxs-lookup"><span data-stu-id="4d389-150">Response</span></span>

<span data-ttu-id="4d389-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[グラフ](../resources/chart.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4d389-151">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d389-152">例</span><span class="sxs-lookup"><span data-stu-id="4d389-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d389-153">要求</span><span class="sxs-lookup"><span data-stu-id="4d389-153">Request</span></span>
<span data-ttu-id="4d389-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d389-154">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4d389-155">応答</span><span class="sxs-lookup"><span data-stu-id="4d389-155">Response</span></span>
<span data-ttu-id="4d389-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4d389-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->