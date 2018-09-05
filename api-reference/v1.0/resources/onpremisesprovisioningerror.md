# <a name="onpremisesprovisioningerror-resource-type"></a>onPremisesProvisioningError リソースの種類

内部設置型ディレクトリを Azure Active Directory に同期するときの[ユーザー](user.md)と[グループ](group.md)のエンティティのディレクトリ同期エラーを表します。

## <a name="properties"></a>プロパティ

| プロパティ | タイプ | 説明 |
|:---------------|:--------|:----------|
|category|文字列| 事前設定時のエラーのカテゴリです。 注意: 現時点で使用可能な値は 1 つだけです。 使用可能な値: *PropertyConflict* - プロパティの値が一意でないことを示します。 他のオブジェクトには、プロパティの同じ値が含まれます。 |
|occurredDateTime|DateTimeOffset| エラーが発生した日時。 |
|propertyCausingError|文字列| エラーの原因となっているディレクトリのプロパティの名前。 現在使用可能な値: *UserPrincipalName* または *ProxyAddress* |
|value|文字列| エラーの原因となっているプロパティの値です。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->