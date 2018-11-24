# <a name="teamguestsettings-resource-type"></a>teamGuestSettings リソースの種類



来園者が作成、更新、または[チーム](team.md)内のチャンネルを削除するかどうかを構成するのに設定します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|True の場合、来園者のセットを追加したりチャンネルを更新する場合。|
|allowDeleteChannels|Boolean|場合は true を指定すると、来園者に設定するには、チャンネルを削除できます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
