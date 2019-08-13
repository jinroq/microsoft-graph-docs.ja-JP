---
title: 'TableRowCollection: add　'
description: '表の末尾に行を追加します。 この api を使用して複数行データを受け入れることができることに注意してください。 一度に1つずつ行を追加すると、パフォーマンスが低下する可能性があります。 推奨される方法は、単一の行を挿入するのではなく、1回の呼び出しで複数の行をまとめてバッチ処理することです。 最良の結果を得るには、アプリケーション側に挿入する行を収集して、単一の行の追加操作を実行します。 行数を試してみて、単一の API 呼び出しで使用するための最適な行数を決定します。 '
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 12166f656429938cc0ee92ca8c7537fa7560e026
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316326"
---
# <a name="tablerowcollection-add"></a><span data-ttu-id="32cdf-108">TableRowCollection: add　</span><span class="sxs-lookup"><span data-stu-id="32cdf-108">TableRowCollection: add</span></span>

<span data-ttu-id="32cdf-109">表の末尾に行を追加します。</span><span class="sxs-lookup"><span data-stu-id="32cdf-109">Adds rows to the end of the table.</span></span> <span data-ttu-id="32cdf-110">この api を使用して複数行データを受け入れることができることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="32cdf-110">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="32cdf-111">一度に1つずつ行を追加すると、パフォーマンスが低下する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="32cdf-111">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="32cdf-112">推奨される方法は、単一の行を挿入するのではなく、1回の呼び出しで複数の行をまとめてバッチ処理することです。</span><span class="sxs-lookup"><span data-stu-id="32cdf-112">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="32cdf-113">最良の結果を得るには、アプリケーション側に挿入する行を収集して、単一の行の追加操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="32cdf-113">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="32cdf-114">行数を試してみて、単一の API 呼び出しで使用するための最適な行数を決定します。</span><span class="sxs-lookup"><span data-stu-id="32cdf-114">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="32cdf-115">エラー処理</span><span class="sxs-lookup"><span data-stu-id="32cdf-115">Error Handling</span></span>

<span data-ttu-id="32cdf-116">この要求に対して、504 HTTP エラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32cdf-116">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="32cdf-117">このエラーに対する適切な対応は、要求を繰り返すことです。</span><span class="sxs-lookup"><span data-stu-id="32cdf-117">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="32cdf-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="32cdf-118">Permissions</span></span>
<span data-ttu-id="32cdf-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32cdf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32cdf-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32cdf-121">Permission type</span></span>      | <span data-ttu-id="32cdf-122">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="32cdf-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32cdf-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32cdf-123">Delegated (work or school account)</span></span> | <span data-ttu-id="32cdf-124">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32cdf-124">Files.ReadWrite</span></span>    |
|<span data-ttu-id="32cdf-125">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32cdf-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32cdf-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32cdf-126">Not supported.</span></span>    |
|<span data-ttu-id="32cdf-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32cdf-127">Application</span></span> | <span data-ttu-id="32cdf-128">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32cdf-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="32cdf-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32cdf-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="32cdf-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32cdf-130">Request headers</span></span>
| <span data-ttu-id="32cdf-131">名前</span><span class="sxs-lookup"><span data-stu-id="32cdf-131">Name</span></span>       | <span data-ttu-id="32cdf-132">説明</span><span class="sxs-lookup"><span data-stu-id="32cdf-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="32cdf-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="32cdf-133">Authorization</span></span>  | <span data-ttu-id="32cdf-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="32cdf-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32cdf-136">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="32cdf-136">Workbook-Session-Id</span></span>  | <span data-ttu-id="32cdf-p106">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="32cdf-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32cdf-139">要求本文</span><span class="sxs-lookup"><span data-stu-id="32cdf-139">Request body</span></span>
<span data-ttu-id="32cdf-140">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="32cdf-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32cdf-141">パラメーター</span><span class="sxs-lookup"><span data-stu-id="32cdf-141">Parameter</span></span>    | <span data-ttu-id="32cdf-142">型</span><span class="sxs-lookup"><span data-stu-id="32cdf-142">Type</span></span>   |<span data-ttu-id="32cdf-143">説明</span><span class="sxs-lookup"><span data-stu-id="32cdf-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32cdf-144">index</span><span class="sxs-lookup"><span data-stu-id="32cdf-144">index</span></span>|<span data-ttu-id="32cdf-145">Int32</span><span class="sxs-lookup"><span data-stu-id="32cdf-145">Int32</span></span>|<span data-ttu-id="32cdf-p107">省略可能。新しい行の相対位置を指定します。null の場合、最後に追加が行われます。挿入した行の下のすべての行が下方向にシフトします。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="32cdf-p107">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="32cdf-151">values</span><span class="sxs-lookup"><span data-stu-id="32cdf-151">values</span></span>|<span data-ttu-id="32cdf-152">Json</span><span class="sxs-lookup"><span data-stu-id="32cdf-152">Json</span></span>|<span data-ttu-id="32cdf-p108">省略可能。テーブルの行の書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="32cdf-p108">Optional. A 2-dimensional array of unformatted values of the table row.</span></span>|

## <a name="response"></a><span data-ttu-id="32cdf-155">応答</span><span class="sxs-lookup"><span data-stu-id="32cdf-155">Response</span></span>

<span data-ttu-id="32cdf-156">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[WorkbookTableRow](../resources/tablerow.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="32cdf-156">If successful, this method returns `200 OK` response code and [WorkbookTableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32cdf-157">例</span><span class="sxs-lookup"><span data-stu-id="32cdf-157">Example</span></span>
<span data-ttu-id="32cdf-158">この例では、テーブルの最後に2行のデータが挿入されます。</span><span class="sxs-lookup"><span data-stu-id="32cdf-158">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="32cdf-159">要求</span><span class="sxs-lookup"><span data-stu-id="32cdf-159">Request</span></span>
<span data-ttu-id="32cdf-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32cdf-160">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="32cdf-161">プロトコル</span><span class="sxs-lookup"><span data-stu-id="32cdf-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "index": 5,
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32cdf-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32cdf-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tablerowcollection-add-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32cdf-163">応答</span><span class="sxs-lookup"><span data-stu-id="32cdf-163">Response</span></span>
<span data-ttu-id="32cdf-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32cdf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRowCollection: add",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Inconsistent types between parameter (Collection) and table (None)",
    "Error: /api-reference/v1.0/api/tablerowcollection-add.md/tablerowcollection_add/values:
      Type mismatch between example and table. Parameter name: values; example type (Collection(Collection)) is a collection, while the table description type (microsoft.graph.Json) is not."
  ],
  "tocPath": ""
}-->
