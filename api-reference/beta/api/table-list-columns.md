---
title: 列を一覧表示する
description: tablecolumn オブジェクトのリストを取得します。
author: lumine2008
ms.openlocfilehash: 18bd254a1d45e95d35862c33a59e9ce1c70de6ba
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306805"
---
# <a name="list-columns"></a><span data-ttu-id="5fa8c-103">列を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5fa8c-103">List columns</span></span>

> <span data-ttu-id="5fa8c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fa8c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5fa8c-106">tablecolumn オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-106">Retrieve a list of tablecolumn objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5fa8c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5fa8c-107">Permissions</span></span>
<span data-ttu-id="5fa8c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fa8c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5fa8c-110">Permission type</span></span>      | <span data-ttu-id="5fa8c-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5fa8c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fa8c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5fa8c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5fa8c-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5fa8c-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5fa8c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5fa8c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fa8c-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5fa8c-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5fa8c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5fa8c-116">Application</span></span> | <span data-ttu-id="5fa8c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fa8c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5fa8c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/columns
GET /workbook/worksheets/{id|name}/tables/{id|name}/columns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5fa8c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5fa8c-119">Optional query parameters</span></span>
<span data-ttu-id="5fa8c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="5fa8c-121">
  [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) クエリ パラメーターを使用して結果をページングすると、信頼性の高い結果を得られます。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-121">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="5fa8c-122">こうして、大きな結果セットに関連するパフォーマンスの問題を回避できます。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-122">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fa8c-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5fa8c-123">Request headers</span></span>
| <span data-ttu-id="5fa8c-124">名前</span><span class="sxs-lookup"><span data-stu-id="5fa8c-124">Name</span></span>      |<span data-ttu-id="5fa8c-125">説明</span><span class="sxs-lookup"><span data-stu-id="5fa8c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5fa8c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5fa8c-126">Authorization</span></span>  | <span data-ttu-id="5fa8c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5fa8c-129">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="5fa8c-129">Workbook-Session-Id</span></span>  | <span data-ttu-id="5fa8c-p105">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fa8c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="5fa8c-132">Request body</span></span>
<span data-ttu-id="5fa8c-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fa8c-134">応答</span><span class="sxs-lookup"><span data-stu-id="5fa8c-134">Response</span></span>

<span data-ttu-id="5fa8c-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableColumn](../resources/tablecolumn.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-135">If successful, this method returns a `200 OK` response code and collection of [TableColumn](../resources/tablecolumn.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5fa8c-136">例</span><span class="sxs-lookup"><span data-stu-id="5fa8c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fa8c-137">要求</span><span class="sxs-lookup"><span data-stu-id="5fa8c-137">Request</span></span>
<span data-ttu-id="5fa8c-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_columns"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="5fa8c-139">応答</span><span class="sxs-lookup"><span data-stu-id="5fa8c-139">Response</span></span>
<span data-ttu-id="5fa8c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn",
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

> <span data-ttu-id="5fa8c-143">
  **注:\*\* [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) を使用して、多数の列をページングします。</span><span class="sxs-lookup"><span data-stu-id="5fa8c-143">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of columns.</span></span>

<span data-ttu-id="5fa8c-144">例:</span><span class="sxs-lookup"><span data-stu-id="5fa8c-144">Example:</span></span> 

`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5`
`https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns?$top=5&$skip=5`

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List columns",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->