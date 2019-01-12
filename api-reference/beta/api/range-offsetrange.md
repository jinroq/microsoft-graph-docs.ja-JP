---
title: 範囲:OffsetRange
description: 指定した範囲からのオフセットで範囲を表すオブジェクトを取得します。返される範囲のディメンションは、この範囲と一致します。結果の範囲が、ワークシートのグリッドの境界線の外にはみ出る場合は、例外がスローされます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4f1a513a33185dba976398e31caf4996005feb67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925799"
---
# <a name="range-offsetrange"></a><span data-ttu-id="3b70f-105">範囲:OffsetRange</span><span class="sxs-lookup"><span data-stu-id="3b70f-105">Range: OffsetRange</span></span>

> <span data-ttu-id="3b70f-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b70f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b70f-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b70f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b70f-p103">指定した範囲からのオフセットで範囲を表すオブジェクトを取得します。返される範囲のディメンションは、この範囲と一致します。結果の範囲が、ワークシートのグリッドの境界線の外にはみ出る場合は、例外がスローされます。</span><span class="sxs-lookup"><span data-stu-id="3b70f-p103">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>
## <a name="permissions"></a><span data-ttu-id="3b70f-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b70f-111">Permissions</span></span>
<span data-ttu-id="3b70f-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b70f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b70f-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b70f-114">Permission type</span></span>      | <span data-ttu-id="3b70f-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b70f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b70f-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b70f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3b70f-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b70f-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b70f-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b70f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b70f-119">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3b70f-119">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3b70f-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b70f-120">Application</span></span> | <span data-ttu-id="3b70f-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b70f-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b70f-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b70f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/OffsetRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/OffsetRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/OffsetRange

```
## <a name="request-headers"></a><span data-ttu-id="3b70f-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b70f-123">Request headers</span></span>
| <span data-ttu-id="3b70f-124">名前</span><span class="sxs-lookup"><span data-stu-id="3b70f-124">Name</span></span>       | <span data-ttu-id="3b70f-125">説明</span><span class="sxs-lookup"><span data-stu-id="3b70f-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3b70f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b70f-126">Authorization</span></span>  | <span data-ttu-id="3b70f-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b70f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3b70f-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3b70f-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="3b70f-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="3b70f-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b70f-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b70f-132">Request body</span></span>
<span data-ttu-id="3b70f-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="3b70f-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3b70f-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3b70f-134">Parameter</span></span>    | <span data-ttu-id="3b70f-135">Type</span><span class="sxs-lookup"><span data-stu-id="3b70f-135">Type</span></span>   |<span data-ttu-id="3b70f-136">説明</span><span class="sxs-lookup"><span data-stu-id="3b70f-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b70f-137">rowOffset</span><span class="sxs-lookup"><span data-stu-id="3b70f-137">rowOffset</span></span>|<span data-ttu-id="3b70f-138">number</span><span class="sxs-lookup"><span data-stu-id="3b70f-138">number</span></span>|<span data-ttu-id="3b70f-p107">範囲をオフセットする行数 (正、負、または 0)。正の値は下方向へのオフセットです。また、負の値は上方向へのオフセットです。</span><span class="sxs-lookup"><span data-stu-id="3b70f-p107">The number of rows (positive, negative, or 0) by which the range is to be offset. Positive values are offset downward, and negative values are offset upward.</span></span>|
|<span data-ttu-id="3b70f-141">columnOffset</span><span class="sxs-lookup"><span data-stu-id="3b70f-141">columnOffset</span></span>|<span data-ttu-id="3b70f-142">number</span><span class="sxs-lookup"><span data-stu-id="3b70f-142">number</span></span>|<span data-ttu-id="3b70f-p108">範囲をオフセットする列数 (正、負、または 0)。正の値は右方向へのオフセットです。また、負の値は左方向へのオフセットです。</span><span class="sxs-lookup"><span data-stu-id="3b70f-p108">The number of columns (positive, negative, or 0) by which the range is to be offset. Positive values are offset to the right, and negative values are offset to the left.</span></span>|

## <a name="response"></a><span data-ttu-id="3b70f-145">応答</span><span class="sxs-lookup"><span data-stu-id="3b70f-145">Response</span></span>

<span data-ttu-id="3b70f-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3b70f-146">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b70f-147">例</span><span class="sxs-lookup"><span data-stu-id="3b70f-147">Example</span></span>
<span data-ttu-id="3b70f-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="3b70f-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3b70f-149">要求</span><span class="sxs-lookup"><span data-stu-id="3b70f-149">Request</span></span>
<span data-ttu-id="3b70f-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3b70f-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="3b70f-151">応答</span><span class="sxs-lookup"><span data-stu-id="3b70f-151">Response</span></span>
<span data-ttu-id="3b70f-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b70f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
