# <a name="shareddriveitem-resource-type"></a>SharedDriveItem リソースの種類

**sharedDriveItem** リソースは、[Shares](../api/shares_get.md) API を使用して共有 [driveItem](driveitem.md) にアクセスする場合に返されます。

## <a name="json-representation"></a>JSON 表記

以下は、**sharedDriveItem** リソースの JSON 表記です。

**sharedDriveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。

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

    /* relationships*/
    "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
    "root": { "@odata.type": "microsoft.graph.driveItem" },
    "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
    "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型                          | 説明                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | String                        | アクセスされている共有の一意識別子。              |
| name     | String                        | 共有項目の表示名。                             |
| owner    | [IdentitySet](identityset.md) | 参照されている共有アイテムの所有者に関する情報。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型                                  | 説明                                                                                                                                                                                                |
| :----------- | :------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| items        | Collection([DriveItem](driveitem.md)) | 共有 **driveItem** リソースのコレクション。このコレクションは列挙することはできませんが、アイテムには固有の ID でアクセスできます。                                                                        |
| root         | [DriveItem](driveitem.md)             | 最上位の共有 **driveItem**。単一のファイルが共有されている場合、このアイテムがファイルになります。フォルダーが共有されている場合は、この項目はフォルダーになります。アイテムのファセットを使用して、どちらのケースが適用されるか判断します。 |
| driveItem    | [driveItem](driveitem.md)             | 共有されたリソースの **driveItem**。これは、**root** プロパティと一致します。                                                                                                             |
| site         | [site](site.md)                       | 共有されたアイテムを含む **サイト** リソース。                                                                                                                                                |

## <a name="methods"></a>メソッド

| Method                                  | REST パス                |
| :-------------------------------------- | :----------------------- |
| [共有アイテムを取得する](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>備考

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