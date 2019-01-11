---
title: '範囲: 挿入'
description: この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。
localization_priority: Normal
ms.openlocfilehash: 0e7ab0d729dad4eec7fb455774cfed19bf4f5013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831515"
---
# <a name="range-insert"></a><span data-ttu-id="543d1-104">範囲: 挿入</span><span class="sxs-lookup"><span data-stu-id="543d1-104">Range: insert</span></span>

> <span data-ttu-id="543d1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="543d1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="543d1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="543d1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="543d1-p103">この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="543d1-p103">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="543d1-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="543d1-109">Permissions</span></span>
<span data-ttu-id="543d1-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="543d1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="543d1-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="543d1-112">Permission type</span></span>      | <span data-ttu-id="543d1-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="543d1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="543d1-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="543d1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="543d1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="543d1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="543d1-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="543d1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="543d1-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="543d1-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="543d1-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="543d1-118">Application</span></span> | <span data-ttu-id="543d1-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="543d1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="543d1-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="543d1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="543d1-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="543d1-121">Request headers</span></span>
| <span data-ttu-id="543d1-122">名前</span><span class="sxs-lookup"><span data-stu-id="543d1-122">Name</span></span>       | <span data-ttu-id="543d1-123">説明</span><span class="sxs-lookup"><span data-stu-id="543d1-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="543d1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="543d1-124">Authorization</span></span>  | <span data-ttu-id="543d1-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="543d1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="543d1-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="543d1-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="543d1-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="543d1-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="543d1-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="543d1-130">Request body</span></span>
<span data-ttu-id="543d1-131">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="543d1-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="543d1-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="543d1-132">Parameter</span></span>    | <span data-ttu-id="543d1-133">Type</span><span class="sxs-lookup"><span data-stu-id="543d1-133">Type</span></span>   |<span data-ttu-id="543d1-134">説明</span><span class="sxs-lookup"><span data-stu-id="543d1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="543d1-135"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="543d1-135">shift</span></span>|<span data-ttu-id="543d1-136">文字列</span><span class="sxs-lookup"><span data-stu-id="543d1-136">string</span></span>|<span data-ttu-id="543d1-p107">セルをシフトする方向を指定します。可能な値は、`Down`、`Right` です。</span><span class="sxs-lookup"><span data-stu-id="543d1-p107">Specifies which way to shift the cells.  Possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="543d1-139">応答</span><span class="sxs-lookup"><span data-stu-id="543d1-139">Response</span></span>

<span data-ttu-id="543d1-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="543d1-140">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="543d1-141">例</span><span class="sxs-lookup"><span data-stu-id="543d1-141">Example</span></span>
<span data-ttu-id="543d1-142">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="543d1-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="543d1-143">要求</span><span class="sxs-lookup"><span data-stu-id="543d1-143">Request</span></span>
<span data-ttu-id="543d1-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="543d1-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="543d1-145">応答</span><span class="sxs-lookup"><span data-stu-id="543d1-145">Response</span></span>
<span data-ttu-id="543d1-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="543d1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
