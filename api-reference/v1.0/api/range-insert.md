---
title: '範囲: 挿入'
description: この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。
ms.openlocfilehash: 242db28474965493ceb8a584e8d9fb01679f13d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020283"
---
# <a name="range-insert"></a><span data-ttu-id="53f96-104">範囲: 挿入</span><span class="sxs-lookup"><span data-stu-id="53f96-104">Range: insert</span></span>

<span data-ttu-id="53f96-p102">この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="53f96-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="53f96-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="53f96-107">Permissions</span></span>
<span data-ttu-id="53f96-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53f96-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53f96-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53f96-110">Permission type</span></span>      | <span data-ttu-id="53f96-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="53f96-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53f96-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53f96-112">Delegated (work or school account)</span></span> | <span data-ttu-id="53f96-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="53f96-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="53f96-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53f96-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53f96-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53f96-115">Not supported.</span></span>    |
|<span data-ttu-id="53f96-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53f96-116">Application</span></span> | <span data-ttu-id="53f96-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53f96-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="53f96-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53f96-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="53f96-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53f96-119">Request headers</span></span>
| <span data-ttu-id="53f96-120">名前</span><span class="sxs-lookup"><span data-stu-id="53f96-120">Name</span></span>       | <span data-ttu-id="53f96-121">説明</span><span class="sxs-lookup"><span data-stu-id="53f96-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53f96-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53f96-122">Authorization</span></span>  | <span data-ttu-id="53f96-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="53f96-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53f96-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="53f96-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="53f96-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="53f96-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53f96-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="53f96-128">Request body</span></span>
<span data-ttu-id="53f96-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="53f96-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="53f96-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="53f96-130">Parameter</span></span>    | <span data-ttu-id="53f96-131">型</span><span class="sxs-lookup"><span data-stu-id="53f96-131">Type</span></span>   |<span data-ttu-id="53f96-132">説明</span><span class="sxs-lookup"><span data-stu-id="53f96-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53f96-133"><legacyBold>Shift</legacyBold></span><span class="sxs-lookup"><span data-stu-id="53f96-133">shift</span></span>|<span data-ttu-id="53f96-134">文字列</span><span class="sxs-lookup"><span data-stu-id="53f96-134">string</span></span>|<span data-ttu-id="53f96-135">セルをシフトする方向を指定します。</span><span class="sxs-lookup"><span data-stu-id="53f96-135">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="53f96-136">可能な値: `Down`、 `Right`。</span><span class="sxs-lookup"><span data-stu-id="53f96-136">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="53f96-137">応答</span><span class="sxs-lookup"><span data-stu-id="53f96-137">Response</span></span>

<span data-ttu-id="53f96-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53f96-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53f96-139">例</span><span class="sxs-lookup"><span data-stu-id="53f96-139">Example</span></span>
<span data-ttu-id="53f96-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="53f96-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="53f96-141">要求</span><span class="sxs-lookup"><span data-stu-id="53f96-141">Request</span></span>
<span data-ttu-id="53f96-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53f96-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_insert"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/insert
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <a name="response"></a><span data-ttu-id="53f96-143">応答</span><span class="sxs-lookup"><span data-stu-id="53f96-143">Response</span></span>
<span data-ttu-id="53f96-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53f96-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: insert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->