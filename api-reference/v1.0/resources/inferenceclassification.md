# <a name="inferenceclassification-resource-type"></a>inferenceClassification リソースの種類

ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。 

詳しくは、「[優先受信トレイを管理する](manage_focused_inbox.md)」を参照してください。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[inferenceClassificationOverride を作成する](../api/inferenceclassification_post_overrides.md) |[inferenceClassificationOverride](inferenceclassificationoverride.md)| SMTP アドレスで示される送信者のオーバーライドを作成します。この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。|
|[オーバーライドを一覧表示する](../api/inferenceclassification_list_overrides.md) |[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション| ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|id|string| 読み取り専用です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|overrides|[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション| ユーザーが、`focused` または `other` の特定の方法で特定の差出人からのメッセージを常時分類するための一連のオーバーライド。読み取り専用です。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->