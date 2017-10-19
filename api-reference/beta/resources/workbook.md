# <a name="workbook-resource-type"></a>Workbook リソースタイプ

Workbook は、ワークシート、テーブル、範囲などの関連するブック オブジェクトを含む最上位オブジェクトです。

## <a name="properties"></a>プロパティ
なし

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[セッションを作成する](../api/workbook_createsession.md) | [workbookSessionInfo](workbooksessioninfo.md) |永続または非永続セッションを開始するために、ブック セッションを作成します。|
|[セッションを閉じる](../api/workbook_closesession.md) | なし |既存のセッションを終了します。|
|[セッションを最新の情報に更新](../api/workbook_refreshsession.md) | なし |既存のセッションを更新します。|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|names|[NamedItem](nameditem.md) コレクション|ワークブックのスコープにある名前付き項目 (名前付き範囲と名前付き定数) のコレクションを表します。読み取り専用。|
|tables|[Table](table.md) コレクション|ブックに関連付けられているテーブルのコレクションを表します。読み取り専用。|
|worksheets|[Worksheet](worksheet.md) コレクション|ブックに関連付けられているワークシートのコレクションを表します。読み取り専用。|

## <a name="functions"></a>関数

[Excel の関数](#functions):構文 `POST /workbook/functions/{function-name}` を使用し、また JSON オブジェクトを使用して本文の関数の引数を提供することでブック関数を呼び出します。 関数の結果としての `value` および任意の `error` 文字列が、関数の結果のオブジェクトに返されます。 `null` の `error` 値は、関数の実行が成功したことを示します。 

サポートされている関数の完全な一覧は、[こちら](https://support.office.com/en-us/article/Excel-functions-alphabetical-b3944572-255d-4efb-bb96-c6d90033e188) です。 特定のパラメーター名とデータ型については関数のシグネチャを参照してください。

_重要な注意点: _ 
* 範囲入力パラメーターは、範囲のアドレス文字列ではなく、range オブジェクトを使用して提供されます。  
* Index パラメーターは、API のほとんどで使用されている 0 オリジンとは異なり、1 オリジンインデックス (添字が 1 から始まる) です。 

例: 

以下の例では、`vlookup` 関数は検索値、入力範囲、および返される値を渡すことによって呼び出されます。 

要求: 

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

応答:

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

例: 

以下の例では、`median` 関数は配列の入力範囲を渡すことによって呼び出されます。 

要求: 

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

応答:

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
