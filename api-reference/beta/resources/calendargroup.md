# <a name="calendargroup-resource-type"></a>calendarGroup リソースの種類

予定表のグループです。

**注**： Outlook.com によってサポートされるのは、../me/calendars ショートカットでアクセス可能な既定の予定表グループのみです。その予定表グループを削除することはできません。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[予定表グループを一覧表示する](../api/user_list_calendargroups.md) |[Calendar](calendar.md) collection| ユーザーの予定表グループを取得します。|
|[予定表グループを作成する](../api/user_post_calendargroups.md) |[Calendar](calendar.md)| 新しい予定表グループを作成します。|
|[予定表グループを取得する](../api/calendargroup_get.md) | [calendarGroup](calendargroup.md) |予定表グループ オブジェクトのプロパティと関係を読み取ります。|
|[Update](../api/calendargroup_update.md) | [calendarGroup](calendargroup.md) |calendarGroup オブジェクトを更新します。 |
|[Delete](../api/calendargroup_delete.md) | なし |calendarGroup オブジェクトを削除します。 |
|[予定表を一覧表示する](../api/calendargroup_list_calendars.md) |[Calendar](calendar.md) collection| 予定表グループ内の予定表を一覧表示する|
|[予定表を作成する](../api/calendargroup_post_calendars.md) |[Calendar](calendar.md)| 予定表グループに新しい予定表を作成します。|


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|name|String|グループの名前。|
|changeKey|String|予定表グループのバージョンを識別します。予定表グループを変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用です。|
|classId|Guid|クラス識別子。読み取り専用です。|
|id|String|グループの一意識別子。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|予定表|[Calendar](calendar.md) collection|予定表グループ内の予定表。ナビゲーション プロパティ。読み取り専用です。Null 許容型。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
