# <a name="shareddriveitem-resource-type"></a>SharedDriveItem リソースタイプ

**SharedDriveItem** リソースは、[Shares](../api/shares_get.md) API を使用して共有 [DriveItem](driveitem.md) にアクセスする場合に返されます。このリソースは、[Drive](drive.md) リソースに似ていますが、共有リンクまたは shareId でアクセス可能な DriveItems のみを対象としています。

### <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->
```json
{
    "id": "string",
    "name": "string",
    "owner": { "@odata.type": "microsoft.graph.identitySet" },
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" }
}
```

### <a name="properties"></a>プロパティ

| プロパティ  | 型                                  | 説明                                                          |
|:----------|:--------------------------------------|:---------------------------------------------------------------------|
| id        | String                                | アクセスされている共有の一意識別子。                  |
| name      | String                                | 共有項目の表示名。                                 |
| owner     | [IdentitySet](identityset.md)         | 参照されている共有項目の所有者に関する情報です。     |
| items     | Collection([DriveItem](driveitem.md)) | 共有 DriveItem リソースのコレクションです。このコレクションは列挙することはできませんが、項目には固有の ID でアクセスできます。 |
| root      | [DriveItem](driveitem.md)             | 最上位の共有 DriveItem です。単一のファイルが共有されている場合、この項目がファイルになります。フォルダーが共有されている場合は、この項目はフォルダーになります。項目のファセットを使用して、どちらのケースが適用されるか判断します。 |

## <a name="remarks"></a>注釈 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharepointIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->