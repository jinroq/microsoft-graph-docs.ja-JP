---
title: 行を一覧表示する
description: tablerow オブジェクトの一覧を取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e93594a5b4e208213780c71d38cb489aa280ca7e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637851"
---
# <a name="list-rows"></a><span data-ttu-id="74820-103">行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="74820-103">List rows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74820-104">tablerow オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="74820-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="74820-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="74820-105">Permissions</span></span>
<span data-ttu-id="74820-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74820-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74820-108">Permission type</span></span>      | <span data-ttu-id="74820-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="74820-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74820-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74820-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74820-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74820-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74820-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74820-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74820-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74820-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="74820-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74820-114">Application</span></span> | <span data-ttu-id="74820-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74820-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74820-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74820-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="74820-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="74820-117">Optional query parameters</span></span>
<span data-ttu-id="74820-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="74820-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="74820-119">
  [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) クエリ パラメーターを使用して結果をページングすると、信頼性の高い結果を得られます。</span><span class="sxs-lookup"><span data-stu-id="74820-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="74820-120">こうして、大きな結果セットに関連するパフォーマンスの問題を回避できます。</span><span class="sxs-lookup"><span data-stu-id="74820-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74820-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74820-121">Request headers</span></span>
| <span data-ttu-id="74820-122">名前</span><span class="sxs-lookup"><span data-stu-id="74820-122">Name</span></span>      |<span data-ttu-id="74820-123">説明</span><span class="sxs-lookup"><span data-stu-id="74820-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="74820-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="74820-124">Authorization</span></span>  | <span data-ttu-id="74820-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="74820-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="74820-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="74820-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="74820-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="74820-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74820-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="74820-130">Request body</span></span>
<span data-ttu-id="74820-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="74820-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74820-132">応答</span><span class="sxs-lookup"><span data-stu-id="74820-132">Response</span></span>

<span data-ttu-id="74820-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookTableRow](../resources/workbooktablerow.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="74820-133">If successful, this method returns a `200 OK` response code and collection of [workbookTableRow](../resources/workbooktablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="74820-134">例</span><span class="sxs-lookup"><span data-stu-id="74820-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74820-135">要求</span><span class="sxs-lookup"><span data-stu-id="74820-135">Request</span></span>
<span data-ttu-id="74820-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74820-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="74820-137">応答</span><span class="sxs-lookup"><span data-stu-id="74820-137">Response</span></span>
<span data-ttu-id="74820-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74820-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 82

{
  "value": [
    {
      "index": 99,
      "values": "values-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74820-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="74820-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74820-142">Visual</span><span class="sxs-lookup"><span data-stu-id="74820-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_rows-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74820-143">Java</span><span class="sxs-lookup"><span data-stu-id="74820-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_rows-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

> <span data-ttu-id="74820-144">
  **注:\*\* [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) クエリ パラメーターを使用して、多数の行をページングします。</span><span class="sxs-lookup"><span data-stu-id="74820-144">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="74820-145">例:</span><span class="sxs-lookup"><span data-stu-id="74820-145">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/table-list-rows.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/table-list-rows.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
