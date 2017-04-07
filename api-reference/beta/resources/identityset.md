# <a name="identityset-resource-type"></a>IdentitySet リソースの種類

**IdentitySet** リソースは、[ID](identity.md) リソースのキー付きコレクションです。_作成者_または_最終更新者_など、アイテムのさまざまなイベントに関連付けられている ID のセットを表すために使用されます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "user", "device", "application" ],
  "@odata.type": "microsoft.graph.identitySet"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>プロパティ

| プロパティ    | 型                    | 説明                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| application | [Identity](identity.md) | 省略可能。このアクションに関連付けられているアプリケーション。 |
| デバイス      | [Identity](identity.md) | 省略可能。このアクションに関連付けられているデバイス。      |
| ユーザー        | [Identity](identity.md) | 省略可能。このアクションに関連付けられているユーザー。        |

## <a name="remarks"></a>注釈 

**IdentitySet** リソースの使用法については、[DriveItem](driveitem.md) を参照してください。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
