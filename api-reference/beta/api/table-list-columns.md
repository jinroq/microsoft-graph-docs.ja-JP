---
title: 列を一覧表示する
description: tablecolumn オブジェクトのリストを取得します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: c3598c7e579b8c767c500ed2ab47322520eb50f9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409552"
---
# <a name="list-columns"></a><span data-ttu-id="91193-103">列を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="91193-103">List columns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91193-104">tablecolumn オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="91193-104">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="91193-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91193-105">Permissions</span></span>
<span data-ttu-id="91193-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91193-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91193-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91193-108">Permission type</span></span>      | <span data-ttu-id="91193-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="91193-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91193-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91193-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91193-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91193-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91193-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91193-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91193-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91193-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91193-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91193-114">Application</span></span> | <span data-ttu-id="91193-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91193-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91193-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91193-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="91193-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="91193-117">Optional query parameters</span></span>
<span data-ttu-id="91193-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="91193-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="91193-119">
  [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) クエリ パラメーターを使用して結果をページングすると、信頼性の高い結果を得られます。</span><span class="sxs-lookup"><span data-stu-id="91193-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="91193-120">こうして、大きな結果セットに関連するパフォーマンスの問題を回避できます。</span><span class="sxs-lookup"><span data-stu-id="91193-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91193-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91193-121">Request headers</span></span>
| <span data-ttu-id="91193-122">名前</span><span class="sxs-lookup"><span data-stu-id="91193-122">Name</span></span>      |<span data-ttu-id="91193-123">説明</span><span class="sxs-lookup"><span data-stu-id="91193-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91193-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="91193-124">Authorization</span></span>  | <span data-ttu-id="91193-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="91193-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91193-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="91193-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="91193-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="91193-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91193-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="91193-130">Request body</span></span>
<span data-ttu-id="91193-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="91193-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91193-132">応答</span><span class="sxs-lookup"><span data-stu-id="91193-132">Response</span></span>

<span data-ttu-id="91193-133">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[workbookTableColumn](../resources/workbooktablecolumn.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="91193-133">If successful, this method returns a `200 OK` response code and collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91193-134">例</span><span class="sxs-lookup"><span data-stu-id="91193-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91193-135">要求</span><span class="sxs-lookup"><span data-stu-id="91193-135">Request</span></span>
<span data-ttu-id="91193-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91193-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="91193-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="91193-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="91193-138">C#</span><span class="sxs-lookup"><span data-stu-id="91193-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91193-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91193-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91193-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="91193-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91193-141">応答</span><span class="sxs-lookup"><span data-stu-id="91193-141">Response</span></span>
<span data-ttu-id="91193-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="91193-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

> <span data-ttu-id="91193-145">
  **注:\*\* [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) を使用して、多数の列をページングします。</span><span class="sxs-lookup"><span data-stu-id="91193-145">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="91193-146">例: </span><span class="sxs-lookup"><span data-stu-id="91193-146">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
