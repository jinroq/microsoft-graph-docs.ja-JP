---
title: 範囲:OffsetRange
description: 指定した範囲からのオフセットで範囲を表すオブジェクトを取得します。返される範囲のディメンションは、この範囲と一致します。結果の範囲が、ワークシートのグリッドの境界線の外にはみ出る場合は、例外がスローされます。
ms.openlocfilehash: fcbc13fa17e0df97eceb4705e7775d733d1728dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023817"
---
# <a name="range-offsetrange"></a><span data-ttu-id="590bd-105">範囲:OffsetRange</span><span class="sxs-lookup"><span data-stu-id="590bd-105">Range: OffsetRange</span></span>

<span data-ttu-id="590bd-p102">指定した範囲からのオフセットで範囲を表すオブジェクトを取得します。返される範囲のディメンションは、この範囲と一致します。結果の範囲が、ワークシートのグリッドの境界線の外にはみ出る場合は、例外がスローされます。</span><span class="sxs-lookup"><span data-stu-id="590bd-p102">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="590bd-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="590bd-109">Permissions</span></span>
<span data-ttu-id="590bd-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="590bd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="590bd-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="590bd-112">Permission type</span></span>      | <span data-ttu-id="590bd-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="590bd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="590bd-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="590bd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="590bd-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="590bd-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="590bd-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="590bd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="590bd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="590bd-117">Not supported.</span></span>    |
|<span data-ttu-id="590bd-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="590bd-118">Application</span></span> | <span data-ttu-id="590bd-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="590bd-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="590bd-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="590bd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/offsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/offsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/offsetRange

```
## <a name="request-headers"></a><span data-ttu-id="590bd-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="590bd-121">Request headers</span></span>
| <span data-ttu-id="590bd-122">名前</span><span class="sxs-lookup"><span data-stu-id="590bd-122">Name</span></span>       | <span data-ttu-id="590bd-123">説明</span><span class="sxs-lookup"><span data-stu-id="590bd-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="590bd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="590bd-124">Authorization</span></span>  | <span data-ttu-id="590bd-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="590bd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="590bd-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="590bd-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="590bd-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="590bd-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="590bd-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="590bd-130">Request body</span></span>
<span data-ttu-id="590bd-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="590bd-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="590bd-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="590bd-132">Parameter</span></span>    | <span data-ttu-id="590bd-133">型</span><span class="sxs-lookup"><span data-stu-id="590bd-133">Type</span></span>   |<span data-ttu-id="590bd-134">説明</span><span class="sxs-lookup"><span data-stu-id="590bd-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="590bd-135">rowOffset</span><span class="sxs-lookup"><span data-stu-id="590bd-135">rowOffset</span></span>|<span data-ttu-id="590bd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="590bd-136">Int32</span></span>|<span data-ttu-id="590bd-p106">範囲をオフセットする行数 (正、負、または 0)。正の値は下方向へのオフセットです。また、負の値は上方向へのオフセットです。</span><span class="sxs-lookup"><span data-stu-id="590bd-p106">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="590bd-139">columnOffset</span><span class="sxs-lookup"><span data-stu-id="590bd-139">columnOffset</span></span>|<span data-ttu-id="590bd-140">Int32</span><span class="sxs-lookup"><span data-stu-id="590bd-140">Int32</span></span>|<span data-ttu-id="590bd-p107">範囲をオフセットする列数 (正、負、または 0)。正の値は右方向へのオフセットです。また、負の値は左方向へのオフセットです。</span><span class="sxs-lookup"><span data-stu-id="590bd-p107">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="590bd-143">応答</span><span class="sxs-lookup"><span data-stu-id="590bd-143">Response</span></span>

<span data-ttu-id="590bd-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="590bd-144">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="590bd-145">例</span><span class="sxs-lookup"><span data-stu-id="590bd-145">Example</span></span>
<span data-ttu-id="590bd-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="590bd-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="590bd-147">要求</span><span class="sxs-lookup"><span data-stu-id="590bd-147">Request</span></span>
<span data-ttu-id="590bd-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="590bd-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_offsetrange"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/offsetRange
Content-type: application/json
Content-length: 49

{
  "rowOffset": 3,
  "columnOffset": 5
}
```

##### <a name="response"></a><span data-ttu-id="590bd-149">応答</span><span class="sxs-lookup"><span data-stu-id="590bd-149">Response</span></span>
<span data-ttu-id="590bd-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="590bd-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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