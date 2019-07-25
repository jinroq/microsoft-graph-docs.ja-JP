---
title: Update chart
description: グラフ オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 37b57a7d2a22a672dfc159d8a4b4fe23d53d5134
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882090"
---
# <a name="update-chart"></a><span data-ttu-id="c430b-103">Update chart</span><span class="sxs-lookup"><span data-stu-id="c430b-103">Update chart</span></span>

<span data-ttu-id="c430b-104">グラフ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c430b-104">Update the properties of chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c430b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c430b-105">Permissions</span></span>
<span data-ttu-id="c430b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c430b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c430b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c430b-108">Permission type</span></span>      | <span data-ttu-id="c430b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c430b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c430b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c430b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c430b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c430b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c430b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c430b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c430b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c430b-113">Not supported.</span></span>    |
|<span data-ttu-id="c430b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c430b-114">Application</span></span> | <span data-ttu-id="c430b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c430b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c430b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c430b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c430b-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c430b-117">Optional request headers</span></span>
| <span data-ttu-id="c430b-118">名前</span><span class="sxs-lookup"><span data-stu-id="c430b-118">Name</span></span>       | <span data-ttu-id="c430b-119">説明</span><span class="sxs-lookup"><span data-stu-id="c430b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c430b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c430b-120">Authorization</span></span>  | <span data-ttu-id="c430b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c430b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c430b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c430b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="c430b-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="c430b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c430b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c430b-126">Request body</span></span>
<span data-ttu-id="c430b-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="c430b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c430b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c430b-130">Property</span></span>     | <span data-ttu-id="c430b-131">型</span><span class="sxs-lookup"><span data-stu-id="c430b-131">Type</span></span>   |<span data-ttu-id="c430b-132">説明</span><span class="sxs-lookup"><span data-stu-id="c430b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c430b-133">height</span><span class="sxs-lookup"><span data-stu-id="c430b-133">height</span></span>|<span data-ttu-id="c430b-134">double</span><span class="sxs-lookup"><span data-stu-id="c430b-134">double</span></span>|<span data-ttu-id="c430b-135">グラフ オブジェクトの高さをポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="c430b-135">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="c430b-136">left</span><span class="sxs-lookup"><span data-stu-id="c430b-136">left</span></span>|<span data-ttu-id="c430b-137">double</span><span class="sxs-lookup"><span data-stu-id="c430b-137">double</span></span>|<span data-ttu-id="c430b-138">グラフの左側からワークシートの原点までの距離 (ポイント単位)。</span><span class="sxs-lookup"><span data-stu-id="c430b-138">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="c430b-139">name</span><span class="sxs-lookup"><span data-stu-id="c430b-139">name</span></span>|<span data-ttu-id="c430b-140">string</span><span class="sxs-lookup"><span data-stu-id="c430b-140">string</span></span>|<span data-ttu-id="c430b-141">グラフ オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="c430b-141">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="c430b-142">top</span><span class="sxs-lookup"><span data-stu-id="c430b-142">top</span></span>|<span data-ttu-id="c430b-143">double</span><span class="sxs-lookup"><span data-stu-id="c430b-143">double</span></span>|<span data-ttu-id="c430b-144">オブジェクトの上端から (ワークシートの) 1 行目の上部または (グラフの) グラフ領域の上部までの距離をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="c430b-144">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="c430b-145">width</span><span class="sxs-lookup"><span data-stu-id="c430b-145">width</span></span>|<span data-ttu-id="c430b-146">double</span><span class="sxs-lookup"><span data-stu-id="c430b-146">double</span></span>|<span data-ttu-id="c430b-147">グラフ オブジェクトの幅をポイント単位で表します。</span><span class="sxs-lookup"><span data-stu-id="c430b-147">Represents the width, in points, of the chart object.</span></span>|

## <a name="response"></a><span data-ttu-id="c430b-148">応答</span><span class="sxs-lookup"><span data-stu-id="c430b-148">Response</span></span>

<span data-ttu-id="c430b-149">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookChart](../resources/chart.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c430b-149">If successful, this method returns a `200 OK` response code and updated [WorkbookChart](../resources/chart.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c430b-150">例</span><span class="sxs-lookup"><span data-stu-id="c430b-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c430b-151">要求</span><span class="sxs-lookup"><span data-stu-id="c430b-151">Request</span></span>
<span data-ttu-id="c430b-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c430b-152">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c430b-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c430b-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chart"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}
Content-type: application/json
Content-length: 52

{
  "height": 99,
  "left": 99
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c430b-154">C#</span><span class="sxs-lookup"><span data-stu-id="c430b-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chart-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c430b-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="c430b-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chart-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c430b-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="c430b-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chart-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c430b-157">Java</span><span class="sxs-lookup"><span data-stu-id="c430b-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chart-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c430b-158">応答</span><span class="sxs-lookup"><span data-stu-id="c430b-158">Response</span></span>
<span data-ttu-id="c430b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c430b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update chart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
