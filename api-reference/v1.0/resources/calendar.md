# <a name="calendar-resource-type"></a>calendar リソース型

イベントのコンテナーである予定表です。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[予定表を一覧表示する](../api/user_list_calendars.md)|[calendar](calendar.md) collection|ユーザーのすべての予定表を取得するか、既定またはその他の特定の予定表グループの予定表を取得します。|
|[予定表を作成する](../api/user_post_calendars.md) |[calendar](calendar.md)| 既定の予定表グループまたは特定の予定表グループに予定表を作成します。|
|[予定表を取得する](../api/calendar_get.md) | [calendar](calendar.md) |予定表オブジェクトのプロパティとリレーションシップを読み取ります。|
|[更新する](../api/calendar_update.md) | [calendar](calendar.md)  |予定表オブジェクトを更新します。 |
|[削除](../api/calendar_delete.md) | なし |予定表オブジェクトを削除します。 |
|[calendarView を一覧表示する](../api/calendar_list_calendarview.md) |[Event](event.md) collection| ユーザーの標準として設定されている予定表 `(../me/calendarview)` または特定の予定表から、時間範囲で定義したカレンダー ビューのイベントの発生、例外、および単一インスタンスを取得します。|
|[イベントを一覧表示する](../api/calendar_list_events.md) |[Event](event.md) collection| 予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[イベントを作成する](../api/calendar_post_events.md) |[Event](event.md)| 既定または指定の予定表に新しいイベントを作成します。|
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[calendar](calendar.md)  |新規または既存の予定表に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ予定表を取得する](../api/singlevaluelegacyextendedproperty_get.md)  | [calendar](calendar.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む予定表を取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [calendar](calendar.md) | 新規または既存の予定表に、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ予定表を取得する](../api/multivaluelegacyextendedproperty_get.md)  | [calendar](calendar.md) | `$expand` を使用して、複数値の拡張プロパティを含む予定表を取得します。 |


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|name|String|予定表の名前。|
|changeKey|String|予定表オブジェクトのバージョンを識別します。予定表を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用。|
|color|String|UI で予定表を他の予定表から区別するための配色テーマを指定します。プロパティ値は次のとおりです。薄い青=0、薄い緑=1、薄いオレンジ=2、薄い灰色=3、薄い黄=4、薄い青緑=5、薄いピンク=6、薄い茶色=7、薄い赤=8、最大色=9、自動=-1|
|id|String|グループの一意識別子。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|calendarView|[Event](event.md) collection|予定表のカレンダー ビュー。ナビゲーション プロパティ。読み取り専用。|
|events|[Event](event.md) collection|予定表内のイベント。ナビゲーション プロパティ。読み取り専用。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| 予定表に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 予定表に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
