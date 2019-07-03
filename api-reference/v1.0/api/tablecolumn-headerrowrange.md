---
title: 'TableColumn: HeaderRowRange'
description: 列のヘッダー行に関連付けられた範囲オブジェクトを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6759894a7b7f781991b0c3b2c7568e05d7cee217
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456653"
---
# <a name="tablecolumn-headerrowrange"></a><span data-ttu-id="e91e7-103">TableColumn: HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="e91e7-103">TableColumn: HeaderRowRange</span></span>

<span data-ttu-id="e91e7-104">列のヘッダー行に関連付けられた範囲オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="e91e7-104">Gets the range object associated with the header row of the column.</span></span>
## <a name="permissions"></a><span data-ttu-id="e91e7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e91e7-105">Permissions</span></span>
<span data-ttu-id="e91e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e91e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e91e7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e91e7-108">Permission type</span></span>      | <span data-ttu-id="e91e7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e91e7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e91e7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e91e7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e91e7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e91e7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e91e7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e91e7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e91e7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e91e7-113">Not supported.</span></span>    |
|<span data-ttu-id="e91e7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e91e7-114">Application</span></span> | <span data-ttu-id="e91e7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e91e7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e91e7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e91e7-116">HTTP request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e91e7-117">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e91e7-117">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/headerRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/headerRowRange

```
## <a name="request-headers"></a><span data-ttu-id="e91e7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e91e7-118">Request headers</span></span>
| <span data-ttu-id="e91e7-119">名前</span><span class="sxs-lookup"><span data-stu-id="e91e7-119">Name</span></span>       | <span data-ttu-id="e91e7-120">説明</span><span class="sxs-lookup"><span data-stu-id="e91e7-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e91e7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e91e7-121">Authorization</span></span>  | <span data-ttu-id="e91e7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e91e7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e91e7-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e91e7-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="e91e7-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="e91e7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e91e7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e91e7-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e91e7-128">応答</span><span class="sxs-lookup"><span data-stu-id="e91e7-128">Response</span></span>

<span data-ttu-id="e91e7-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Range](../resources/range.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e91e7-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e91e7-130">例</span><span class="sxs-lookup"><span data-stu-id="e91e7-130">Example</span></span>
<span data-ttu-id="e91e7-131">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e91e7-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e91e7-132">要求</span><span class="sxs-lookup"><span data-stu-id="e91e7-132">Request</span></span>
<span data-ttu-id="e91e7-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e91e7-133">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "tablecolumn_headerrowrange",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/headerRowRange
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e91e7-134">C#</span><span class="sxs-lookup"><span data-stu-id="e91e7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumn-headerrowrange-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e91e7-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e91e7-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumn-headerrowrange-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e91e7-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="e91e7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumn-headerrowrange-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e91e7-137">応答</span><span class="sxs-lookup"><span data-stu-id="e91e7-137">Response</span></span>
<span data-ttu-id="e91e7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e91e7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "TableColumn: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
