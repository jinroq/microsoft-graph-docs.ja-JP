---
title: Update chartlegend
description: chartlegend オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c12874efca72938bfd819a84caabd756c102ae05
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327724"
---
# <a name="update-chartlegend"></a><span data-ttu-id="7388b-103">Update chartlegend</span><span class="sxs-lookup"><span data-stu-id="7388b-103">Update chartlegend</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7388b-104">chartlegend オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7388b-104">Update the properties of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7388b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7388b-105">Permissions</span></span>
<span data-ttu-id="7388b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7388b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7388b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7388b-108">Permission type</span></span>      | <span data-ttu-id="7388b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7388b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7388b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7388b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7388b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7388b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7388b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7388b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7388b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7388b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7388b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7388b-114">Application</span></span> | <span data-ttu-id="7388b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7388b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7388b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7388b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts/{name}/legend
```
## <a name="optional-request-headers"></a><span data-ttu-id="7388b-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7388b-117">Optional request headers</span></span>
| <span data-ttu-id="7388b-118">名前</span><span class="sxs-lookup"><span data-stu-id="7388b-118">Name</span></span>       | <span data-ttu-id="7388b-119">説明</span><span class="sxs-lookup"><span data-stu-id="7388b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7388b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7388b-120">Authorization</span></span>  | <span data-ttu-id="7388b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7388b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7388b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7388b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="7388b-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="7388b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7388b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7388b-126">Request body</span></span>
<span data-ttu-id="7388b-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7388b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7388b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7388b-130">Property</span></span>     | <span data-ttu-id="7388b-131">型</span><span class="sxs-lookup"><span data-stu-id="7388b-131">Type</span></span>   |<span data-ttu-id="7388b-132">説明</span><span class="sxs-lookup"><span data-stu-id="7388b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7388b-133">overlay</span><span class="sxs-lookup"><span data-stu-id="7388b-133">overlay</span></span>|<span data-ttu-id="7388b-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="7388b-134">boolean</span></span>|<span data-ttu-id="7388b-135">グラフの凡例をグラフの本体に重ねるかどうかを指定するブール型の値です。</span><span class="sxs-lookup"><span data-stu-id="7388b-135">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="7388b-136">position</span><span class="sxs-lookup"><span data-stu-id="7388b-136">position</span></span>|<span data-ttu-id="7388b-137">string</span><span class="sxs-lookup"><span data-stu-id="7388b-137">string</span></span>|<span data-ttu-id="7388b-p105">グラフの凡例の位置を表します。可能な値は、`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom` です。</span><span class="sxs-lookup"><span data-stu-id="7388b-p105">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="7388b-140">visible</span><span class="sxs-lookup"><span data-stu-id="7388b-140">visible</span></span>|<span data-ttu-id="7388b-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="7388b-141">boolean</span></span>|<span data-ttu-id="7388b-142">ChartLegend オブジェクトを表示または非表示にするかを表すブール型の値。</span><span class="sxs-lookup"><span data-stu-id="7388b-142">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="response"></a><span data-ttu-id="7388b-143">応答</span><span class="sxs-lookup"><span data-stu-id="7388b-143">Response</span></span>

<span data-ttu-id="7388b-144">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[workbookChartLegend](../resources/workbookchartlegend.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7388b-144">If successful, this method returns a `200 OK` response code and updated [workbookChartLegend](../resources/workbookchartlegend.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7388b-145">例</span><span class="sxs-lookup"><span data-stu-id="7388b-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7388b-146">要求</span><span class="sxs-lookup"><span data-stu-id="7388b-146">Request</span></span>
<span data-ttu-id="7388b-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7388b-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartlegend"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```
##### <a name="response"></a><span data-ttu-id="7388b-148">応答</span><span class="sxs-lookup"><span data-stu-id="7388b-148">Response</span></span>
<span data-ttu-id="7388b-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7388b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookChartLegend"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "visible": true,
  "position": "position-value",
  "overlay": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update chartlegend",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
