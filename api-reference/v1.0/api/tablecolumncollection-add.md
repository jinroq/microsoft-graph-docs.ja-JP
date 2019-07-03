---
title: 'TableColumnCollection: 追加'
description: テーブルに新しい列を追加します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d1ff9479cfc5f25cb87304126b17d5750ba3eb38
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445521"
---
# <a name="tablecolumncollection-add"></a><span data-ttu-id="862c6-103">TableColumnCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="862c6-103">TableColumnCollection: add</span></span>

<span data-ttu-id="862c6-104">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="862c6-104">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="862c6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="862c6-105">Permissions</span></span>
<span data-ttu-id="862c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="862c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="862c6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="862c6-108">Permission type</span></span>      | <span data-ttu-id="862c6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="862c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="862c6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="862c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="862c6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="862c6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="862c6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="862c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="862c6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="862c6-113">Not supported.</span></span>    |
|<span data-ttu-id="862c6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="862c6-114">Application</span></span> | <span data-ttu-id="862c6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="862c6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="862c6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="862c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="862c6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="862c6-117">Request headers</span></span>
| <span data-ttu-id="862c6-118">名前</span><span class="sxs-lookup"><span data-stu-id="862c6-118">Name</span></span>       | <span data-ttu-id="862c6-119">説明</span><span class="sxs-lookup"><span data-stu-id="862c6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="862c6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="862c6-120">Authorization</span></span>  | <span data-ttu-id="862c6-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="862c6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="862c6-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="862c6-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="862c6-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="862c6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="862c6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="862c6-126">Request body</span></span>
<span data-ttu-id="862c6-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="862c6-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="862c6-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="862c6-128">Parameter</span></span>    | <span data-ttu-id="862c6-129">型</span><span class="sxs-lookup"><span data-stu-id="862c6-129">Type</span></span>   |<span data-ttu-id="862c6-130">説明</span><span class="sxs-lookup"><span data-stu-id="862c6-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="862c6-131">index</span><span class="sxs-lookup"><span data-stu-id="862c6-131">index</span></span>|<span data-ttu-id="862c6-132">Int32</span><span class="sxs-lookup"><span data-stu-id="862c6-132">Int32</span></span>|<span data-ttu-id="862c6-p104">新しい列の相対位置を指定します。この位置の前の列は右にシフトされます。インデックス値は、最後の列のインデックス値と等しいか、小さくなります。そのため、テーブルの末尾に列を追加するためには使用できません。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="862c6-p104">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="862c6-137">values</span><span class="sxs-lookup"><span data-stu-id="862c6-137">values</span></span>|<span data-ttu-id="862c6-138">Json</span><span class="sxs-lookup"><span data-stu-id="862c6-138">Json</span></span>|<span data-ttu-id="862c6-p105">省略可能。テーブルの列の、書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="862c6-p105">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|
|<span data-ttu-id="862c6-141">name</span><span class="sxs-lookup"><span data-stu-id="862c6-141">name</span></span>|<span data-ttu-id="862c6-142">string</span><span class="sxs-lookup"><span data-stu-id="862c6-142">string</span></span>|<span data-ttu-id="862c6-143">name</span><span class="sxs-lookup"><span data-stu-id="862c6-143">name</span></span>
## <a name="response"></a><span data-ttu-id="862c6-144">応答</span><span class="sxs-lookup"><span data-stu-id="862c6-144">Response</span></span>

<span data-ttu-id="862c6-145">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="862c6-145">If successful, this method returns `200 OK` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="862c6-146">例</span><span class="sxs-lookup"><span data-stu-id="862c6-146">Example</span></span>
<span data-ttu-id="862c6-147">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="862c6-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="862c6-148">要求</span><span class="sxs-lookup"><span data-stu-id="862c6-148">Request</span></span>
<span data-ttu-id="862c6-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="862c6-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="862c6-150">プロトコル</span><span class="sxs-lookup"><span data-stu-id="862c6-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": 3,
  "values": [
    {
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="862c6-151">C#</span><span class="sxs-lookup"><span data-stu-id="862c6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tablecolumncollection-add-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="862c6-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="862c6-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablecolumncollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="862c6-153">目的-C</span><span class="sxs-lookup"><span data-stu-id="862c6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tablecolumncollection-add-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="862c6-154">応答</span><span class="sxs-lookup"><span data-stu-id="862c6-154">Response</span></span>
<span data-ttu-id="862c6-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="862c6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Inconsistent types between parameter (Object) and table (None)",
    "Error: /api-reference/v1.0/api/tablecolumncollection-add.md/tablecolumncollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Object)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
