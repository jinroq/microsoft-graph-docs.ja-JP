---
title: 範囲:BoundingRect
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 169b65beb185c12c61a719aba68f139b31ce0a50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928438"
---
# <a name="range-boundingrect"></a><span data-ttu-id="0256e-103">範囲:BoundingRect</span><span class="sxs-lookup"><span data-stu-id="0256e-103">Range: BoundingRect</span></span>

> <span data-ttu-id="0256e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0256e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0256e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0256e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0256e-p102">指定した範囲を包含する、最小の Range オブジェクトを取得します。たとえば、"B2:C5" と "D10:E15" の GetBoundingRect は、"B2:E16" になります。</span><span class="sxs-lookup"><span data-stu-id="0256e-p102">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="0256e-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0256e-108">Permissions</span></span>
<span data-ttu-id="0256e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0256e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0256e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0256e-111">Permission type</span></span>      | <span data-ttu-id="0256e-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0256e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0256e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0256e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0256e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0256e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0256e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0256e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0256e-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0256e-116">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0256e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0256e-117">Application</span></span> | <span data-ttu-id="0256e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0256e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0256e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0256e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/BoundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/BoundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/BoundingRect

```
## <a name="request-headers"></a><span data-ttu-id="0256e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0256e-120">Request headers</span></span>
| <span data-ttu-id="0256e-121">名前</span><span class="sxs-lookup"><span data-stu-id="0256e-121">Name</span></span>       | <span data-ttu-id="0256e-122">説明</span><span class="sxs-lookup"><span data-stu-id="0256e-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0256e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0256e-123">Authorization</span></span>  | <span data-ttu-id="0256e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0256e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0256e-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0256e-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="0256e-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="0256e-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0256e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="0256e-129">Request body</span></span>
<span data-ttu-id="0256e-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0256e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0256e-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0256e-131">Parameter</span></span>    | <span data-ttu-id="0256e-132">Type</span><span class="sxs-lookup"><span data-stu-id="0256e-132">Type</span></span>   |<span data-ttu-id="0256e-133">説明</span><span class="sxs-lookup"><span data-stu-id="0256e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0256e-134">anotherRange</span><span class="sxs-lookup"><span data-stu-id="0256e-134">anotherRange</span></span>|<span data-ttu-id="0256e-135">文字列</span><span class="sxs-lookup"><span data-stu-id="0256e-135">string</span></span>|<span data-ttu-id="0256e-136">Range オブジェクト、アドレスまたは範囲名。</span><span class="sxs-lookup"><span data-stu-id="0256e-136">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="0256e-137">応答</span><span class="sxs-lookup"><span data-stu-id="0256e-137">Response</span></span>

<span data-ttu-id="0256e-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0256e-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0256e-139">例</span><span class="sxs-lookup"><span data-stu-id="0256e-139">Example</span></span>
<span data-ttu-id="0256e-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0256e-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0256e-141">要求</span><span class="sxs-lookup"><span data-stu-id="0256e-141">Request</span></span>
<span data-ttu-id="0256e-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0256e-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/BoundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="0256e-143">応答</span><span class="sxs-lookup"><span data-stu-id="0256e-143">Response</span></span>
<span data-ttu-id="0256e-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0256e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
