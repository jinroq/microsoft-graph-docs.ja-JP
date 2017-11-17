# <a name="patchcontentcommand-resource-type"></a>patchContentCommand リソースの種類

PATCH 要求で OneNote ページに加える変更。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。[PATCH pages/{id}`](../api/page_update.md) 要求の本文に送信されます。 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|action|String|ターゲット要素で実行するアクション。使用可能な値: `replace`、`append`、`delete`、`insert`、`prepend`。|
|content|String|ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります。 |
|position|String|指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。使用可能な値: `after` (既定値) または `before`。|
|target|String|更新する要素。要素の `#<data-id>` または生成された `<id>`、または `body` か `title` のキーワードでなければなりません。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->