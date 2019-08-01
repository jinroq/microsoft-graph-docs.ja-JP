---
title: '範囲: 挿入'
description: この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: dba4588113466881ef656242c04b705b1a513885
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022228"
---
# <a name="range-insert"></a><span data-ttu-id="641cf-104">範囲: 挿入</span><span class="sxs-lookup"><span data-stu-id="641cf-104">Range: insert</span></span>

<span data-ttu-id="641cf-p102">この範囲を占めるセルまたはセルの範囲をワークシートに挿入し、領域を空けるために他のセルをシフトします。この時点で空き領域に位置する、新しい Range オブジェクトが返されます。</span><span class="sxs-lookup"><span data-stu-id="641cf-p102">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>
## <a name="permissions"></a><span data-ttu-id="641cf-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="641cf-107">Permissions</span></span>
<span data-ttu-id="641cf-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="641cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="641cf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="641cf-110">Permission type</span></span>      | <span data-ttu-id="641cf-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="641cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="641cf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="641cf-112">Delegated (work or school account)</span></span> | <span data-ttu-id="641cf-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="641cf-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="641cf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="641cf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="641cf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="641cf-115">Not supported.</span></span>    |
|<span data-ttu-id="641cf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="641cf-116">Application</span></span> | <span data-ttu-id="641cf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="641cf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="641cf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="641cf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/insert
POST /workbook/worksheets/{id|name}/range(address='<address>')/insert
POST /workbook/tables/{id|name}/columns/{id|name}/range/insert

```
## <a name="request-headers"></a><span data-ttu-id="641cf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="641cf-119">Request headers</span></span>
| <span data-ttu-id="641cf-120">名前</span><span class="sxs-lookup"><span data-stu-id="641cf-120">Name</span></span>       | <span data-ttu-id="641cf-121">説明</span><span class="sxs-lookup"><span data-stu-id="641cf-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="641cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="641cf-122">Authorization</span></span>  | <span data-ttu-id="641cf-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="641cf-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="641cf-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="641cf-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="641cf-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="641cf-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="641cf-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="641cf-128">Request body</span></span>
<span data-ttu-id="641cf-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="641cf-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="641cf-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="641cf-130">Parameter</span></span>    | <span data-ttu-id="641cf-131">型</span><span class="sxs-lookup"><span data-stu-id="641cf-131">Type</span></span>   |<span data-ttu-id="641cf-132">説明</span><span class="sxs-lookup"><span data-stu-id="641cf-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="641cf-133">Shift</span><span class="sxs-lookup"><span data-stu-id="641cf-133">shift</span></span>|<span data-ttu-id="641cf-134">string</span><span class="sxs-lookup"><span data-stu-id="641cf-134">string</span></span>|<span data-ttu-id="641cf-135">セルをシフトする方向を指定します。</span><span class="sxs-lookup"><span data-stu-id="641cf-135">Specifies which way to shift the cells.</span></span>  <span data-ttu-id="641cf-136">使用可能な値は`Down`、 `Right`、です。</span><span class="sxs-lookup"><span data-stu-id="641cf-136">The possible values are: `Down`, `Right`.</span></span>|

## <a name="response"></a><span data-ttu-id="641cf-137">応答</span><span class="sxs-lookup"><span data-stu-id="641cf-137">Response</span></span>

<span data-ttu-id="641cf-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="641cf-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="641cf-139">例</span><span class="sxs-lookup"><span data-stu-id="641cf-139">Example</span></span>
<span data-ttu-id="641cf-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="641cf-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="641cf-141">要求</span><span class="sxs-lookup"><span data-stu-id="641cf-141">Request</span></span>
<span data-ttu-id="641cf-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="641cf-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="641cf-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="641cf-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="641cf-144">C#</span><span class="sxs-lookup"><span data-stu-id="641cf-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-insert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="641cf-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="641cf-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-insert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="641cf-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="641cf-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-insert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="641cf-147">Java</span><span class="sxs-lookup"><span data-stu-id="641cf-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-insert-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="641cf-148">応答</span><span class="sxs-lookup"><span data-stu-id="641cf-148">Response</span></span>
<span data-ttu-id="641cf-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="641cf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
