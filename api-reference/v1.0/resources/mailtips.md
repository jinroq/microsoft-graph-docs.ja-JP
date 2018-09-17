# <a name="mailtips-resource-type"></a>mailTips リソースの種類

メッセージの作成中にユーザーに表示される、受信者に関する情報メッセージです。 メッセージの受信者に対する自動返信としての不在時のメッセージがその例です。


## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
| AutomaticReplies | [AutomaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | 受信者によって設定されている場合の自動応答に関するメールのヒント。 |
| CustomMailTip | 文字列 | 受信者のメールボックスに設定可能なカスタム メールのヒント。 |
| DeliveryRestricted| ブール値 | 受信者のメールボックスが制限されているかどうか。たとえば、送信者の定義済みリストからのメッセージのみを受け付ける、送信者の定義済みリストからのメッセージを拒否する、または認証された送信者からのメッセージのみを受信するなどです。 |
| emailAddress | [emailAddress](../resources/emailaddress.md) | メールヒントを取得する受信者の電子メール アドレス。 |
| エラー | [mailTipsError](../resources/mailtipserror.md) | [GetMailTips](../api/user_getmailtips.md) アクション中に発生するエラー。 |
| ExternalMemberCount | Int32 | 受信者が配布リストの場合は外部メンバーの数です。 |
| IsModerated |ブール値  | 受信者へのメッセージ送信に承認が必要かどうか。たとえば、受信者が大規模な配布リストであり、モデレーターが配布リストに送信されたメッセージを承認するようにセットアップされている場合、または受信者へのメッセージの送信に受信者の上司の承認を必要とする場合などです。 |
| MailboxFull | ブール値 | 受信者のメールボックスのフル状態。 |
| MaxMessageSize | Int32 | 受信者の組織またはメールボックスに対して構成されているメッセージの最大サイズ。 |
| RecipientScope | RecipientScopeType | 受信者のスコープです。 可能な値は、`none`、`internal`、`external`、`externalPartner`、`externalNonParther` です。 たとえば、管理者は別の組織をその「パートナー」に設定できます。 スコープは、管理者が特定のメール ヒントが特定のスコープにアクセスできるようにしたい場合に便利です。 メッセージが組織から送信されても支障がないことを送信者に伝えたり、言葉遣いや文調、内容について正しい判断を下せるよう支援するのにも役立ちます。|
| RecipientSuggestions | [recipient](../resources/recipient.md) コレクション | 同じメッセージに表示される前のコンテキストに基づいて提案される受信者。 |
| TotalMemberCount | Int32 | 受信者が配布リストの場合はメンバー数です。 |

### <a name="recipientscopetype-values"></a>recipientScopeType 値

| 値
|:-------------------------
| なし
| 内部
| 外部
| ExternalPartner
| ExternalNonPartner


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
