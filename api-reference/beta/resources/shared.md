# <a name="shared-resource-type"></a>Shared リソースタイプ

**Shared** リソースは、DriveItem が他のユーザーと共有されていることを示します。リソースは、項目がどのように共有されているかに関する情報を含んでいます。

[**Driveitem**](driveitem.md) が null でない **shared** ファセットを持つ場合、項目は共有されています。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "scope": "public | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>プロパティ

| プロパティ       | 型                          | 説明                                                                                        |
| :------------- | :---------------------------- | :------------------------------------------------------------------------------------------------- |
| owner          | [IdentitySet](identityset.md) | 共有項目の所有者の ID。読み取り専用。                                           |
| scope          | 文字列                        | `anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。 読み取り専用です。 |
| sharedBy       | [identitySet](identityset.md) | 項目を共有するユーザーの ID。読み取り専用です。                                           |
| sharedDateTime | DateTimeOffset                | 項目が共有された UTC 日時。読み取り専用です。                                         |

## <a name="scope-values"></a>スコープの値

| 値        | 説明                                                                           |
|:-------------|:--------------------------------------------------------------------------------------|
| public       | 項目は、リンクを持つすべてのユーザーに対して機能するリンクを使用して共有されます。               |
| organization | 項目は、所有者の組織内にいるすべてのユーザーに対して機能するリンクを使用して共有されます。 |
| users        | 項目は、特定のユーザーのみと共有されます。                                          |

## <a name="remarks"></a>備考

**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shared resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
