---
title: 範囲:OffsetRange
description: 指定した範囲からのオフセットで範囲を表すオブジェクトを取得します。返される範囲のディメンションは、この範囲と一致します。結果の範囲が、ワークシートのグリッドの境界線の外にはみ出る場合は、例外がスローされます。
ms.openlocfilehash: 301862e46a571754bcb4032c7c7bf87e3564268f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071209"
---
# <a name="range-offsetrange"></a><span data-ttu-id="24692-105">範囲:OffsetRange</span><span class="sxs-lookup"><span data-stu-id="24692-105">Range: OffsetRange</span></span>

> <span data-ttu-id="24692-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24692-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24692-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24692-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="24692-p103">指定した範囲からのオフセットで範囲を表すオブジェクトを取得します。返される範囲のディメンションは、この範囲と一致します。結果の範囲が、ワークシートのグリッドの境界線の外にはみ出る場合は、例外がスローされます。</span><span class="sxs-lookup"><span data-stu-id="24692-p103">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="24692-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="24692-111">Permissions</span></span>
<span data-ttu-id="24692-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24692-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24692-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24692-114">Permission type</span></span>      | <span data-ttu-id="24692-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="24692-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24692-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24692-116">Delegated (work or school account)</span></span> | <span data-ttu-id="24692-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24692-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24692-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24692-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24692-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24692-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="24692-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24692-120">Application</span></span> | <span data-ttu-id="24692-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24692-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24692-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24692-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="24692-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24692-123">Request headers</span></span>
| <span data-ttu-id="24692-124">名前</span><span class="sxs-lookup"><span data-stu-id="24692-124">Name</span></span>       | <span data-ttu-id="24692-125">説明</span><span class="sxs-lookup"><span data-stu-id="24692-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="24692-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="24692-126">Authorization</span></span>  | <span data-ttu-id="24692-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="24692-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24692-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="24692-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="24692-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="24692-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24692-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="24692-132">Request body</span></span>
<span data-ttu-id="24692-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="24692-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="24692-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="24692-134">Parameter</span></span>    | <span data-ttu-id="24692-135">型</span><span class="sxs-lookup"><span data-stu-id="24692-135">Type</span></span>   |<span data-ttu-id="24692-136">説明</span><span class="sxs-lookup"><span data-stu-id="24692-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24692-137">rowOffset</span><span class="sxs-lookup"><span data-stu-id="24692-137">rowOffset</span></span>|<span data-ttu-id="24692-138">数値</span><span class="sxs-lookup"><span data-stu-id="24692-138">number</span></span>|<span data-ttu-id="24692-p107">範囲をオフセットする行数 (正、負、または 0)。正の値は下方向へのオフセットです。また、負の値は上方向へのオフセットです。</span><span class="sxs-lookup"><span data-stu-id="24692-p107">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="24692-141">columnOffset</span><span class="sxs-lookup"><span data-stu-id="24692-141">columnOffset</span></span>|<span data-ttu-id="24692-142">数値</span><span class="sxs-lookup"><span data-stu-id="24692-142">number</span></span>|<span data-ttu-id="24692-p108">範囲をオフセットする列数 (正、負、または 0)。正の値は右方向へのオフセットです。また、負の値は左方向へのオフセットです。</span><span class="sxs-lookup"><span data-stu-id="24692-p108">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="24692-145">応答</span><span class="sxs-lookup"><span data-stu-id="24692-145">Response</span></span>

<span data-ttu-id="24692-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24692-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24692-147">例</span><span class="sxs-lookup"><span data-stu-id="24692-147">Example</span></span>
<span data-ttu-id="24692-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="24692-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24692-149">要求</span><span class="sxs-lookup"><span data-stu-id="24692-149">Request</span></span>
<span data-ttu-id="24692-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24692-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/OffsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": {
  },
  "columnOffset": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="24692-151">応答</span><span class="sxs-lookup"><span data-stu-id="24692-151">Response</span></span>
<span data-ttu-id="24692-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24692-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: OffsetRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->