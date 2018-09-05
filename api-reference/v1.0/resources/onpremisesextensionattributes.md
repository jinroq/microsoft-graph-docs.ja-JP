# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes リソースの種類

 [user](user.md) エンティティの **onPremisesExtensionAttributes** プロパティは、15 個のカスタム拡張機能の属性のプロパティを含みます。 **onPremisesSyncEnabled** のユーザーでは、このプロパティのセットは内部設置型の Active Directory をマスタとし、Azure AD に同期され、読み取り専用となります。 クラウドのみのユーザー (**onPremisesSyncEnabled** が falseの場合) では、これらのプロパティは作成時または更新時に設定されることがあります。


## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|extensionAttribute1|String| 最初のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute2|String| 2 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute3|String| 3 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute4|String| 4 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute5|String| 5 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute6|String| 6 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute7|String| 7 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute8|String| 8 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute9|String| 9 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute10|String| 10 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute11|String| 11 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute12|String| 12 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute13|String| 13 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute14|String| 14 番目のカスタマイズ可能な拡張機能の属性です。 |
|extensionAttribute15|String| 15 番目のカスタマイズ可能な拡張機能の属性です。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->