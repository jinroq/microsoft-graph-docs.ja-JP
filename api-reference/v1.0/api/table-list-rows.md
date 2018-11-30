---
title: 行を一覧表示する
description: tablerow オブジェクトの一覧を取得します。
ms.openlocfilehash: d284b49b46c87ec30996d8b7ad0262af43365ad7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022701"
---
# <a name="list-rows"></a><span data-ttu-id="59a96-103">行を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="59a96-103">List rows</span></span>

<span data-ttu-id="59a96-104">tablerow オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="59a96-104">Retrieve a list of tablerow objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="59a96-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="59a96-105">Permissions</span></span>
<span data-ttu-id="59a96-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59a96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59a96-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="59a96-108">Permission type</span></span>      | <span data-ttu-id="59a96-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="59a96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59a96-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="59a96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59a96-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59a96-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="59a96-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="59a96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59a96-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59a96-113">Not supported.</span></span>    |
|<span data-ttu-id="59a96-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="59a96-114">Application</span></span> | <span data-ttu-id="59a96-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59a96-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59a96-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="59a96-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59a96-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="59a96-117">Optional query parameters</span></span>
<span data-ttu-id="59a96-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59a96-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>  <span data-ttu-id="59a96-119">
  [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) クエリ パラメーターを使用して結果をページングすると、信頼性の高い結果を得られます。</span><span class="sxs-lookup"><span data-stu-id="59a96-119">For reliable results, use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through the results.</span></span> <span data-ttu-id="59a96-120">こうして、大きな結果セットに関連するパフォーマンスの問題を回避できます。</span><span class="sxs-lookup"><span data-stu-id="59a96-120">This will help avoid performance problems related to large result sets.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59a96-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="59a96-121">Request headers</span></span>
| <span data-ttu-id="59a96-122">名前</span><span class="sxs-lookup"><span data-stu-id="59a96-122">Name</span></span>      |<span data-ttu-id="59a96-123">説明</span><span class="sxs-lookup"><span data-stu-id="59a96-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59a96-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="59a96-124">Authorization</span></span>  | <span data-ttu-id="59a96-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="59a96-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59a96-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="59a96-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="59a96-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="59a96-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59a96-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="59a96-130">Request body</span></span>
<span data-ttu-id="59a96-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="59a96-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59a96-132">応答</span><span class="sxs-lookup"><span data-stu-id="59a96-132">Response</span></span>

<span data-ttu-id="59a96-133">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[WorkbookTableRow](../resources/tablerow.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="59a96-133">If successful, this method returns a `200 OK` response code and collection of [WorkbookTableRow](../resources/tablerow.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59a96-134">例</span><span class="sxs-lookup"><span data-stu-id="59a96-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59a96-135">要求</span><span class="sxs-lookup"><span data-stu-id="59a96-135">Request</span></span>
<span data-ttu-id="59a96-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="59a96-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_rows"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5
```
##### <a name="response"></a><span data-ttu-id="59a96-137">応答</span><span class="sxs-lookup"><span data-stu-id="59a96-137">Response</span></span>
<span data-ttu-id="59a96-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="59a96-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
> <span data-ttu-id="59a96-141">
  **注:\*\* [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) クエリ パラメーターと [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) クエリ パラメーターを使用して、多数の行をページングします。</span><span class="sxs-lookup"><span data-stu-id="59a96-141">**Note:** Use the [$top](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top) and [$skip](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skip-parameter) query parameters to page through large numbers of rows.</span></span>

<span data-ttu-id="59a96-142">例:</span><span class="sxs-lookup"><span data-stu-id="59a96-142">Example:</span></span> 

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5`
`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows?$top=5&$skip=5`


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->