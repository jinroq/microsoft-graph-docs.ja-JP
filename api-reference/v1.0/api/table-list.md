---
title: TableCollection の一覧表示
description: テーブル オブジェクトの一覧を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b54ad094690d148c312003161fb929d9232b0750
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35278940"
---
# <a name="list-tablecollection"></a><span data-ttu-id="186eb-103">TableCollection の一覧表示</span><span class="sxs-lookup"><span data-stu-id="186eb-103">List TableCollection</span></span>

<span data-ttu-id="186eb-104">テーブル オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="186eb-104">Retrieve a list of table objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="186eb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="186eb-105">Permissions</span></span>
<span data-ttu-id="186eb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="186eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="186eb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="186eb-108">Permission type</span></span>      | <span data-ttu-id="186eb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="186eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="186eb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="186eb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="186eb-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="186eb-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="186eb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="186eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="186eb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="186eb-113">Not supported.</span></span>    |
|<span data-ttu-id="186eb-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="186eb-114">Application</span></span> | <span data-ttu-id="186eb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="186eb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="186eb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="186eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables
GET /workbook/worksheets/{id|name}/tables
```
## <a name="optional-query-parameters"></a><span data-ttu-id="186eb-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="186eb-117">Optional query parameters</span></span>
<span data-ttu-id="186eb-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="186eb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="186eb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="186eb-119">Request headers</span></span>
| <span data-ttu-id="186eb-120">名前</span><span class="sxs-lookup"><span data-stu-id="186eb-120">Name</span></span>      |<span data-ttu-id="186eb-121">説明</span><span class="sxs-lookup"><span data-stu-id="186eb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="186eb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="186eb-122">Authorization</span></span>  | <span data-ttu-id="186eb-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="186eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="186eb-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="186eb-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="186eb-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="186eb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="186eb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="186eb-128">Request body</span></span>
<span data-ttu-id="186eb-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="186eb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="186eb-130">応答</span><span class="sxs-lookup"><span data-stu-id="186eb-130">Response</span></span>

<span data-ttu-id="186eb-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[WorkbookTable](../resources/table.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="186eb-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookTable](../resources/table.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="186eb-132">例</span><span class="sxs-lookup"><span data-stu-id="186eb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="186eb-133">要求</span><span class="sxs-lookup"><span data-stu-id="186eb-133">Request</span></span>
<span data-ttu-id="186eb-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="186eb-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablecollection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables
```
##### <a name="response"></a><span data-ttu-id="186eb-135">応答</span><span class="sxs-lookup"><span data-stu-id="186eb-135">Response</span></span>
<span data-ttu-id="186eb-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="186eb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "id": "99",
      "name": "name-value",
      "showHeaders": true,
      "showTotals": true,
      "style": "style-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="186eb-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="186eb-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="186eb-140">C#</span><span class="sxs-lookup"><span data-stu-id="186eb-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tablecollection-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="186eb-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="186eb-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tablecollection-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="186eb-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="186eb-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_tablecollection-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
> <span data-ttu-id="186eb-143">**注:** [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターを使用して、多数のテーブルをページングします。</span><span class="sxs-lookup"><span data-stu-id="186eb-143">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) query parameters to page through large numbers of tables.</span></span>

<span data-ttu-id="186eb-144">例:</span><span class="sxs-lookup"><span data-stu-id="186eb-144">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TableCollection",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/table-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/table-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/table-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
