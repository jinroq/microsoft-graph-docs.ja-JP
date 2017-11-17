# <a name="locationconstraintitem-resource-type"></a>locationConstraintItem リソースの種類

会議の場所に関して、クライアントが表明している条件です。

[location](location.md) から派生します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  
  ],
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
| address | [physicalAddress](physicalAddress.md) |場所の番地。 |
| displayName  | String | 場所に関連付けられた名前。                       |
| locationEmailAddress | String | 場所の電子メール アドレス (省略可能)。 |
| resolveAvailability | Boolean | true に設定されているときに指定したリソースがビジー状態である場合は、[findMeetingTimes](../api/user_findmeetingtimes.md) は空いている別のリソースを検索します。false に設定されているときに指定したリソースがビジー状態である場合は、**findMeetingTimes** はリソースが空いているかどうかを確認しないで、ユーザーのキャッシュでトップにランク付けられているリソースを返します。既定値は true です。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->