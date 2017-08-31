# <a name="itemreference-resource-type"></a>ItemReference リソースの種類

**ItemReference** リソースは、[DriveItem](driveitem.md) を処理するために必要な情報を API を介して提供します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ      | 型                              | 説明                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| driveId       | String                            | アイテムを含むドライブ インスタンスの一意識別子。読み取り専用です。                                 |
| id            | String                            | ドライブ内のアイテムの一意識別子。読み取り専用です。                                                     |
| name          | String                            | 参照中のアイテムの名前。読み取り専用です。                                                          |
| path          | String                            | アイテムへの移動に使用可能なパス。読み取り専用です。                                                  |
| shareId       | String                            | [共有](../api/shares_get.md) API 経由でアクセスできる共有リソースの一意識別子。 |
| sharepointIds | [sharepointIds](sharepointids.md) | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。                                   |

## <a name="remarks"></a>注釈

**itemReference** リソースからの **driveItem** を処理するには、次の形式の URL を構築します。

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

**path** の値は、対象ドライブを基準にした API パスです。例: `/drive/root:/Documents/myfile.docx`。

階層リンクの人が認識できるパスを取得するために、パスの文字列内にある最初の `:` までのすべてを無視しても問題ありません。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
