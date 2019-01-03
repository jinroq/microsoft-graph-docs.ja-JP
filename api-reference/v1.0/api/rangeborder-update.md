---
title: rangeborder を更新する
description: rangeborder オブジェクトのプロパティを更新します。
author: lumine2008
ms.openlocfilehash: ed9b2e5fa6b3d4a1dd3c227160eb71435e9a3817
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311943"
---
# <a name="update-rangeborder"></a><span data-ttu-id="47e30-103">rangeborder を更新する</span><span class="sxs-lookup"><span data-stu-id="47e30-103">Update rangeborder</span></span>

<span data-ttu-id="47e30-104">rangeborder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="47e30-104">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="47e30-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="47e30-105">Permissions</span></span>
<span data-ttu-id="47e30-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47e30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47e30-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47e30-108">Permission type</span></span>      | <span data-ttu-id="47e30-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="47e30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47e30-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47e30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47e30-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47e30-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="47e30-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47e30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47e30-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47e30-113">Not supported.</span></span>    |
|<span data-ttu-id="47e30-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47e30-114">Application</span></span> | <span data-ttu-id="47e30-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47e30-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47e30-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47e30-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names/{name}/range/format/borders/{sideIndex}
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/{sideIndex}
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/{sideIndex}
```
## <a name="optional-request-headers"></a><span data-ttu-id="47e30-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47e30-117">Optional request headers</span></span>
| <span data-ttu-id="47e30-118">名前</span><span class="sxs-lookup"><span data-stu-id="47e30-118">Name</span></span>       | <span data-ttu-id="47e30-119">説明</span><span class="sxs-lookup"><span data-stu-id="47e30-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="47e30-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="47e30-120">Authorization</span></span>  | <span data-ttu-id="47e30-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="47e30-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47e30-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="47e30-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="47e30-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="47e30-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47e30-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="47e30-126">Request body</span></span>
<span data-ttu-id="47e30-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="47e30-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="47e30-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47e30-130">Property</span></span>     | <span data-ttu-id="47e30-131">種類</span><span class="sxs-lookup"><span data-stu-id="47e30-131">Type</span></span>   |<span data-ttu-id="47e30-132">説明</span><span class="sxs-lookup"><span data-stu-id="47e30-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47e30-133">color</span><span class="sxs-lookup"><span data-stu-id="47e30-133">color</span></span>|<span data-ttu-id="47e30-134">文字列</span><span class="sxs-lookup"><span data-stu-id="47e30-134">string</span></span>|<span data-ttu-id="47e30-135">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="47e30-135">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="47e30-136">style</span><span class="sxs-lookup"><span data-stu-id="47e30-136">style</span></span>|<span data-ttu-id="47e30-137">文字列</span><span class="sxs-lookup"><span data-stu-id="47e30-137">string</span></span>|<span data-ttu-id="47e30-138">境界線の線のスタイルを指定する線のスタイルの定数の 1 つです。</span><span class="sxs-lookup"><span data-stu-id="47e30-138">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="47e30-139">可能な値: `None`、 `Continuous`、 `Dash`、 `DashDot`、 `DashDotDot`、 `Dot`、 `Double`、 `SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="47e30-139">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="47e30-140">weight</span><span class="sxs-lookup"><span data-stu-id="47e30-140">weight</span></span>|<span data-ttu-id="47e30-141">文字列</span><span class="sxs-lookup"><span data-stu-id="47e30-141">string</span></span>|<span data-ttu-id="47e30-142">範囲周辺の罫線の太さを指定します。</span><span class="sxs-lookup"><span data-stu-id="47e30-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="47e30-143">可能な値: `Hairline`、 `Thin`、 `Medium`、 `Thick`。</span><span class="sxs-lookup"><span data-stu-id="47e30-143">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="47e30-144">応答</span><span class="sxs-lookup"><span data-stu-id="47e30-144">Response</span></span>

<span data-ttu-id="47e30-145">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[WorkbookRangeBorder](../resources/rangeborder.md)オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="47e30-145">If successful, this method returns a `200 OK` response code and updated [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47e30-146">例</span><span class="sxs-lookup"><span data-stu-id="47e30-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47e30-147">要求</span><span class="sxs-lookup"><span data-stu-id="47e30-147">Request</span></span>
<span data-ttu-id="47e30-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="47e30-148">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="47e30-149">応答</span><span class="sxs-lookup"><span data-stu-id="47e30-149">Response</span></span>
<span data-ttu-id="47e30-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="47e30-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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