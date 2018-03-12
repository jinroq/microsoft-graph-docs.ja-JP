# <a name="location-resource-type"></a>場所リソースの種類

イベントの場所の情報を表します。


## <a name="properties"></a>プロパティ
| プロパティ  | 型   | 説明                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| address | [physicalAddress](physicaladdress.md) |場所の番地。 |
| displayName  | String | 場所に関連付けられた名前。                       |
| locationEmailAddress | String | 場所の電子メール アドレス (省略可能)。              |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.location"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```

## <a name="remarks"></a>注釈

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "location resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
