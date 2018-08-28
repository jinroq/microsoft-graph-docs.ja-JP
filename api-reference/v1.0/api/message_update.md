# <a name="update-message"></a>メッセージを更新する

メッセージ オブジェクトのプロパティを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Mail.ReadWrite    |
|委任 (個人用 Microsoft アカウント) | Mail.ReadWrite    |
|アプリケーション | Mail.ReadWrite |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| 承認  | 文字列  | ベアラー {トークン}。必須。 |
| Content-Type | 文字列  | エンティティ本文内のデータの性質です。必須。 |
## <a name="request-body"></a>要求本文
要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。

| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|bccRecipients|Recipient|メッセージの BCC 受信者。 isDraft = trueの場合にのみ更新可能です。|
|categories|String コレクション|メッセージに関連付けられたカテゴリ。|
|ccRecipients|Recipient collection|メッセージの CC 受信者。 isDraft = trueの場合にのみ更新可能です。|
|from|Recipient|メッセージのメールボックス所有者と送信者。 isDraft = trueの場合にのみ更新可能です。 値は、使用される実際のメールボックスに対応する必要があります。|
|importance|文字列|メッセージの重要度。 使用可能な値: `Low`、`Normal`、`High`。|
|inferenceClassification | 文字列 | 推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーの対象メッセージの分類。 使用可能な値: `focused` または `other`。 |
|internetMessageId |文字列 |[RFC2822](http://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。 isDraft = trueの場合にのみ更新可能です。|
|isRead|ブーリアン|メッセージが読み取られたかどうかを示します。|
|replyTo|Recipient collection|返信時に使用される電子メール アドレス。 isDraft = trueの場合にのみ更新可能です。|
|sender|Recipient|メッセージを生成するために実際に使用されるアカウント。 isDraft = true の場合、そして[共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)からメッセージを送信、または [デリゲート](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信した場合にのみ更新可能です。 値は、使用される実際のメールボックスに対応する必要があります。|
|toRecipients|Recipient collection|メッセージの宛先。 isDraft = trueの場合にのみ更新可能です。|
|本文|ItemBody|メッセージの本文。 isDraft = trueの場合にのみ更新可能です。|
|isDeliveryReceiptRequested|ブーリアン|メッセージの開封応答が要求されているかどうかを示します。|
|isReadReceiptRequested|ブーリアン|メッセージの開封応答が要求されているかどうかを示します。|
|subject|文字列|メッセージの件名を指定します。 isDraft = trueの場合にのみ更新可能です。|

**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
