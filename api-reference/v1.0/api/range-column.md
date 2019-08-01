---
title: 範囲:列
description: 範囲に含まれる列を 1 つ取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 9942d09a0c47ee47b7b1a2781bbee87c636cd2f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025352"
---
# <a name="range-column"></a><span data-ttu-id="1c50b-103">範囲:列</span><span class="sxs-lookup"><span data-stu-id="1c50b-103">Range: Column</span></span>

<span data-ttu-id="1c50b-104">範囲に含まれる列を 1 つ取得します。</span><span class="sxs-lookup"><span data-stu-id="1c50b-104">Gets a column contained in the range.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c50b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c50b-105">Permissions</span></span>
<span data-ttu-id="1c50b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c50b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c50b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c50b-108">Permission type</span></span>      | <span data-ttu-id="1c50b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c50b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c50b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c50b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c50b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c50b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1c50b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c50b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c50b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c50b-113">Not supported.</span></span>    |
|<span data-ttu-id="1c50b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c50b-114">Application</span></span> | <span data-ttu-id="1c50b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c50b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c50b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c50b-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c50b-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="1c50b-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names/{name}/range/column
GET /workbook/worksheets/{id|name}/range(address='<address>')/column
GET /workbook/tables/{id|name}/columns/{id|name}/range/column

```
## <a name="request-headers"></a><span data-ttu-id="1c50b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c50b-118">Request headers</span></span>
| <span data-ttu-id="1c50b-119">名前</span><span class="sxs-lookup"><span data-stu-id="1c50b-119">Name</span></span>       | <span data-ttu-id="1c50b-120">説明</span><span class="sxs-lookup"><span data-stu-id="1c50b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1c50b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c50b-121">Authorization</span></span>  | <span data-ttu-id="1c50b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1c50b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c50b-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1c50b-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="1c50b-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="1c50b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="path-parameters"></a><span data-ttu-id="1c50b-127">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="1c50b-127">Path parameters</span></span>
<span data-ttu-id="1c50b-128">要求パスに、次のパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="1c50b-128">In the request path, provide the following parameters.</span></span>

| <span data-ttu-id="1c50b-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1c50b-129">Parameter</span></span>    | <span data-ttu-id="1c50b-130">型</span><span class="sxs-lookup"><span data-stu-id="1c50b-130">Type</span></span>   |<span data-ttu-id="1c50b-131">説明</span><span class="sxs-lookup"><span data-stu-id="1c50b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c50b-132">column</span><span class="sxs-lookup"><span data-stu-id="1c50b-132">column</span></span>|<span data-ttu-id="1c50b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="1c50b-133">Int32</span></span>|<span data-ttu-id="1c50b-p104">取得する範囲の列番号。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="1c50b-p104">Column number of the range to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="1c50b-136">応答</span><span class="sxs-lookup"><span data-stu-id="1c50b-136">Response</span></span>

<span data-ttu-id="1c50b-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1c50b-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c50b-138">例</span><span class="sxs-lookup"><span data-stu-id="1c50b-138">Example</span></span>
<span data-ttu-id="1c50b-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="1c50b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1c50b-140">要求</span><span class="sxs-lookup"><span data-stu-id="1c50b-140">Request</span></span>
<span data-ttu-id="1c50b-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c50b-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "range_column"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/column(column=5)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c50b-142">C#</span><span class="sxs-lookup"><span data-stu-id="1c50b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-column-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c50b-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c50b-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-column-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c50b-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="1c50b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-column-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c50b-145">Java</span><span class="sxs-lookup"><span data-stu-id="1c50b-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-column-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c50b-146">応答</span><span class="sxs-lookup"><span data-stu-id="1c50b-146">Response</span></span>
<span data-ttu-id="1c50b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1c50b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Range: Column",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
