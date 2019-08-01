---
title: TableColumn を作成する
description: この API を使用して、新しい TableColumn を作成します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: bc76e8445ecd1c4e7b92817970046301a41cce2d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021418"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="66dd7-103">TableColumn を作成する</span><span class="sxs-lookup"><span data-stu-id="66dd7-103">Create TableColumn</span></span>

<span data-ttu-id="66dd7-104">この API を使用して、新しい TableColumn を作成します。</span><span class="sxs-lookup"><span data-stu-id="66dd7-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="66dd7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66dd7-105">Permissions</span></span>
<span data-ttu-id="66dd7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66dd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66dd7-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66dd7-108">Permission type</span></span>      | <span data-ttu-id="66dd7-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66dd7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66dd7-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66dd7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66dd7-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66dd7-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="66dd7-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66dd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66dd7-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66dd7-113">Not supported.</span></span>    |
|<span data-ttu-id="66dd7-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66dd7-114">Application</span></span> | <span data-ttu-id="66dd7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66dd7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="66dd7-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66dd7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="66dd7-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66dd7-117">Request headers</span></span>
| <span data-ttu-id="66dd7-118">名前</span><span class="sxs-lookup"><span data-stu-id="66dd7-118">Name</span></span>       | <span data-ttu-id="66dd7-119">説明</span><span class="sxs-lookup"><span data-stu-id="66dd7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66dd7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="66dd7-120">Authorization</span></span>  | <span data-ttu-id="66dd7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66dd7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66dd7-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="66dd7-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="66dd7-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="66dd7-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66dd7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="66dd7-126">Request body</span></span>
<span data-ttu-id="66dd7-127">要求本文で、 [WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="66dd7-127">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66dd7-128">応答</span><span class="sxs-lookup"><span data-stu-id="66dd7-128">Response</span></span>

<span data-ttu-id="66dd7-129">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66dd7-129">If successful, this method returns `201 Created` response code and [WorkbookTableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66dd7-130">例</span><span class="sxs-lookup"><span data-stu-id="66dd7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66dd7-131">要求</span><span class="sxs-lookup"><span data-stu-id="66dd7-131">Request</span></span>
<span data-ttu-id="66dd7-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66dd7-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="66dd7-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="66dd7-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="66dd7-134">C#</span><span class="sxs-lookup"><span data-stu-id="66dd7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tablecolumn-from-table-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66dd7-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="66dd7-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tablecolumn-from-table-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="66dd7-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="66dd7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tablecolumn-from-table-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="66dd7-137">Java</span><span class="sxs-lookup"><span data-stu-id="66dd7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tablecolumn-from-table-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="66dd7-138">要求本文で、 [WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="66dd7-138">In the request body, supply a JSON representation of [WorkbookTableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="66dd7-139">応答</span><span class="sxs-lookup"><span data-stu-id="66dd7-139">Response</span></span>
<span data-ttu-id="66dd7-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66dd7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
