---
title: rangeborder を更新する
description: rangeborder オブジェクトのプロパティを更新します。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 99db19208242ae25c94c081b4e43f9f8caa47e67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877057"
---
# <a name="update-rangeborder"></a><span data-ttu-id="e7408-103">rangeborder を更新する</span><span class="sxs-lookup"><span data-stu-id="e7408-103">Update rangeborder</span></span>

> <span data-ttu-id="e7408-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e7408-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7408-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7408-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7408-106">rangeborder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e7408-106">Update the properties of rangeborder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7408-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7408-107">Permissions</span></span>
<span data-ttu-id="e7408-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7408-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7408-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7408-110">Permission type</span></span>      | <span data-ttu-id="e7408-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7408-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7408-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7408-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e7408-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7408-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7408-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7408-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7408-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7408-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e7408-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7408-116">Application</span></span> | <span data-ttu-id="e7408-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7408-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7408-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7408-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/borders(<sideIndex>)
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/borders(<sideIndex>)
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/borders(<sideIndex>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="e7408-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7408-119">Optional request headers</span></span>
| <span data-ttu-id="e7408-120">名前</span><span class="sxs-lookup"><span data-stu-id="e7408-120">Name</span></span>       | <span data-ttu-id="e7408-121">説明</span><span class="sxs-lookup"><span data-stu-id="e7408-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e7408-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7408-122">Authorization</span></span>  | <span data-ttu-id="e7408-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7408-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7408-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e7408-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e7408-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e7408-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7408-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7408-128">Request body</span></span>
<span data-ttu-id="e7408-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="e7408-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e7408-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7408-132">Property</span></span>     | <span data-ttu-id="e7408-133">種類</span><span class="sxs-lookup"><span data-stu-id="e7408-133">Type</span></span>   |<span data-ttu-id="e7408-134">説明</span><span class="sxs-lookup"><span data-stu-id="e7408-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7408-135">color</span><span class="sxs-lookup"><span data-stu-id="e7408-135">color</span></span>|<span data-ttu-id="e7408-136">文字列</span><span class="sxs-lookup"><span data-stu-id="e7408-136">string</span></span>|<span data-ttu-id="e7408-137">枠線の色を表す HTML カラー コード。形式は #RRGGBB (例: "FFA500")、または名前付きの HTML 色 (例: "オレンジ") です。</span><span class="sxs-lookup"><span data-stu-id="e7408-137">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="e7408-138">style</span><span class="sxs-lookup"><span data-stu-id="e7408-138">style</span></span>|<span data-ttu-id="e7408-139">文字列</span><span class="sxs-lookup"><span data-stu-id="e7408-139">string</span></span>|<span data-ttu-id="e7408-p106">罫線の線スタイルを指定する、線スタイル定数のいずれか 1 つ。可能な値は、`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot` です。</span><span class="sxs-lookup"><span data-stu-id="e7408-p106">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="e7408-142">weight</span><span class="sxs-lookup"><span data-stu-id="e7408-142">weight</span></span>|<span data-ttu-id="e7408-143">文字列</span><span class="sxs-lookup"><span data-stu-id="e7408-143">string</span></span>|<span data-ttu-id="e7408-p107">範囲を取り囲む罫線の太さを指定します。可能な値は、`Hairline`、`Thin`、`Medium`、`Thick` です。</span><span class="sxs-lookup"><span data-stu-id="e7408-p107">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="response"></a><span data-ttu-id="e7408-146">応答</span><span class="sxs-lookup"><span data-stu-id="e7408-146">Response</span></span>

<span data-ttu-id="e7408-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [RangeBorder](../resources/rangeborder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7408-147">If successful, this method returns a `200 OK` response code and updated [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7408-148">例</span><span class="sxs-lookup"><span data-stu-id="e7408-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7408-149">要求</span><span class="sxs-lookup"><span data-stu-id="e7408-149">Request</span></span>
<span data-ttu-id="e7408-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7408-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangeborder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders(<sideIndex>)
Content-type: application/json
Content-length: 136

{
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
##### <a name="response"></a><span data-ttu-id="e7408-151">応答</span><span class="sxs-lookup"><span data-stu-id="e7408-151">Response</span></span>
<span data-ttu-id="e7408-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7408-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
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
