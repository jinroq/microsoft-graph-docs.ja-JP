# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings リソースの種類



メッセージングを構成する設定は、[チーム](team.md)内の参照。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolean|場合 true の場合、ユーザーに設定するには、自分のメッセージを編集できます。|
|allowUserDeleteMessages|Boolean|場合は true の場合、ユーザーに設定するには、そのメッセージを削除できます。|
|allowOwnerDeleteMessages|Boolean|場合は true の場合、所有者に設定するには、任意のメッセージを削除できます。|
|allowTeamMentions|Boolean|場合、参照投稿を許可する @team を true に設定します。|
|allowChannelMentions|Boolean|場合、参照投稿を許可する @channel を true に設定します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
