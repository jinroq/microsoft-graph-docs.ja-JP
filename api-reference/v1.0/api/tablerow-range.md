---
title: TableRow:Range
description: 行全体に関連付けられた範囲オブジェクトを返します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 784e99c932f7a3dd747b66df6ebf5427504e2336
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024344"
---
# <a name="tablerow-range"></a><span data-ttu-id="97f27-103">TableRow:Range</span><span class="sxs-lookup"><span data-stu-id="97f27-103">TableRow: Range</span></span>

<span data-ttu-id="97f27-104">行全体に関連付けられた範囲オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="97f27-104">Returns the range object associated with the entire row.</span></span>
## <a name="permissions"></a><span data-ttu-id="97f27-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="97f27-105">Permissions</span></span>
<span data-ttu-id="97f27-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97f27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97f27-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="97f27-108">Permission type</span></span>      | <span data-ttu-id="97f27-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="97f27-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97f27-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="97f27-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97f27-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97f27-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="97f27-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="97f27-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97f27-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97f27-113">Not supported.</span></span>    |
|<span data-ttu-id="97f27-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="97f27-114">Application</span></span> | <span data-ttu-id="97f27-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97f27-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97f27-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97f27-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="97f27-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="97f27-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows/{index}/range
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows/{index}/range

```
## <a name="request-headers"></a><span data-ttu-id="97f27-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97f27-118">Request headers</span></span>
| <span data-ttu-id="97f27-119">名前</span><span class="sxs-lookup"><span data-stu-id="97f27-119">Name</span></span>       | <span data-ttu-id="97f27-120">説明</span><span class="sxs-lookup"><span data-stu-id="97f27-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97f27-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97f27-121">Authorization</span></span>  | <span data-ttu-id="97f27-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="97f27-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97f27-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="97f27-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="97f27-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="97f27-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97f27-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="97f27-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="97f27-128">応答</span><span class="sxs-lookup"><span data-stu-id="97f27-128">Response</span></span>

<span data-ttu-id="97f27-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="97f27-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97f27-130">例</span><span class="sxs-lookup"><span data-stu-id="97f27-130">Example</span></span>
<span data-ttu-id="97f27-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="97f27-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="97f27-132">要求</span><span class="sxs-lookup"><span data-stu-id="97f27-132">Request</span></span>
<span data-ttu-id="97f27-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="97f27-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablerow_range"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97f27-134">C#</span><span class="sxs-lookup"><span data-stu-id="97f27-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablerow-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97f27-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="97f27-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerow-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97f27-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="97f27-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablerow-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97f27-137">Java</span><span class="sxs-lookup"><span data-stu-id="97f27-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tablerow-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="97f27-138">応答</span><span class="sxs-lookup"><span data-stu-id="97f27-138">Response</span></span>
<span data-ttu-id="97f27-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="97f27-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableRow: Range",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
