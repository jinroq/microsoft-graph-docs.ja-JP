# <a name="workbook-resource-type"></a><span data-ttu-id="537dd-101">Workbook リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="537dd-101">Workbook resource type</span></span>

<span data-ttu-id="537dd-102">Workbook は、ワークシート、テーブル、範囲などの関連するブック オブジェクトを含む最上位オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="537dd-102">Workbook is the top level object which contains related workbook objects such as worksheets, tables, ranges, etc.</span></span>

## <a name="properties"></a><span data-ttu-id="537dd-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="537dd-103">Properties</span></span>
<span data-ttu-id="537dd-104">なし</span><span class="sxs-lookup"><span data-stu-id="537dd-104">None</span></span>

## <a name="methods"></a><span data-ttu-id="537dd-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="537dd-105">Methods</span></span>

| <span data-ttu-id="537dd-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="537dd-106">Method</span></span>       | <span data-ttu-id="537dd-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="537dd-107">Return Type</span></span>  |<span data-ttu-id="537dd-108">説明</span><span class="sxs-lookup"><span data-stu-id="537dd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="537dd-109">セッションを作成する</span><span class="sxs-lookup"><span data-stu-id="537dd-109">Create Upload Session</span></span>](../api/workbook_createsession.md) | [<span data-ttu-id="537dd-110">workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="537dd-110">workbookSessionInfo</span></span>](workbooksessioninfo.md) |<span data-ttu-id="537dd-111">永続または非永続セッションを開始するために、ブック セッションを作成します。</span><span class="sxs-lookup"><span data-stu-id="537dd-111">Create a workbook session to start a persistent or non-persistent session.</span></span>|
|[<span data-ttu-id="537dd-112">セッションを閉じる</span><span class="sxs-lookup"><span data-stu-id="537dd-112">Close Session</span></span>](../api/workbook_closesession.md) | <span data-ttu-id="537dd-113">なし</span><span class="sxs-lookup"><span data-stu-id="537dd-113">None</span></span> |<span data-ttu-id="537dd-114">既存のセッションを終了します。</span><span class="sxs-lookup"><span data-stu-id="537dd-114">Close an existing session.</span></span>|
|[<span data-ttu-id="537dd-115">セッションを最新の情報に更新</span><span class="sxs-lookup"><span data-stu-id="537dd-115">Refresh Session</span></span>](../api/workbook_refreshsession.md) | <span data-ttu-id="537dd-116">なし</span><span class="sxs-lookup"><span data-stu-id="537dd-116">None</span></span> |<span data-ttu-id="537dd-117">既存のセッションを更新します。</span><span class="sxs-lookup"><span data-stu-id="537dd-117">Refresh an existing session.</span></span>|


## <a name="relationships"></a><span data-ttu-id="537dd-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="537dd-118">Relationships</span></span>
| <span data-ttu-id="537dd-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="537dd-119">Relationship</span></span> | <span data-ttu-id="537dd-120">型</span><span class="sxs-lookup"><span data-stu-id="537dd-120">Type</span></span>   |<span data-ttu-id="537dd-121">説明</span><span class="sxs-lookup"><span data-stu-id="537dd-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="537dd-122">names</span><span class="sxs-lookup"><span data-stu-id="537dd-122">names</span></span>|<span data-ttu-id="537dd-123">[NamedItem](nameditem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="537dd-123">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="537dd-p101">ワークブックのスコープにある名前付き項目 (名前付き範囲と名前付き定数) のコレクションを表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="537dd-p101">Represents a collection of workbook scoped named items (named ranges and constants). Read-only.</span></span>|
|<span data-ttu-id="537dd-126">tables</span><span class="sxs-lookup"><span data-stu-id="537dd-126">tables</span></span>|<span data-ttu-id="537dd-127">[Table](table.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="537dd-127">[Table](table.md) collection</span></span>|<span data-ttu-id="537dd-p102">ブックに関連付けられているテーブルのコレクションを表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="537dd-p102">Represents a collection of tables associated with the workbook. Read-only.</span></span>|
|<span data-ttu-id="537dd-130">worksheets</span><span class="sxs-lookup"><span data-stu-id="537dd-130">worksheets</span></span>|<span data-ttu-id="537dd-131">[Worksheet](worksheet.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="537dd-131">[Worksheet](worksheet.md) collection</span></span>|<span data-ttu-id="537dd-p103">ブックに関連付けられているワークシートのコレクションを表します。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="537dd-p103">Represents a collection of worksheets associated with the workbook. Read-only.</span></span>|

## <a name="functions"></a><span data-ttu-id="537dd-134">関数</span><span class="sxs-lookup"><span data-stu-id="537dd-134">Functions</span></span>

<span data-ttu-id="537dd-135">[Excel の関数](#functions):構文 `POST /workbook/functions/{function-name}` を使用し、また JSON オブジェクトを使用して本文の関数の引数を提供することでブック関数を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="537dd-135">[Excel functions](#functions): Invoke a workbook function using the syntax `POST /workbook/functions/{function-name}` and providing the function argument(s) in the body using a JSON object. The function's resulting  and any  strings are returned in the function result object. The  value of  indicates successful execution of the function.</span></span> <span data-ttu-id="537dd-136">関数の結果としての `value` および任意の `error` 文字列が、関数の結果のオブジェクトに返されます。</span><span class="sxs-lookup"><span data-stu-id="537dd-136">The function's resulting `value` and any `error` strings are returned in the function result object.</span></span> <span data-ttu-id="537dd-137">`null` の `error` 値は、関数の実行が成功したことを示します。</span><span class="sxs-lookup"><span data-stu-id="537dd-137">The `error` value of `null` indicates successful execution of the function.</span></span> 

<span data-ttu-id="537dd-138">サポートされている関数の完全な一覧は、[こちら](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188) です。</span><span class="sxs-lookup"><span data-stu-id="537dd-138">The complete list of supported functions are listed here. Refer to the function signature for specific parameter names and data types.</span></span> <span data-ttu-id="537dd-139">特定のパラメーター名とデータ型については関数のシグネチャを参照してください。</span><span class="sxs-lookup"><span data-stu-id="537dd-139">The complete list of supported functions are listed here. Refer to the function signature for specific parameter names and data types.</span></span>

<span data-ttu-id="537dd-140">_重要な注意点: _</span><span class="sxs-lookup"><span data-stu-id="537dd-140">_Important notes:_</span></span> 
* <span data-ttu-id="537dd-141">範囲入力パラメーターは、範囲のアドレス文字列ではなく、range オブジェクトを使用して提供されます。</span><span class="sxs-lookup"><span data-stu-id="537dd-141">The range input parameter is supplied using a range object instead of the range address string.</span></span>  
* <span data-ttu-id="537dd-142">Index パラメーターは、API のほとんどで使用されている 0 オリジンとは異なり、1 オリジンインデックス (添字が 1 から始まる) です。</span><span class="sxs-lookup"><span data-stu-id="537dd-142">The index parameter is 1-indexed unlike the 0-index used in most of the APIs.</span></span> 

<span data-ttu-id="537dd-143">例:</span><span class="sxs-lookup"><span data-stu-id="537dd-143">Example:</span></span> 

<span data-ttu-id="537dd-144">以下の例では、`vlookup` 関数は検索値、入力範囲、および返される値を渡すことによって呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="537dd-144">In the below example, `vlookup` function is called by passing lookup value, input range and the value to be returned.</span></span> 

<span data-ttu-id="537dd-145">要求:</span><span class="sxs-lookup"><span data-stu-id="537dd-145">Request:</span></span> 

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

<span data-ttu-id="537dd-146">応答:</span><span class="sxs-lookup"><span data-stu-id="537dd-146">Response:</span></span>

```http
HTTP code: 200, OK
content-type: application/json;odata.metadata 

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/vlookup()",
    "error": null,
    "value": "28.3"
}
```

<span data-ttu-id="537dd-147">例:</span><span class="sxs-lookup"><span data-stu-id="537dd-147">Example:</span></span> 

<span data-ttu-id="537dd-148">以下の例では、`median` 関数は配列の入力範囲を渡すことによって呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="537dd-148">In the below example, `median` function is called by passing the input range(s) in an array.</span></span> 

<span data-ttu-id="537dd-149">要求:</span><span class="sxs-lookup"><span data-stu-id="537dd-149">Request:</span></span> 

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

<span data-ttu-id="537dd-150">応答:</span><span class="sxs-lookup"><span data-stu-id="537dd-150">Response:</span></span>

```http
HTTP code: 200, OK
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
