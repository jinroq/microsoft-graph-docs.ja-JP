---
title: Microsoft Graph で Excel のブック関数を使用する
description: どのブック関数も、`POST /workbook/functions/{function-name}` という構文を使用することにより呼び出すことができます 本文の中で関数の引数は、JSON オブジェクトを使用して指定します。 関数の結果としての `value` および任意の `error` 文字列が、関数の結果のオブジェクトに返されます。 `null` の `error` 値は、関数の実行が成功したことを示します。
ms.openlocfilehash: 36b07277123ccb04de5607a513cee6f576be5550
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092540"
---
# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a><span data-ttu-id="2bcaa-106">Microsoft Graph で Excel のブック関数を使用する</span><span class="sxs-lookup"><span data-stu-id="2bcaa-106">Use workbook functions in Excel with Microsoft Graph</span></span>

<span data-ttu-id="2bcaa-107">どのブック関数も、`POST /workbook/functions/{function-name}` という構文を使用することにより呼び出すことができます</span><span class="sxs-lookup"><span data-stu-id="2bcaa-107">You can invoke any workbook function by using the following syntax: `POST /workbook/functions/{function-name}`.</span></span> <span data-ttu-id="2bcaa-108">本文の中で関数の引数は、JSON オブジェクトを使用して指定します。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-108">You provide the function argument(s) in the body using a JSON object.</span></span> <span data-ttu-id="2bcaa-109">関数の結果としての `value` および任意の `error` 文字列が、関数の結果のオブジェクトに返されます。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-109">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="2bcaa-110">`null` の `error` 値は、関数の実行が成功したことを示します。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-110">The `error` value of `null` indicates successful execution of the function.</span></span>

<span data-ttu-id="2bcaa-p103">サポートされている関数の完全な一覧は、[こちら](https://support.office.com/ja-JP/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188)です。特定のパラメーター名とデータ型については関数のシグネチャを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-p103">The complete list of supported functions are listed [here](https://support.office.com/ja-JP/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188). Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="2bcaa-113">_重要な注意点: _</span><span class="sxs-lookup"><span data-stu-id="2bcaa-113">_Important notes:_</span></span>
* <span data-ttu-id="2bcaa-114">範囲入力パラメーターは、範囲のアドレス文字列ではなく、range オブジェクトを使用して提供されます。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-114">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="2bcaa-115">Index パラメーターは、API のほとんどで使用されている 0 オリジンとは異なり、1 オリジンのインデックス (添字が 1 から始まる) です。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-115">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span>

<span data-ttu-id="2bcaa-116">例: **vlookup**</span><span class="sxs-lookup"><span data-stu-id="2bcaa-116">Example: **vlookup**</span></span>

<span data-ttu-id="2bcaa-117">Excel スプレッドシートで、`vlookup` 関数は次の引数を取ります。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-117">In an Excel spreadsheet, the `vlookup` function takes the following arguments:</span></span>

1. <span data-ttu-id="2bcaa-118">**lookup_value** (必須) 検索する値。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-118">**lookup_value** (required) The value you want to look up.</span></span>
2. <span data-ttu-id="2bcaa-119">**table_array** (必須) 参照値を検索するセルの範囲。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-119">**table_array** (required) The range of cells where the lookup value is located.</span></span> <span data-ttu-id="2bcaa-120">参照値が正しく動作するには、常に VLOOKUP の範囲で参照値が最初の列にある必要があることに留意してください。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-120">Remember that the lookup value should always be in the first column in the range for VLOOKUP to work correctly.</span></span> <span data-ttu-id="2bcaa-121">たとえば、参照値がセル C2 にある場合、範囲は C 列から始まる必要があります。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-121">For example, if your lookup value is in cell C2 then your range should start with C.</span></span>
3. <span data-ttu-id="2bcaa-122">**col_index_num** (必須) 範囲内で、戻り値が入れられる列番号。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-122">**col_index_num** (required) The column number in the range that contains the return value.</span></span> <span data-ttu-id="2bcaa-123">たとえば、B2: D11 を範囲として指定すると、B を最初の列、C を 2 番目の列というようにカウントする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-123">For example, if you specify B2: D11 as the range, you should count B as the first column, C as the second, and so on.</span></span>
4. <span data-ttu-id="2bcaa-124">**range_lookup** (オプション) **VLOOKUP** で近似値を検索するのか、それとも完全一致を検索するのかを指定する論理値。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-124">**range_lookup** (optional) The logical value that specifies whether you want **VLOOKUP** to find an approximate or an exact match.</span></span> <span data-ttu-id="2bcaa-125">戻り値として近似一致を使用する場合は **TRUE** を指定し、完全一致を必要とする場合は **FALSE** を指定します。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-125">Specify **TRUE** if you want an approximate match or **FALSE** if you want an exact match of the return value.</span></span> <span data-ttu-id="2bcaa-126">何も指定しない場合、既定値は常に TRUE、つまり近似一致になります。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-126">If you don't specify anything, the default value will always be TRUE or approximate match.</span></span>

<span data-ttu-id="2bcaa-127">セル内では、`vlookup` 関数は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-127">Inside a cell, the `vlookup` function looks like this:</span></span>

<span data-ttu-id="2bcaa-128">=VLOOKUP(<参照値>, <参照値を含む範囲>, <戻り値を含む範囲内の列番号>, <近似一致には TRUE、完全一致には FALSE をオプションで指定>)</span><span class="sxs-lookup"><span data-stu-id="2bcaa-128">=VLOOKUP(lookup value, range containing the lookup value, the column number in the range containing the return value, optionally specify TRUE for approximate match or FALSE for an exact match)</span></span>

<span data-ttu-id="2bcaa-129">([VLOOKUP Excel 関数](https://support.office.com/ja-JP/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)についてのドキュメントを参照してください。)</span><span class="sxs-lookup"><span data-stu-id="2bcaa-129">(See the documentation for the [VLOOKUP Excel function](https://support.office.com/ja-JP/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1).)</span></span>


##### <a name="request"></a><span data-ttu-id="2bcaa-130">要求:</span><span class="sxs-lookup"><span data-stu-id="2bcaa-130">Request:</span></span>
<span data-ttu-id="2bcaa-131">次の例では、Excel REST API で `vlookup` 関数を呼び出し、これらのパラメーターを渡す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-131">The following example shows how to call the `vlookup` function and pass these parameters with the Excel REST API.</span></span>

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

##### <a name="response"></a><span data-ttu-id="2bcaa-132">応答</span><span class="sxs-lookup"><span data-stu-id="2bcaa-132">Response</span></span>

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

<span data-ttu-id="2bcaa-133">例: `median`</span><span class="sxs-lookup"><span data-stu-id="2bcaa-133">Example: `median`</span></span>

<span data-ttu-id="2bcaa-134">Excel スプレッドシートでは、`median` 関数は 1 つ以上の入力範囲の配列を取ります。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-134">In an Excel spreadsheet, the `median` function takes an array of one or more input ranges.</span></span>

<span data-ttu-id="2bcaa-135">セル内では、`median` 関数は次の例のようになります。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-135">Inside a cell, the `median` function looks like this example:</span></span>

<span data-ttu-id="2bcaa-136">=MEDIAN(A2:A6)</span><span class="sxs-lookup"><span data-stu-id="2bcaa-136">=MEDIAN(A2:A6)</span></span>

<span data-ttu-id="2bcaa-137">([MEDIAN Excel 関数](https://support.office.com/ja-JP/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)についてのドキュメントを参照してください。)</span><span class="sxs-lookup"><span data-stu-id="2bcaa-137">(See the documentation for the [MEDIAN Excel function](https://support.office.com/ja-JP/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2).)</span></span>

##### <a name="request"></a><span data-ttu-id="2bcaa-138">要求</span><span class="sxs-lookup"><span data-stu-id="2bcaa-138">Request</span></span>
<span data-ttu-id="2bcaa-139">次の例では、Excel REST API で `median` 関数と 1 つ以上の入力範囲を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2bcaa-139">The following example shows how to call the `median` function and one or more input ranges with the Excel REST API.</span></span>

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

##### <a name="response"></a><span data-ttu-id="2bcaa-140">応答</span><span class="sxs-lookup"><span data-stu-id="2bcaa-140">Response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="2bcaa-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="2bcaa-141">See also</span></span>
* [<span data-ttu-id="2bcaa-142">Microsoft Graph で Excel のセッションを管理する</span><span class="sxs-lookup"><span data-stu-id="2bcaa-142">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="2bcaa-143">Microsoft Graph を使用して Excel ブックに書き込む</span><span class="sxs-lookup"><span data-stu-id="2bcaa-143">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="2bcaa-144">Microsoft Graph により Excel のある範囲の書式を更新する</span><span class="sxs-lookup"><span data-stu-id="2bcaa-144">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="2bcaa-145">Microsoft Graph により Excel のグラフ イメージを表示する</span><span class="sxs-lookup"><span data-stu-id="2bcaa-145">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="2bcaa-146">Excel REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="2bcaa-146">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
