# <a name="nameditem-resource-type"></a>NamedItem リソースの種類

セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[追加](../api/nameditem_add.md)|[WorkbookNamedItem](nameditem.md)|新しい名前を指定したスコープのコレクションに追加します。|
|[AddFormulaLocal](../api/nameditem_addformulalocal.md)|[WorkbookNamedItem](nameditem.md)|ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。|
|[NamedItem を取得する](../api/nameditem_get.md) | [WorkbookNamedItem](nameditem.md) |namedItem オブジェクトのプロパティと関係を読み取ります。|
|[更新する](../api/nameditem_update.md) | [WorkbookNamedItem](nameditem.md)   |NamedItem オブジェクトを更新します。 |
|[範囲](../api/nameditem_range.md)|[範囲](range.md)|名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。|
|[リスト](../api/nameditem_list.md) | [WorkbookNamedItem](nameditem.md) コレクション |namedItem オブジェクトのコレクションを取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|名前|文字列|オブジェクトの名前。読み取り専用です。|
|コメント|文字列|この名前に関連付けられているコメントを表します。|
|範囲|文字列|名前がブックを対象にしているのか、特定のワークシートを対象にしているのかを示します。読み取り専用です。|
|種類|文字列|名前に関連付けられた参照の種類を示します。 可能な値は、`String`、`Integer`、`Double`、`Boolean`、`Range`です。 読み取り専用。|
|値|Json|定義されている名前が参照する数式を表します。例: =Sheet14!$B$2:$H$12、=4.75, など。読み取り専用です。|
|表示|ブール値|オブジェクトを表示するかどうかを指定します。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ     | 型   |説明|
|:---------------|:--------|:----------|
|ワークシート|[WorkbookWorksheet](worksheet.md)|名前付きのアイテムの対象になるワークシートを返します。アイテムの対象がワークシートの場合にのみ使用できます。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
