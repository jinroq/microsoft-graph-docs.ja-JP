---
title: TableRow を作成する
description: 'テーブルの末尾に行を追加します。 API がこの API を使用して複数の行データを受け入れることができることに注意してください。 一度に 1 行を追加すると、パフォーマンスが低下する可能性があります。 推奨されるアプローチは、1 つの行の挿入を行うのではなく、1 回の呼び出しでまとめて行をバッチ処理することです。 最良の結果を得るには、収集アプリケーション側で挿入して、1 つの行を実行する行操作を追加します。 理想的な 1 つの API 呼び出しで使用する行の数を決定する行の番号を試してください。 '
ms.openlocfilehash: c7a4340005f7eaea60d95c806475de92373e1364
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068701"
---
# <a name="create-tablerow"></a><span data-ttu-id="fe4e7-108">TableRow を作成する</span><span class="sxs-lookup"><span data-stu-id="fe4e7-108">Create TableRow</span></span>

> <span data-ttu-id="fe4e7-109">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-109">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe4e7-110">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-110">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe4e7-111">テーブルの末尾に行を追加します。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-111">Adds rows to the end of the table.</span></span> <span data-ttu-id="fe4e7-112">API がこの API を使用して複数の行データを受け入れることができることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-112">Note that the API can accept multiple rows data using this API.</span></span> <span data-ttu-id="fe4e7-113">一度に 1 行を追加すると、パフォーマンスが低下する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-113">Adding one row at a time could lead to performance degradation.</span></span> <span data-ttu-id="fe4e7-114">推奨されるアプローチは、1 つの行の挿入を行うのではなく、1 回の呼び出しでまとめて行をバッチ処理することです。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-114">The recommended approach would be to batch the rows together in a single call rather than doing single row insertion.</span></span> <span data-ttu-id="fe4e7-115">最良の結果を得るには、収集アプリケーション側で挿入して、1 つの行を実行する行操作を追加します。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-115">For best results, collect the rows to be inserted on the application side and perform single rows add operation.</span></span> <span data-ttu-id="fe4e7-116">理想的な 1 つの API 呼び出しで使用する行の数を決定する行の番号を試してください。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-116">Experiment with the number of rows to determine the ideal number of rows to use in single API call.</span></span> 

## <a name="error-handling"></a><span data-ttu-id="fe4e7-117">エラー処理</span><span class="sxs-lookup"><span data-stu-id="fe4e7-117">Error Handling</span></span>

<span data-ttu-id="fe4e7-118">この要求に対して、504 HTTP エラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-118">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="fe4e7-119">このエラーに対する適切な対応は、要求を繰り返すことです。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-119">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe4e7-120">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe4e7-120">Permissions</span></span>
<span data-ttu-id="fe4e7-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe4e7-123">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe4e7-123">Permission type</span></span>      | <span data-ttu-id="fe4e7-124">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe4e7-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe4e7-125">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe4e7-125">Delegated (work or school account)</span></span> | <span data-ttu-id="fe4e7-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe4e7-126">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe4e7-127">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe4e7-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe4e7-128">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-128">Not supported.</span></span>    |
|<span data-ttu-id="fe4e7-129">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe4e7-129">Application</span></span> | <span data-ttu-id="fe4e7-130">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe4e7-131">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe4e7-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows/add

```
## <a name="request-headers"></a><span data-ttu-id="fe4e7-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe4e7-132">Request headers</span></span>
| <span data-ttu-id="fe4e7-133">名前</span><span class="sxs-lookup"><span data-stu-id="fe4e7-133">Name</span></span>       | <span data-ttu-id="fe4e7-134">説明</span><span class="sxs-lookup"><span data-stu-id="fe4e7-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fe4e7-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe4e7-135">Authorization</span></span>  | <span data-ttu-id="fe4e7-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe4e7-138">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fe4e7-138">Workbook-Session-Id</span></span>  | <span data-ttu-id="fe4e7-p107">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-p107">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe4e7-141">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe4e7-141">Request body</span></span>
<span data-ttu-id="fe4e7-142">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-142">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fe4e7-143">パラメーター</span><span class="sxs-lookup"><span data-stu-id="fe4e7-143">Parameter</span></span>    | <span data-ttu-id="fe4e7-144">型</span><span class="sxs-lookup"><span data-stu-id="fe4e7-144">Type</span></span>   |<span data-ttu-id="fe4e7-145">説明</span><span class="sxs-lookup"><span data-stu-id="fe4e7-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe4e7-146">index</span><span class="sxs-lookup"><span data-stu-id="fe4e7-146">index</span></span>|<span data-ttu-id="fe4e7-147">数値</span><span class="sxs-lookup"><span data-stu-id="fe4e7-147">number</span></span>|<span data-ttu-id="fe4e7-p108">省略可能。新しい行の相対位置を指定します。null の場合、最後に追加が行われます。挿入した行の下のすべての行が下方向にシフトします。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-p108">Optional. Specifies the relative position of the new row. If null, the addition happens at the end. Any rows below the inserted row are shifted downwards. Zero-indexed.</span></span>|
|<span data-ttu-id="fe4e7-153">values</span><span class="sxs-lookup"><span data-stu-id="fe4e7-153">values</span></span>|<span data-ttu-id="fe4e7-154">(boolean、string、または number)</span><span class="sxs-lookup"><span data-stu-id="fe4e7-154">(boolean or string or number)</span></span>|<span data-ttu-id="fe4e7-155">テーブルの行の書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-155">A 2-dimensional array of unformatted values of the table rows.</span></span>|

## <a name="response"></a><span data-ttu-id="fe4e7-156">応答</span><span class="sxs-lookup"><span data-stu-id="fe4e7-156">Response</span></span>

<span data-ttu-id="fe4e7-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [TableRow](../resources/tablerow.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-157">If successful, this method returns `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe4e7-158">例</span><span class="sxs-lookup"><span data-stu-id="fe4e7-158">Example</span></span>
<span data-ttu-id="fe4e7-159">この例では、テーブルの末尾に 2 行のデータが挿入されます。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-159">In this example two rows of data are inserted at the end of the table.</span></span> 

##### <a name="request"></a><span data-ttu-id="fe4e7-160">要求</span><span class="sxs-lookup"><span data-stu-id="fe4e7-160">Request</span></span>
<span data-ttu-id="fe4e7-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-161">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerowcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows/add
Content-type: application/json
Content-length: 51

{
  "values": [
    [1, 2, 3],
    [4, 5, 6]
  ]
}
```

##### <a name="response"></a><span data-ttu-id="fe4e7-162">応答</span><span class="sxs-lookup"><span data-stu-id="fe4e7-162">Response</span></span>
<span data-ttu-id="fe4e7-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe4e7-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
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
  "tocPath": ""
}-->