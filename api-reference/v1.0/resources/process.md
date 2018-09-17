# <a name="process-resource-type"></a>プロセス リソースの種類

ステートフルなアラートに関連するプロセスについてを説明します。

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|accountName|文字列|ユーザーは、例、アカウント名、SID、およびように識別子 (ユーザー アカウントのコンテキストでプロセスが実行された) を考慮します。|
|commandLine|文字列|完全な処理の呼び出しは、すべてのパラメーターを含むを使用できます。|
|createdDateTime|DateTimeOffset|プロセスが開始された時刻です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表示し、常に UTC 時間です。 例えば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります：`'2014-01-01T00:00:00Z'` 。|
|fileHash|[fileHash](filehash.md)|複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。|
|integrityLevel|processIntegrityLevel|プロセスの整合性レベルです。 可能な値は、`unknown`、`untrusted`、`low`、`medium`、`high`、`system` です。|
|isElevated|ブール値|プロセスが昇格した場合はTrueです。|
|名前|文字列|プロセスの画像ファイル名です。|
|parentProcessCreatedDateTime|DateTimeOffset|親プロセスの開始日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表示し、常に UTC 時間です。 例えば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります：`'2014-01-01T00:00:00Z'` 。|
|parentProcessId|Int32| 親プロセスのプロセス ID (PID)です。|
|parentProcessName|文字列|親プロセスの画像ファイル名です。|
|パス|文字列|ファイル名を含む完全パスです。|
|processId|Int32|プロセスのプロセス ID (PID)です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->