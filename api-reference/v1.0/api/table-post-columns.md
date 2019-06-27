---
title: TableColumn を作成する
description: この API を使用して、新しい TableColumn を作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 300ff8804bda1314fa5918f28852b1e013abd064
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278933"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="04e77-103">TableColumn を作成する</span><span class="sxs-lookup"><span data-stu-id="04e77-103">Create TableColumn</span></span>

<span data-ttu-id="04e77-104">この API を使用して、新しい TableColumn を作成します。</span><span class="sxs-lookup"><span data-stu-id="04e77-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="04e77-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04e77-105">Permissions</span></span>
<span data-ttu-id="04e77-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04e77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e77-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04e77-108">Permission type</span></span>      | <span data-ttu-id="04e77-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04e77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04e77-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04e77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04e77-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04e77-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="04e77-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04e77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04e77-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e77-113">Not supported.</span></span>    |
|<span data-ttu-id="04e77-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04e77-114">Application</span></span> | <span data-ttu-id="04e77-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e77-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04e77-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04e77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="04e77-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04e77-117">Request headers</span></span>
| <span data-ttu-id="04e77-118">名前</span><span class="sxs-lookup"><span data-stu-id="04e77-118">Name</span></span>       | <span data-ttu-id="04e77-119">説明</span><span class="sxs-lookup"><span data-stu-id="04e77-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04e77-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e77-120">Authorization</span></span>  | <span data-ttu-id="04e77-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04e77-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04e77-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="04e77-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="04e77-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="04e77-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e77-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="04e77-126">Request body</span></span>
<span data-ttu-id="04e77-127">要求本文で、 [WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="04e77-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04e77-128">応答</span><span class="sxs-lookup"><span data-stu-id="04e77-128">Response</span></span>

<span data-ttu-id="04e77-129">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="04e77-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e77-130">例</span><span class="sxs-lookup"><span data-stu-id="04e77-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04e77-131">要求</span><span class="sxs-lookup"><span data-stu-id="04e77-131">Request</span></span>
<span data-ttu-id="04e77-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04e77-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="04e77-133">要求本文で、 [WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="04e77-133">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="04e77-134">応答</span><span class="sxs-lookup"><span data-stu-id="04e77-134">Response</span></span>
<span data-ttu-id="04e77-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04e77-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="04e77-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="04e77-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="04e77-139">C#</span><span class="sxs-lookup"><span data-stu-id="04e77-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04e77-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="04e77-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="04e77-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="04e77-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_tablecolumn_from_table-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-post-columns.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
