# <a name="messagerulepredicates-resource-type"></a>messageRulePredicates リソースの種類


ルールで使用可能な条件および例外のセットを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
| bodyContains | コレクション (文字列) | 条件または例外を適用するために、受信メッセージの本文に表示される文字列を表します。 |
| bodyOrSubjectContains | コレクション (文字列) | 条件または例外を適用するために、受信メッセージの本文または件名に表示される文字列を表します。 |
| カテゴリ | コレクション (文字列) | 条件または例外を適用するために、受信メッセージにラベルを付けるカテゴリを表します。 |
| fromAddresses | コレクション ([受信者](recipient.md)) | 条件または例外を適用するために、受信メッセージの特定の送信者のメール アドレスを表します。 |
| hasAttachments | ブール型 | 条件または例外を適用するために、受信メッセージに添付ファイルがあるかどうかを示します。 |
| headerContains | コレクション (文字列) | 条件または例外を適用するために、受信メッセージのヘッダーに表示される文字列を表します。 |
| 重要性 | 重要性 | 条件または例外を適用するために、受信メッセージに記録される重要性: `low`、`normal`、`high`。 |
| isApprovalRequest | ブール値 | 条件または例外を適用するために、受信メッセージが承認要求であるかどうかを示します。 |
| isAutomaticForward | ブール値 | 条件または例外を適用するために、受信メッセージが自動的に転送されるかどうかを示します。 |
| isAutomaticReply | ブール値 | 条件または例外を適用するために、受信メッセージが自動返信であるかどうかを示します。 |
| isEncrypted | ブール型 | 条件または例外を適用するために、受信メッセージが暗号化されるかどうかを示します。 |
| isMeetingRequest | ブール値 | 条件または例外を適用するために、受信メッセージが会議出席依頼であるかどうかを示します。 |
| isMeetingResponse | ブール値 | 条件または例外を適用するために、受信メッセージが会議出席依頼の返信であるかどうかを示します。 |
| isNonDeliveryReport | ブール値 | 条件または例外を適用するために、受信メッセージが配信不能レポートであるかどうかを示します。 |
| IsPermissionControlled | ブール値 | 条件または例外を適用するために、受信メッセージがアクセス許可制御 (RMS 保護) されるかどうかを示します。 |
| isReadReceipt | ブール値 | 条件または例外を適用するために、受信メッセージが開封確認メッセージであるかどうかを示します。 |
| isSigned | ブール値 | 条件または例外を適用するために、受信メッセージが S/MIME 署名されているかどうかを示します。 |
| isVoicemail | ブール値 | 条件または例外を適用するために、受信メッセージがボイス メールかどうかを示します。 |
| messageActionFlag | messageActionFlag  | 条件または例外を適用するために、受信メッセージに表示されるアクション フラグの値を表します。 可能な値は、`any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review` です。 |
| notSentToMe | ブール値 | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの受信者でないことを示します。 |
| recipientContains | コレクション (文字列) | 条件または例外を適用するために、受信メッセージの **ToRecipients** または **CcRecipients** プロパティに表示される文字列を表します。 |
| senderContains | コレクション (文字列) | 条件または例外を適用するために、受信メッセージの **From** プロパティに表示される文字列を表します。 |
| 秘密度 | 秘密度 | 条件または例外を適用するために、受信メッセージに記録される秘密度レベルを表します。 指定できる値は、`normal` 、`personal` 、`private` 、 `confidential` です。 |
| sentCcMe | ブール値 | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ccRecipients** プロパティにあるかどうかを示します。 |
| sentOnlyToMe | ブール値 | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの唯一の受信者かどうかを示します。 |
| sentToAddresses | コレクション ([受信者](recipient.md)) | 条件または例外を適用するために、受信メッセージが送信されたメール アドレスを表します。 |
| sentToMe | ブール値 | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ToRecipients** プロパティにあるかどうかを示します。 |
| sentToOrCcMe | ブール値 | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの **toRecipients** または **ccRecipients** プロパティにあるかどうかを示します。 |
| subjectContains | コレクション (文字列) | 条件または例外を適用するために、受信メッセージの件名に表示される文字列を表します。 |
| withinSizeRange | [sizeRange](sizerange.md) | 条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を表します。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
