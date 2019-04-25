---
title: rangeborder を更新する
description: rangeborder オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2d8a3bbd24f83dd635c6254b852a2ecd00660fe9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582417"
---
# <a name="update-rangeborder"></a><span data-ttu-id="4bd8f-103">rangeborder を更新する</span><span class="sxs-lookup"><span data-stu-id="4bd8f-103">Update rangeborder</span></span>

<span data-ttu-id="4bd8f-104">rangeborder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4bd8f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4bd8f-105">Permissions</span></span>
<span data-ttu-id="4bd8f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bd8f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4bd8f-108">Permission type</span></span>      | <span data-ttu-id="4bd8f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4bd8f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4bd8f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4bd8f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4bd8f-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4bd8f-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4bd8f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4bd8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4bd8f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-113">Not supported.</span></span>    |
|<span data-ttu-id="4bd8f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4bd8f-114">Application</span></span> | <span data-ttu-id="4bd8f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4bd8f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4bd8f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4bd8f-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bd8f-117">Optional request headers</span></span>
| <span data-ttu-id="4bd8f-118">名前</span><span class="sxs-lookup"><span data-stu-id="4bd8f-118">Name</span></span>       | <span data-ttu-id="4bd8f-119">説明</span><span class="sxs-lookup"><span data-stu-id="4bd8f-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4bd8f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bd8f-120">Authorization</span></span>  | <span data-ttu-id="4bd8f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4bd8f-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4bd8f-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="4bd8f-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bd8f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4bd8f-126">Request body</span></span>
<span data-ttu-id="4bd8f-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4bd8f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bd8f-130">Property</span></span>     | <span data-ttu-id="4bd8f-131">型</span><span class="sxs-lookup"><span data-stu-id="4bd8f-131">Type</span></span>   |<span data-ttu-id="4bd8f-132">説明</span><span class="sxs-lookup"><span data-stu-id="4bd8f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bd8f-133">color</span><span class="sxs-lookup"><span data-stu-id="4bd8f-133">color</span></span>|<span data-ttu-id="4bd8f-134">文字列</span><span class="sxs-lookup"><span data-stu-id="4bd8f-134">string</span></span>|<span data-ttu-id="4bd8f-135">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="4bd8f-136">style</span><span class="sxs-lookup"><span data-stu-id="4bd8f-136">style</span></span>|<span data-ttu-id="4bd8f-137">string</span><span class="sxs-lookup"><span data-stu-id="4bd8f-137">string</span></span>|<span data-ttu-id="4bd8f-138">罫線の線スタイルを指定する、線スタイル定数のいずれか 1 つ。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-138">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="4bd8f-139">使用可能な値は`None`、 `Continuous`、 `Dash` `DashDot` `DashDotDot` `Dot` `Double`、、、、、 `SlantDashDot`、です。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-139">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="4bd8f-140">weight</span><span class="sxs-lookup"><span data-stu-id="4bd8f-140">weight</span></span>|<span data-ttu-id="4bd8f-141">string</span><span class="sxs-lookup"><span data-stu-id="4bd8f-141">string</span></span>|<span data-ttu-id="4bd8f-142">範囲を取り囲む罫線の太さを指定します。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="4bd8f-143">使用可能な値は`Hairline`、 `Thin`、 `Medium`、 `Thick`、です。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-143">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="4bd8f-144">応答</span><span class="sxs-lookup"><span data-stu-id="4bd8f-144">Response</span></span>

<span data-ttu-id="4bd8f-145">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、更新された[WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-145">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4bd8f-146">例</span><span class="sxs-lookup"><span data-stu-id="4bd8f-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bd8f-147">要求</span><span class="sxs-lookup"><span data-stu-id="4bd8f-147">Request</span></span>
<span data-ttu-id="4bd8f-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="4bd8f-149">応答</span><span class="sxs-lookup"><span data-stu-id="4bd8f-149">Response</span></span>
<span data-ttu-id="4bd8f-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4bd8f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangeborder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
