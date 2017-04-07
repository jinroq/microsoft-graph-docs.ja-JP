# <a name="mailboxsettings-resource-type"></a>mailboxSettings リソースの種類

サインイン ユーザーのプライマリ メールボックスの設定。


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。|
|language|[localeInfo](localeinfo.md)|優先言語および国/地域を含むユーザーのロケール情報。|
|timeZone|string|ユーザーのメールボックスの既定のタイム ゾーン。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->