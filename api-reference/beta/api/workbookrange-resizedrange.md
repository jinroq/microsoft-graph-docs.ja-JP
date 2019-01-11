---
title: 'workbookRange: resizedRange'
description: 現在の範囲オブジェクトに似た (ただし、右下隅がいくつかの行と列で拡張 (または縮小) されている) 範囲オブジェクトを取得します。
localization_priority: Normal
ms.openlocfilehash: fa8e8afcb230191da0ccfc69893f9ce5898eae57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870379"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="b0112-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="b0112-103">workbookRange: resizedRange</span></span>

> <span data-ttu-id="b0112-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b0112-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0112-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0112-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0112-106">現在の範囲オブジェクトに似た (ただし、右下隅がいくつかの行と列で拡張 (または縮小) されている) 範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b0112-106">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0112-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b0112-107">Permissions</span></span>
<span data-ttu-id="b0112-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0112-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0112-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0112-110">Permission type</span></span>      | <span data-ttu-id="b0112-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0112-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0112-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0112-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b0112-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0112-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0112-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0112-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0112-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0112-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b0112-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0112-116">Application</span></span> | <span data-ttu-id="b0112-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0112-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0112-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0112-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="b0112-119">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="b0112-119">Function parameters</span></span>

| <span data-ttu-id="b0112-120">Parameter</span><span class="sxs-lookup"><span data-stu-id="b0112-120">Parameter</span></span>    | <span data-ttu-id="b0112-121">Type</span><span class="sxs-lookup"><span data-stu-id="b0112-121">Type</span></span>   |<span data-ttu-id="b0112-122">説明</span><span class="sxs-lookup"><span data-stu-id="b0112-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0112-123">deltaRows</span><span class="sxs-lookup"><span data-stu-id="b0112-123">deltarows</span></span>|<span data-ttu-id="b0112-124">Int32</span><span class="sxs-lookup"><span data-stu-id="b0112-124">Int32</span></span>|<span data-ttu-id="b0112-p103">現在の範囲を基準にして、右下隅を拡張する行の数です。範囲を拡張するには正の数値、または範囲を縮小するには負の数値を使用します</span><span class="sxs-lookup"><span data-stu-id="b0112-p103">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="b0112-127">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="b0112-127">deltaColumns</span></span>|<span data-ttu-id="b0112-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b0112-128">Int32</span></span>|<span data-ttu-id="b0112-p104">現在の範囲を基準にして、右下隅を拡張する列の数です。範囲を拡張するには正の数値、または範囲を縮小するには負の数値を使用します。</span><span class="sxs-lookup"><span data-stu-id="b0112-p104">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b0112-131">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0112-131">Request headers</span></span>
| <span data-ttu-id="b0112-132">名前</span><span class="sxs-lookup"><span data-stu-id="b0112-132">Name</span></span>       | <span data-ttu-id="b0112-133">説明</span><span class="sxs-lookup"><span data-stu-id="b0112-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0112-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0112-134">Authorization</span></span>  | <span data-ttu-id="b0112-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b0112-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0112-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b0112-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="b0112-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="b0112-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0112-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0112-140">Request body</span></span>
<span data-ttu-id="b0112-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b0112-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0112-142">応答</span><span class="sxs-lookup"><span data-stu-id="b0112-142">Response</span></span>

<span data-ttu-id="b0112-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [workbookRange](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b0112-143">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0112-144">例</span><span class="sxs-lookup"><span data-stu-id="b0112-144">Example</span></span>
<span data-ttu-id="b0112-145">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="b0112-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b0112-146">要求</span><span class="sxs-lookup"><span data-stu-id="b0112-146">Request</span></span>
<span data-ttu-id="b0112-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0112-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="b0112-148">応答</span><span class="sxs-lookup"><span data-stu-id="b0112-148">Response</span></span>
<span data-ttu-id="b0112-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0112-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
