---
title: Workbook リソースタイプ
description: Workbook は、ワークシート、テーブル、範囲などの関連するブック オブジェクトを含む最上位オブジェクトです。
localization_priority: Priority
ms.openlocfilehash: 25b74bcc0ce0b54aace11ed9f829435a510f9c9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835421"
---
# <a name="workbook-resource-type"></a><span data-ttu-id="117cd-103">Workbook リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="117cd-103">Workbook resource type</span></span>

<span data-ttu-id="117cd-104">Workbook は、ワークシート、テーブル、範囲などの関連するブック オブジェクトを含む最上位オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="117cd-104">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="json-representation"></a><span data-ttu-id="117cd-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="117cd-105">JSON representation</span></span>

<span data-ttu-id="117cd-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="117cd-106">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbook"
}-->

```json
{
  "names": [{"@odata.type": "microsoft.graph.workbookNamedItem"}],
  "tables": [{"@odata.type": "microsoft.graph.workbookTable"}],
  "worksheets": [{"@odata.type": "microsoft.graph.workbookWorksheet"}]
}
```

## <a name="properties"></a><span data-ttu-id="117cd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="117cd-107">Properties</span></span>
<span data-ttu-id="117cd-108">なし</span><span class="sxs-lookup"><span data-stu-id="117cd-108">None</span></span>

## <a name="methods"></a><span data-ttu-id="117cd-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="117cd-109">Methods</span></span>

| <span data-ttu-id="117cd-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="117cd-110">Method</span></span>       | <span data-ttu-id="117cd-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="117cd-111">Return Type</span></span>  |<span data-ttu-id="117cd-112">説明</span><span class="sxs-lookup"><span data-stu-id="117cd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="117cd-113">セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="117cd-113">Create Session</span></span>](../api/workbook-createsession.md) | [<span data-ttu-id="117cd-114">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="117cd-114">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="117cd-115">永続または非永続セッションを開始するために、ブック セッションを作成します。</span><span class="sxs-lookup"><span data-stu-id="117cd-115">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="117cd-116">セッションを閉じる</span><span class="sxs-lookup"><span data-stu-id="117cd-116">Close Session</span></span>](../api/workbook-closesession.md) | <span data-ttu-id="117cd-117">なし</span><span class="sxs-lookup"><span data-stu-id="117cd-117">None</span></span> |<span data-ttu-id="117cd-118">既存のセッションを終了します。</span><span class="sxs-lookup"><span data-stu-id="117cd-118">Close an existing session.</span></span>|
|[<span data-ttu-id="117cd-119">セッションを最新の情報に更新</span><span class="sxs-lookup"><span data-stu-id="117cd-119">Refresh Session</span></span>](../api/workbook-refreshsession.md) | <span data-ttu-id="117cd-120">なし</span><span class="sxs-lookup"><span data-stu-id="117cd-120">None</span></span> |<span data-ttu-id="117cd-121">既存のセッションを更新します。</span><span class="sxs-lookup"><span data-stu-id="117cd-121">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="117cd-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="117cd-122">Relationships</span></span>
| <span data-ttu-id="117cd-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="117cd-123">Relationship</span></span> | <span data-ttu-id="117cd-124">型</span><span class="sxs-lookup"><span data-stu-id="117cd-124">Type</span></span>   |<span data-ttu-id="117cd-125">説明</span><span class="sxs-lookup"><span data-stu-id="117cd-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="117cd-126">names</span><span class="sxs-lookup"><span data-stu-id="117cd-126">names</span></span>|<span data-ttu-id="117cd-127">[WorkbookNamedItem](nameditem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="117cd-127">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="117cd-p101">ブック スコープの名前付き項目 (名前付き範囲と名前付き定数) のコレクションを表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="117cd-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="117cd-130">テーブル</span><span class="sxs-lookup"><span data-stu-id="117cd-130">tables</span></span>|<span data-ttu-id="117cd-131">[WorkbookTable](table.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="117cd-131">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="117cd-p102">ブックに関連付けられているテーブルのコレクションを表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="117cd-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="117cd-134">worksheets</span><span class="sxs-lookup"><span data-stu-id="117cd-134">worksheets</span></span>|<span data-ttu-id="117cd-135">[WorkbookWorksheet](worksheet.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="117cd-135">[WorkbookWorksheet](worksheet.md) collection</span></span>|<span data-ttu-id="117cd-p103">ブックに関連付けられているワークシートのコレクションを表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="117cd-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="117cd-138">関数</span><span class="sxs-lookup"><span data-stu-id="117cd-138">Functions</span></span>

<span data-ttu-id="117cd-p104">[Excel の関数](#functions):構文 `POST /workbook/functions/{function-name}` を使用し、また JSON オブジェクトを使用して本文の関数の引数を提供することでブック関数を呼び出します。関数の結果としての `value` および任意の `error` 文字列が、関数の結果のオブジェクトに返されます。`null` の `error` 値は、関数の実行が成功したことを示します。</span><span class="sxs-lookup"><span data-stu-id="117cd-p104">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting `value` and any `error` strings are returned in the function result object. The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="117cd-p105">サポートされている関数の完全な一覧は、[こちら](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)です。特定のパラメーター名とデータ型については関数のシグネチャを参照してください。</span><span class="sxs-lookup"><span data-stu-id="117cd-p105">The complete list of supported functions are listed [here](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="117cd-144">_重要な注意点: _</span><span class="sxs-lookup"><span data-stu-id="117cd-144">_Important notes:_</span></span> 
* <span data-ttu-id="117cd-145">範囲入力パラメーターは、範囲のアドレス文字列ではなく、range オブジェクトを使用して提供されます。</span><span class="sxs-lookup"><span data-stu-id="117cd-145">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="117cd-146">Index パラメーターは、API のほとんどで使用されている 0 オリジンとは異なり、1 オリジンのインデックス (添字が 1 から始まる) です。</span><span class="sxs-lookup"><span data-stu-id="117cd-146">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="117cd-147">例: **vlookup**</span><span class="sxs-lookup"><span data-stu-id="117cd-147">Example: **vlookup**</span></span>

<span data-ttu-id="117cd-148">Excel スプレッドシートで、`vlookup` 関数は次の引数を取ります。</span><span class="sxs-lookup"><span data-stu-id="117cd-148">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="117cd-149">参照値とも呼ばれる、検索対象の値。</span><span class="sxs-lookup"><span data-stu-id="117cd-149">The value you want to look up, also called the lookup value.</span></span>
2. <span data-ttu-id="117cd-150">参照値が所在する範囲。</span><span class="sxs-lookup"><span data-stu-id="117cd-150">The range where the lookup value is located.</span></span> <span data-ttu-id="117cd-151">参照値が正しく動作するには、常に VLOOKUP の範囲で参照値が最初の列にある必要があることに留意してください。</span><span class="sxs-lookup"><span data-stu-id="117cd-151">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="117cd-152">たとえば、参照値がセル C2 にある場合、範囲は C 列から始まる必要があります。</span><span class="sxs-lookup"><span data-stu-id="117cd-152">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="117cd-153">戻り値を含む範囲の列番号。</span><span class="sxs-lookup"><span data-stu-id="117cd-153">The column number in the range that contains the return value.</span></span> <span data-ttu-id="117cd-154">たとえば、B2: D11 を範囲として指定すると、B を最初の列、C を 2 番目の列というようにカウントする必要があります。</span><span class="sxs-lookup"><span data-stu-id="117cd-154">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="117cd-155">また、戻り値の近似一致を使用する場合は TRUE を指定し、完全一致を必要とする場合は FALSE を指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="117cd-155">Optionally, you can specify TRUE if you want an approximate match or FALSE if you want an exact match of the return value.</span></span> <span data-ttu-id="117cd-156">何も指定しない場合、既定値は常に TRUE、つまり近似一致になります。</span><span class="sxs-lookup"><span data-stu-id="117cd-156">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="117cd-157">セル内では、`vlookup` 関数は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="117cd-157">Inside a cell, the `vlookup` function looks like this:</span></span> 

<span data-ttu-id="117cd-158">=VLOOKUP(<参照値>, <参照値を含む範囲>, <戻り値を含む範囲内の列番号>, <近似一致には TRUE、完全一致には FALSE をオプションで指定>)</span><span class="sxs-lookup"><span data-stu-id="117cd-158">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="117cd-159">([VLOOKUP Excel 関数](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)についてのドキュメントを参照してください。)</span><span class="sxs-lookup"><span data-stu-id="117cd-159">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>

<span data-ttu-id="117cd-160">次の例では、Excel REST API で `vlookup` 関数を呼び出し、これらのパラメーターを渡す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="117cd-160">The example below shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

<span data-ttu-id="117cd-161">要求:</span><span class="sxs-lookup"><span data-stu-id="117cd-161">Request:</span></span> 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/vlookup
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "lookupValue": "Temperature",
    "tableArray": { "Address": "Sheet1!E1:G5" },
    "colIndexNum": 2,
    "rangeLookup": false
}
```

<span data-ttu-id="117cd-162">応答:</span><span class="sxs-lookup"><span data-stu-id="117cd-162">Response:</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="117cd-163">例: `median`</span><span class="sxs-lookup"><span data-stu-id="117cd-163">Example: `median`</span></span>

<span data-ttu-id="117cd-164">Excel スプレッドシートでは、`median` 関数は 1 つ以上の入力範囲の配列を取ります。</span><span class="sxs-lookup"><span data-stu-id="117cd-164">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="117cd-165">セル内では、`median` 関数は次の例のようになります。</span><span class="sxs-lookup"><span data-stu-id="117cd-165">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="117cd-166">=MEDIAN(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="117cd-166">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="117cd-167">([MEDIAN Excel 関数](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)についてのドキュメントを参照してください。)</span><span class="sxs-lookup"><span data-stu-id="117cd-167">(See the documentation for the [MEDIAN Excel function](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

<span data-ttu-id="117cd-168">次の例では、Excel REST API で `median` 関数と 1 つ以上の入力範囲を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="117cd-168">The example below shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span> 

<span data-ttu-id="117cd-169">要求:</span><span class="sxs-lookup"><span data-stu-id="117cd-169">Request:</span></span> 

```http 
POST https://graph.microsoft.com/beta/me/drive/root:/book1.xlsx:/workbook/functions/median
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"values" :  [
        { "address": "Sheet2!A1:A5" },
        { "address": "Sheet2!B1:B5" },
      ] 
}
```

<span data-ttu-id="117cd-170">応答:</span><span class="sxs-lookup"><span data-stu-id="117cd-170">Response:</span></span>

```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "@odata.id": "/users('2abcad6a-2fca-4b6e-9577-e358a757d77d')/drive/root/workbook/functions/median()",
  "error": null,
  "value": 30
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Workbook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
