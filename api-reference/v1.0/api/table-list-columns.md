---
title: 列を一覧表示する
description: tablecolumn オブジェクトのリストを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ea0e0845134d3446da81921c68d53faad259be56
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602902"
---
# <a name="list-columns"></a><span data-ttu-id="066a8-103">列を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="066a8-103">List columns</span></span>

<span data-ttu-id="066a8-104">tablecolumn オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="066a8-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="066a8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="066a8-105">Permissions</span></span>
<span data-ttu-id="066a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="066a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="066a8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="066a8-108">Permission type</span></span>      | <span data-ttu-id="066a8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="066a8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="066a8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="066a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="066a8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="066a8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="066a8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="066a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="066a8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="066a8-113">Not supported.</span></span>    |
|<span data-ttu-id="066a8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="066a8-114">Application</span></span> | <span data-ttu-id="066a8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="066a8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="066a8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="066a8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="066a8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="066a8-117">Optional query parameters</span></span>
<span data-ttu-id="066a8-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="066a8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="066a8-119">
  [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) クエリ パラメーターを使用して結果をページングすると、信頼性の高い結果を得られます。</span><span class="sxs-lookup"><span data-stu-id="066a8-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="066a8-120">こうして、大きな結果セットに関連するパフォーマンスの問題を回避できます。</span><span class="sxs-lookup"><span data-stu-id="066a8-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="066a8-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="066a8-121">Request headers</span></span>
| <span data-ttu-id="066a8-122">名前</span><span class="sxs-lookup"><span data-stu-id="066a8-122">Name</span></span>      |<span data-ttu-id="066a8-123">説明</span><span class="sxs-lookup"><span data-stu-id="066a8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="066a8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="066a8-124">Authorization</span></span>  | <span data-ttu-id="066a8-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="066a8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="066a8-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="066a8-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="066a8-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="066a8-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="066a8-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="066a8-130">Request body</span></span>
<span data-ttu-id="066a8-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="066a8-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="066a8-132">応答</span><span class="sxs-lookup"><span data-stu-id="066a8-132">Response</span></span>

<span data-ttu-id="066a8-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[WorkbookTableColumn](../resources/tablecolumn.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="066a8-133">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="066a8-134">例</span><span class="sxs-lookup"><span data-stu-id="066a8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="066a8-135">要求</span><span class="sxs-lookup"><span data-stu-id="066a8-135">Request</span></span>
<span data-ttu-id="066a8-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="066a8-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="066a8-137">応答</span><span class="sxs-lookup"><span data-stu-id="066a8-137">Response</span></span>
<span data-ttu-id="066a8-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="066a8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 126

{
  "value": [
    {
      "id": 99,
      "name": "name-value",
      "index": 99,
      "values": "values-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="066a8-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="066a8-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="066a8-142">Visual</span><span class="sxs-lookup"><span data-stu-id="066a8-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_columns-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="066a8-143">Java</span><span class="sxs-lookup"><span data-stu-id="066a8-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_columns-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

> <span data-ttu-id="066a8-144">
  **注:\*\* [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) を使用して、多数の列をページングします。</span><span class="sxs-lookup"><span data-stu-id="066a8-144">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="066a8-145">例: </span><span class="sxs-lookup"><span data-stu-id="066a8-145">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-list-columns.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-list-columns.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
