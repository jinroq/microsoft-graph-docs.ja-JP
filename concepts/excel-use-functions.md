# <a name="use-workbook-functions-in-excel-with-microsoft-graph"></a>Microsoft Graph で Excel のブック関数を使用する

どのブック関数も、`POST /workbook/functions/{function-name}` という構文を使用することにより呼び出すことができます 本文の中で関数の引数は、JSON オブジェクトを使用して指定します。 関数の結果としての `value` および任意の `error` 文字列が、関数の結果のオブジェクトに返されます。 `null` の `error` 値は、関数の実行が成功したことを示します。

サポートする関数の完全な一覧は、[こちら](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188) で確認できます。特定のパラメータ名とデータ型は関数シグネチャを参照してください。

_重要な注意点:_
* 範囲入力パラメーターは、範囲のアドレス文字列ではなく、range オブジェクトを使用して提供されます。  
* Index パラメーターは、API のほとんどで使用されている 0 オリジンとは異なり、1 オリジンのインデックス (添字が 1 から始まる) です。

例: **vlookup**

Excel スプレッドシートで、`vlookup` 関数は次の引数を取ります。

1. **lookup_value** (必須) 検索する値。
2. **table_array** (必須) 参照値を検索するセルの範囲。 参照値が正しく動作するには、常に VLOOKUP の範囲で参照値が最初の列にある必要があることに留意してください。 たとえば、参照値がセル C2 にある場合、範囲は C 列から始まる必要があります。
3. **col_index_num** (必須) 範囲内で、戻り値が入れられる列番号。 たとえば、B2: D11 を範囲として指定すると、B を最初の列、C を 2 番目の列というようにカウントする必要があります。
4. **range_lookup** (オプション) **VLOOKUP** で近似値を検索するのか、それとも完全一致を検索するのかを指定する論理値。 戻り値として近似一致を使用する場合は **TRUE** を指定し、完全一致を必要とする場合は **FALSE** を指定します。 何も指定しない場合、既定値は常に TRUE、つまり近似一致になります。

セル内では、`vlookup` 関数は次のようになります。

=VLOOKUP(<参照値>, <参照値を含む範囲>, <戻り値を含む範囲内の列番号>, <近似一致には TRUE、完全一致には FALSE をオプションで指定>)

([VLOOKUP Excel 関数](https://support.office.com/en-us/article/VLOOKUP-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1)についてのドキュメントを参照してください。)


##### <a name="request"></a>要求:
次の例では、Excel REST API で `vlookup` 関数を呼び出し、これらのパラメーターを渡す方法を示しています。

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

##### <a name="response"></a>応答

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

例: `median`

Excel スプレッドシートでは、`median` 関数は 1 つ以上の入力範囲の配列を取ります。

セル内では、`median` 関数は次の例のようになります。

=MEDIAN(A2:A6)

([MEDIAN Excel 関数](https://support.office.com/en-us/article/MEDIAN-function-d0916313-4753-414c-8537-ce85bdd967d2)についてのドキュメントを参照してください。)

##### <a name="request"></a>要求
次の例では、Excel REST API で `median` 関数と 1 つ以上の入力範囲を呼び出す方法を示しています。

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

##### <a name="response"></a>応答

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

## <a name="see-also"></a>関連項目
* [Microsoft Graph で Excel のセッションを管理する](excel-manage-sessions.md)
* [Microsoft Graph を使用して Excel ブックに書き込む](excel-write-to-workbook.md)
* [Microsoft Graph により Excel のある範囲の書式を更新する](excel-update-range-format.md)
* [Microsoft Graph により Excel のグラフ イメージを表示する](excel-display-chart-image.md)
* [Excel REST API を使用する](../api-reference/v1.0/resources/excel.md)
