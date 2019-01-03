---
title: ワークシート:Range
description: アドレスまたは名前で指定された範囲オブジェクトを取得します。
author: lumine2008
ms.openlocfilehash: fec1ea97be1ca2c094af7e32deac0b6a37f4f086
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319867"
---
# <a name="worksheet-range"></a><span data-ttu-id="6ae35-103">ワークシート:Range</span><span class="sxs-lookup"><span data-stu-id="6ae35-103">Worksheet: Range</span></span>

<span data-ttu-id="6ae35-104">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="6ae35-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ae35-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6ae35-105">Permissions</span></span>
<span data-ttu-id="6ae35-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ae35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ae35-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ae35-108">Permission type</span></span>      | <span data-ttu-id="6ae35-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ae35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ae35-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ae35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ae35-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ae35-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6ae35-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ae35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ae35-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ae35-113">Not supported.</span></span>    |
|<span data-ttu-id="6ae35-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ae35-114">Application</span></span> | <span data-ttu-id="6ae35-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ae35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ae35-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ae35-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="6ae35-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ae35-117">Request headers</span></span>
| <span data-ttu-id="6ae35-118">名前</span><span class="sxs-lookup"><span data-stu-id="6ae35-118">Name</span></span>       | <span data-ttu-id="6ae35-119">説明</span><span class="sxs-lookup"><span data-stu-id="6ae35-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ae35-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ae35-120">Authorization</span></span>  | <span data-ttu-id="6ae35-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6ae35-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6ae35-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6ae35-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="6ae35-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="6ae35-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="6ae35-126">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="6ae35-126">Function parameters</span></span>

| <span data-ttu-id="6ae35-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6ae35-127">Parameter</span></span>    | <span data-ttu-id="6ae35-128">種類</span><span class="sxs-lookup"><span data-stu-id="6ae35-128">Type</span></span>   |<span data-ttu-id="6ae35-129">説明</span><span class="sxs-lookup"><span data-stu-id="6ae35-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ae35-130">address</span><span class="sxs-lookup"><span data-stu-id="6ae35-130">address</span></span>|<span data-ttu-id="6ae35-131">文字列</span><span class="sxs-lookup"><span data-stu-id="6ae35-131">string</span></span>|<span data-ttu-id="6ae35-p104">省略可能。範囲のアドレスまたは名前。指定されていない場合は、ワークシート全体の範囲が返されます。</span><span class="sxs-lookup"><span data-stu-id="6ae35-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="6ae35-135">応答</span><span class="sxs-lookup"><span data-stu-id="6ae35-135">Response</span></span>

<span data-ttu-id="6ae35-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6ae35-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ae35-137">例</span><span class="sxs-lookup"><span data-stu-id="6ae35-137">Example</span></span>
<span data-ttu-id="6ae35-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6ae35-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6ae35-139">要求</span><span class="sxs-lookup"><span data-stu-id="6ae35-139">Request</span></span>
<span data-ttu-id="6ae35-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ae35-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```

##### <a name="response"></a><span data-ttu-id="6ae35-141">応答</span><span class="sxs-lookup"><span data-stu-id="6ae35-141">Response</span></span>
<span data-ttu-id="6ae35-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ae35-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="6ae35-145">場合、省略可能な`address`パラメーターが指定されていない、この関数は、全体のワークシートのセル範囲を返します。</span><span class="sxs-lookup"><span data-stu-id="6ae35-145">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="6ae35-146">要求</span><span class="sxs-lookup"><span data-stu-id="6ae35-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```

##### <a name="response"></a><span data-ttu-id="6ae35-147">応答</span><span class="sxs-lookup"><span data-stu-id="6ae35-147">Response</span></span>

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
  "description": "Worksheet: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->