---
title: ワークシート:Range
description: アドレスまたは名前で指定された範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 949bbefa0f65c3dfa7daf54a092a315101d7ae79
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36307430"
---
# <a name="worksheet-range"></a><span data-ttu-id="feacd-103">ワークシート:Range</span><span class="sxs-lookup"><span data-stu-id="feacd-103">Worksheet: Range</span></span>

<span data-ttu-id="feacd-104">アドレスまたは名前で指定された範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="feacd-104">Gets the range object specified by the address or name.</span></span>
## <a name="permissions"></a><span data-ttu-id="feacd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="feacd-105">Permissions</span></span>
<span data-ttu-id="feacd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="feacd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="feacd-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="feacd-108">Permission type</span></span>      | <span data-ttu-id="feacd-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="feacd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="feacd-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="feacd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="feacd-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="feacd-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="feacd-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="feacd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="feacd-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="feacd-113">Not supported.</span></span>    |
|<span data-ttu-id="feacd-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="feacd-114">Application</span></span> | <span data-ttu-id="feacd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="feacd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="feacd-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="feacd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets/{id|name}/range

```
## <a name="request-headers"></a><span data-ttu-id="feacd-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="feacd-117">Request headers</span></span>
| <span data-ttu-id="feacd-118">名前</span><span class="sxs-lookup"><span data-stu-id="feacd-118">Name</span></span>       | <span data-ttu-id="feacd-119">説明</span><span class="sxs-lookup"><span data-stu-id="feacd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="feacd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="feacd-120">Authorization</span></span>  | <span data-ttu-id="feacd-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="feacd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="feacd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="feacd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="feacd-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="feacd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="feacd-126">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="feacd-126">Function parameters</span></span>

| <span data-ttu-id="feacd-127">パラメーター</span><span class="sxs-lookup"><span data-stu-id="feacd-127">Parameter</span></span>    | <span data-ttu-id="feacd-128">型</span><span class="sxs-lookup"><span data-stu-id="feacd-128">Type</span></span>   |<span data-ttu-id="feacd-129">説明</span><span class="sxs-lookup"><span data-stu-id="feacd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="feacd-130">address</span><span class="sxs-lookup"><span data-stu-id="feacd-130">address</span></span>|<span data-ttu-id="feacd-131">string</span><span class="sxs-lookup"><span data-stu-id="feacd-131">string</span></span>|<span data-ttu-id="feacd-p104">省略可能。範囲のアドレスまたは名前。指定されていない場合は、ワークシート全体の範囲が返されます。</span><span class="sxs-lookup"><span data-stu-id="feacd-p104">Optional. The address or the name of the range. If not specified, the entire worksheet range is returned.</span></span>|

## <a name="response"></a><span data-ttu-id="feacd-135">応答</span><span class="sxs-lookup"><span data-stu-id="feacd-135">Response</span></span>

<span data-ttu-id="feacd-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="feacd-136">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feacd-137">例</span><span class="sxs-lookup"><span data-stu-id="feacd-137">Example</span></span>
<span data-ttu-id="feacd-138">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="feacd-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="feacd-139">要求</span><span class="sxs-lookup"><span data-stu-id="feacd-139">Request</span></span>
<span data-ttu-id="feacd-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="feacd-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="feacd-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="feacd-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range(address='A1:B2')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="feacd-142">C#</span><span class="sxs-lookup"><span data-stu-id="feacd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="feacd-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="feacd-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="feacd-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="feacd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="feacd-145">Java</span><span class="sxs-lookup"><span data-stu-id="feacd-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="feacd-146">応答</span><span class="sxs-lookup"><span data-stu-id="feacd-146">Response</span></span>
<span data-ttu-id="feacd-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="feacd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="feacd-150">オプション`address`のパラメーターが指定されていない場合、この関数はワークシートの範囲全体を返します。</span><span class="sxs-lookup"><span data-stu-id="feacd-150">If the optional `address` parameter is not specified, this function returns the entire worksheet range.</span></span>

##### <a name="request"></a><span data-ttu-id="feacd-151">要求</span><span class="sxs-lookup"><span data-stu-id="feacd-151">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="feacd-152">プロトコル</span><span class="sxs-lookup"><span data-stu-id="feacd-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "worksheet_range_noaddress"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="feacd-153">C#</span><span class="sxs-lookup"><span data-stu-id="feacd-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/worksheet-range-noaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="feacd-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="feacd-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/worksheet-range-noaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="feacd-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="feacd-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/worksheet-range-noaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="feacd-156">Java</span><span class="sxs-lookup"><span data-stu-id="feacd-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/worksheet-range-noaddress-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="feacd-157">応答</span><span class="sxs-lookup"><span data-stu-id="feacd-157">Response</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
