# <a name="sharepointids-resource-type"></a>SharePointIds リソースの種類

**SharePointIds** リソースは、SharePoint サイトまたは OneDrive for Business に保存されているアイテムのさまざまな識別子を 1 つの構造にグループ化します。

**注:** 個人用の OneDrive から返されたアイテムには **SharePointIds** ファセットは含まれません。

### <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->
```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "webId": "string"
}
```

### <a name="properties"></a>プロパティ

| プロパティ          | 型    | 説明                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| listId            | string  | SharePoint 内にあるアイテムの一覧の一意識別子。                          |
| listItemId        | string  | 含まれているリスト内にあるアイテムの整数の識別子。                    |
| listItemUniqueId  | string  | OneDrive for Busienss または SharePoint サイト内にあるアイテムの一意識別子。 |
| siteId            | string  | アイテムのサイト コレクションの一意識別子。 |
| webId             | string  | アイテムのサイトの一意識別子。                          |

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
