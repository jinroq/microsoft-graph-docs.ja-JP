# <a name="inferenceclassificationoverride-resource-type"></a>inferenceClassificationOverride リソースの種類

特定の差出人からの着信メッセージを常時分類するためのユーザーのオーバーライドを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[更新する](../api/inferenceclassificationoverride_update.md) | [inferenceClassificationOverride](inferenceclassificationoverride.md) |指定のとおり、オーバーライドの **ClassifyAs** フィールドを変更します。 |
|[削除](../api/inferenceclassificationoverride_delete.md) | なし |その ID で指定されたオーバーライドを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|classifyAs|InferenceClassificationType| 特定の差出人からの着信メッセージを常時分類する方法を指定します。 可能な値は、`focused`、`other` です。|
|ID|文字列| オーバーライドの一意識別子。読み取り専用です。|
|senderEmailAddress|[emailAddress](emailaddress.md)|オーバーライドを作成する対象の差出人のメール アドレス情報。|

## <a name="relationships"></a>関係
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->