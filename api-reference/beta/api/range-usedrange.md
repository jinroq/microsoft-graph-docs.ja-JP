---
title: 範囲:UsedRange
description: 指定した範囲オブジェクトのうち使用されている範囲を返します。
author: lumine2008
ms.openlocfilehash: a2a4d4a2de3b86b8682421a62e4e0b6b2cb7c2b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340706"
---
# <a name="range-usedrange"></a><span data-ttu-id="bc3ca-103">範囲:UsedRange</span><span class="sxs-lookup"><span data-stu-id="bc3ca-103">Range: UsedRange</span></span>

> <span data-ttu-id="bc3ca-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc3ca-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc3ca-106">指定した範囲オブジェクトのうち使用されている範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-106">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc3ca-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bc3ca-107">Permissions</span></span>
<span data-ttu-id="bc3ca-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc3ca-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc3ca-110">Permission type</span></span>      | <span data-ttu-id="bc3ca-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc3ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc3ca-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc3ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc3ca-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc3ca-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc3ca-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc3ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc3ca-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc3ca-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc3ca-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc3ca-116">Application</span></span> | <span data-ttu-id="bc3ca-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc3ca-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc3ca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="bc3ca-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc3ca-119">Request headers</span></span>
| <span data-ttu-id="bc3ca-120">名前</span><span class="sxs-lookup"><span data-stu-id="bc3ca-120">Name</span></span>       | <span data-ttu-id="bc3ca-121">説明</span><span class="sxs-lookup"><span data-stu-id="bc3ca-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc3ca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc3ca-122">Authorization</span></span>  | <span data-ttu-id="bc3ca-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc3ca-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bc3ca-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="bc3ca-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc3ca-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc3ca-128">Request body</span></span>
<span data-ttu-id="bc3ca-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bc3ca-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="bc3ca-130">Parameter</span></span>    | <span data-ttu-id="bc3ca-131">種類</span><span class="sxs-lookup"><span data-stu-id="bc3ca-131">Type</span></span>   |<span data-ttu-id="bc3ca-132">説明</span><span class="sxs-lookup"><span data-stu-id="bc3ca-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc3ca-133">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="bc3ca-133">valuesOnly</span></span>|<span data-ttu-id="bc3ca-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="bc3ca-134">boolean</span></span>|<span data-ttu-id="bc3ca-p105">省略可能。値の入っているセルのみを使用セルと見なします。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-p105">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="bc3ca-137">応答</span><span class="sxs-lookup"><span data-stu-id="bc3ca-137">Response</span></span>

<span data-ttu-id="bc3ca-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc3ca-139">例</span><span class="sxs-lookup"><span data-stu-id="bc3ca-139">Example</span></span>
<span data-ttu-id="bc3ca-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bc3ca-141">要求</span><span class="sxs-lookup"><span data-stu-id="bc3ca-141">Request</span></span>
<span data-ttu-id="bc3ca-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="bc3ca-143">応答</span><span class="sxs-lookup"><span data-stu-id="bc3ca-143">Response</span></span>
<span data-ttu-id="bc3ca-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bc3ca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->