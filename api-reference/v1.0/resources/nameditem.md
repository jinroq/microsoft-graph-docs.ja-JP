# <a name="nameditem-resource-type"></a>NamedItem リソースの種類

セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[NamedItem を取得する](../api/nameditem_get.md) | [NamedItem](nameditem.md) |namedItem オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/nameditem_update.md) | [NamedItem](nameditem.md)    |NamedItem オブジェクトを更新します。 |
|[Range](../api/nameditem_range.md)|[Range](range.md)|名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。|
|[List](../api/nameditem_list.md) | [NamedItem](nameditem.md) コレクション |namedItem オブジェクトのコレクションを取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|name|string|オブジェクトの名前。値の取得のみ可能です。|
|type|string|名前に関連付けられている参照の型を示します。可能な値は、`String`、`Integer`、`Double`、`Boolean`、`Range` です。読み取り専用です。|
|value|オブジェクト|定義されている名前が参照する数式を表します。例: =Sheet14!$B$2:$H$12、=4.75, など。読み取り専用です。|
|visible|boolean|オブジェクトを表示するかどうかを指定します。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.range"},
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