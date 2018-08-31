# <a name="recentnotebook-resource-type"></a>recentNotebook リソース型

最近アクセスした OneNote ノートブック。 **recentNotebook** は、[notebook](notebook.md) と類似していますが、より少ないプロパティを持ちます。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|displayName|文字列|ノートブックの名前。|
|lastAccessedTime|DateTimeOffset|ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|
|リンク|[recentNotebookLinks](recentnotebooklinks.md)|ノートブックを開くためのリンク。 リンクは、OneNote クライアントでノートブックを開きます (インストールされている場合)。`oneNoteClientURL` リンクは、OneNote Online でノートブックを開きます。`oneNoteWebURL`|
|sourceService|onenoteSourceService|ノートブックが存在するバックエンド ストア (`OneDriveForBusiness` または `OneDrive` のいずれか)。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}
```

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[getRecentNotebooks](../api/notebook_getrecentnotebooks.md) | [ノートブック](notebook.md) コレクション | ユーザーの最近アクセスしたノートブックのコレクションを取得します。 |
