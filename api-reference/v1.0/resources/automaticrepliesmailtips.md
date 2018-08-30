# <a name="automaticrepliesmailtips-resource-type"></a>automaticRepliesMailTips リソースの種類


メールボックスで設定されている自動返信についての[メール ヒント](../resources/mailtips.md)。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:-----|:-----|:-----|
| message | 文字列 | 自動応答メッセージ。 |
| messageLanguage | [localeInfo](../resources/localeinfo.md) | 自動応答メッセージの言語。 |
| ScheduledEndTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 自動応答を終了する日時。 |
| ScheduledStartTime | [dateTimeTimeZone](../resources/datetimetimezone.md) | 自動応答を開始する日時。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->