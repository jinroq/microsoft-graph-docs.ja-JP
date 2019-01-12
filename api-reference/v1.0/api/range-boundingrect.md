---
title: 範囲:BoundingRect
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9e8f5ef8a4c7c55ead433b0aa0557ce5fca74ecc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953051"
---
# <a name="range-boundingrect"></a><span data-ttu-id="fd57a-103">範囲:BoundingRect</span><span class="sxs-lookup"><span data-stu-id="fd57a-103">Range: BoundingRect</span></span>

<span data-ttu-id="fd57a-p101">指定した範囲を包含する、最小の Range オブジェクトを取得します。たとえば、"B2:C5" と "D10:E15" の GetBoundingRect は、"B2:E16" になります。</span><span class="sxs-lookup"><span data-stu-id="fd57a-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>
## <a name="permissions"></a><span data-ttu-id="fd57a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd57a-106">Permissions</span></span>
<span data-ttu-id="fd57a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd57a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd57a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd57a-109">Permission type</span></span>      | <span data-ttu-id="fd57a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd57a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd57a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd57a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fd57a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd57a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fd57a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd57a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd57a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd57a-114">Not supported.</span></span>    |
|<span data-ttu-id="fd57a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd57a-115">Application</span></span> | <span data-ttu-id="fd57a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd57a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd57a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd57a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/boundingRect
GET /workbook/worksheets/{id|name}/range(address='<address>')/boundingRect
GET /workbook/tables/{id|name}/columns/{id|name}/range/boundingRect

```
## <a name="request-headers"></a><span data-ttu-id="fd57a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd57a-118">Request headers</span></span>
| <span data-ttu-id="fd57a-119">名前</span><span class="sxs-lookup"><span data-stu-id="fd57a-119">Name</span></span>       | <span data-ttu-id="fd57a-120">説明</span><span class="sxs-lookup"><span data-stu-id="fd57a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fd57a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd57a-121">Authorization</span></span>  | <span data-ttu-id="fd57a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fd57a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd57a-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fd57a-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="fd57a-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="fd57a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd57a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd57a-127">Request body</span></span>
<span data-ttu-id="fd57a-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd57a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fd57a-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fd57a-129">Parameter</span></span>    | <span data-ttu-id="fd57a-130">型</span><span class="sxs-lookup"><span data-stu-id="fd57a-130">Type</span></span>   |<span data-ttu-id="fd57a-131">説明</span><span class="sxs-lookup"><span data-stu-id="fd57a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd57a-132">anotherRange</span><span class="sxs-lookup"><span data-stu-id="fd57a-132">anotherRange</span></span>|<span data-ttu-id="fd57a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="fd57a-133">string</span></span>|<span data-ttu-id="fd57a-134">Range オブジェクト、アドレスまたは範囲名。</span><span class="sxs-lookup"><span data-stu-id="fd57a-134">The range object or address or range name.</span></span>|

## <a name="response"></a><span data-ttu-id="fd57a-135">応答</span><span class="sxs-lookup"><span data-stu-id="fd57a-135">Response</span></span>

<span data-ttu-id="fd57a-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fd57a-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd57a-137">例</span><span class="sxs-lookup"><span data-stu-id="fd57a-137">Example</span></span>
<span data-ttu-id="fd57a-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="fd57a-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fd57a-139">要求</span><span class="sxs-lookup"><span data-stu-id="fd57a-139">Request</span></span>
<span data-ttu-id="fd57a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fd57a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "isComposable": true,
  "name": "range_boundingrect"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/boundingRect
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="fd57a-141">応答</span><span class="sxs-lookup"><span data-stu-id="fd57a-141">Response</span></span>
<span data-ttu-id="fd57a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fd57a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: BoundingRect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
