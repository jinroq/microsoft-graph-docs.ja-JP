# <a name="singlevaluelegacyextendedproperty-resource-type"></a>singleValueLegacyExtendedProperty リソースの種類

単一値が含まれる拡張プロパティ。 

オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Post](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) | サポートされているリソース インスタンス: [メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、または [contactFolder](../resources/contactfolder.md) (ただし、グループ[投稿](../resources/post.md)を除く)。 | サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **singleValueLegacyExtendedProperty** を作成します。 |
|[Get](../api/singlevaluelegacyextendedproperty_get.md) |サポートされているリソースのインスタンス ([メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、[contactFolder](../resources/contactfolder.md)、またはグループ[投稿](../resources/post.md)) のいずれか、またはそれらのコレクション、あるいは [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) オブジェクトで拡張されているインスタンスなどのいずれか。 |`$expand` または `$filter` を使用して拡張プロパティでリソース インスタンスを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|string|プロパティの識別に使用されるプロパティ ID。読み取り専用です。|
|value|string|プロパティ値。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singlevaluelegacyextendedproperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->