# <a name="create-and-send-outlook-messages"></a>Outlook メッセージを作成して送信する

Microsoft Graph では、メールは [message](../api-reference/v1.0/resources/message.md) リソースで表されます。 

既定で、メッセージは **id** プロパティの一意のエントリ ID で識別されます。 ストア プロバイダーは、メッセージが最初に下書きとして保存されるか送信されるときに、メッセージにエントリ ID を割り当てます。 この ID は、メッセージを別のフォルダー、ストア、または .PST ファイルにコピーしたり移動したりすると、変更されます。

## <a name="creating-and-sending-mail"></a>メールの作成と送信

Outlook では、同じ [sendMail](../api-reference/v1.0/api/user_sendmail.md) アクションでメールを作成および送信できます。また、下書きを[作成](../api-reference/v1.0/api/user_post_messages.md)してから[コンテンツを追加](../api-reference/v1.0/api/message_update.md)し、その下書きを[送信](../api-reference/v1.0/api/message_send.md)することもできます。

同様に、メールに返信する場合も、同じアクションで返信を送信できます ([返信](../api-reference/v1.0/api/message_reply.md)、[全員に返信](../api-reference/v1.0/api//message_replyall.md)、または[転送](../api-reference/v1.0/api/message_forward.md))。 また、返信の下書きを作成 ([返信](../api-reference/v1.0/api/message_createreply.md)、[全員に返信](../api-reference/v1.0/api//message_createreplyall.md)、または[転送](../api-reference/v1.0/api/message_createforward.md)) してから[コンテンツを追加](../api-reference/v1.0/api/message_update.md)し、その下書きを後で[送信](../api-reference/v1.0/api/message_send.md)することもできます。

下書きと送信済みメッセージをプログラムで区別するには、**isDraft** プロパティを確認します。 

既定では、下書きメッセージは `Drafts` フォルダーに保存され、送信済みメッセージは `Sent Items` フォルダーに保存されます。 利便性のため、Drafts フォルダーと SentItems フォルダーを、それぞれに対応するわかりやすいフォルダー名で指定することもできます。 たとえば、次のようにして Drafts フォルダー内の[メッセージを取得](../api-reference/v1.0/api/user_list_messages.md)できます。

```http
GET /me/mailfolders('Drafts')
```

### <a name="body-format-and-malicious-script"></a>本文の形式と悪意のあるスクリプト

<!-- Remove the following 2 sections from the message.md topics 
-->

メッセージ本文には、HTML 形式かテキスト形式を使用できます。GET 応答で返される既定のメッセージ本文の種類は HTML 形式です。

[メッセージを取得](../api-reference/v1.0/api/message_get.md)する際に、次の要求ヘッダーで、**body** プロパティと **uniqueBody** プロパティがテキスト形式で返されるように指定できます。

```
Prefer: outlook.body-content-type="text"
```
HTML 形式でメッセージ本文を取得するには、次のヘッダーを指定するか、単にこのヘッダーをスキップします。
```
Prefer: outlook.body-content-type="html"
```

いずれかのヘッダーを指定した場合、成功応答には対応する `Preference-Applied` ヘッダーが含まれます。

- テキスト形式要求の場合: `Preference-Applied: outlook.body-content-type="text"`
- HTML 形式要求の場合: `Preference-Applied: outlook.body-content-type="html"`

本文が HTML の場合、既定では、Outlook は **body** プロパティに埋め込まれている安全でない可能性のある HTML (JavaScript など) を削除してから、本文の内容を REST 応答で返します。

元の HTML コンテンツ全体を取得するには、次の HTTP 要求ヘッダーを含めます。
```
Prefer: outlook.allow-unsafe-html
```

### <a name="differentiating-the-from-and-sender-properties"></a>from プロパティと sender プロパティの区別

メッセージの作成中、Outlook はたいてい **from** プロパティと **sender** プロパティを同じサインイン ユーザーに設定しています。 次のシナリオでは、これらのプロパティを更新できます。

- **From** プロパティは、Exchange 管理者がメールボックスの **SendAs** 権限を他のユーザーに割り当てた場合には変更が可能です。管理者は、Azure ポータルでメールボックス所有者の **メールボックスのアクセス許可** を選択するか、Exchange 管理センターまたは Windows PowerShell Add-ADPermission コマンドレットを使用してこれを行えます。その後、プログラムを使用して、**From** プロパティを、対象メールボックスの **SendAs** 権限を持ついずれかのユーザーに自動的に設定できます。
- **sender** プロパティは、メールボックス所有者が 1 人以上のユーザーにそのメールボックスからメッセージを送信する権限を委任すると、変更できます。 メールボックス所有者は、Outlook で委任できます。 代理人がメールボックス所有者に代わってメッセージを送信する場合、Outlook は **sender** プロパティを代理人のアカウントに設定し、**from** プロパティはメールボックス所有者のままになります。 プログラムを使用して、対象メールボックスの委任アクセス許可を取得したユーザーに **sender** プロパティを設定することができます。

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a>MailTips を使用して受信者の状態を確認し、時間を節約する (プレビュー)

[MailTips](../api-reference/beta/resources/mailtips.md) を使用すると、メールを送信する前にスマートに意思決定できます。 MailTips を使用すると、受信者のメールボックスが特定の送信者のみに制限されているかどうかや、その受信者にメールを送信するには承認が必要かなどの情報を取得できます。

## <a name="integrating-with--social-gesture-preview"></a>@ ソーシャル ジェスチャとの統合 (プレビュー)

@ メンションとは、それらがメッセージに含まれている場合にユーザーに警告する通知のことです。 [mention](../api-reference/beta/resources/mention.md) リソースを使用すると、メールに含まれる一般的なオンライン ソーシャル ジェスチャである @ プレフィックスを、アプリで設定および取得できます。
次の操作を実行できます。

- [メッセージを作成](../api-reference/beta/api/user_post_messages.md#request-2)する際に @ メンションを作成する
- [ユーザーのメールボックス内にある、そのユーザーの @ メンションを含むすべてのメッセージを取得する](../api-reference/beta/api/user_list_messages.md#request-2)
- [メッセージ内の @ メンションすべてを取得する](../api-reference/beta/api/message_get.md#request-2) 


## <a name="other-shared-capabilities"></a>その他の共有機能

Microsoft Graph エンティティ間で共有されている次の一般的な機能を活用します。

- メッセージの作成や更新など、1 つ以上の種類の変更が発生した場合の、メッセージの[変更通知](../api-reference/v1.0/resources/webhooks.md)を受信登録します。
- [フォルダー内のメッセージへの増分の変更を追跡](delta_query_messages.md)します。
- [オープン拡張機能](extensibility_overview.md#open-extensions)や[スキーマ拡張機能](extensibility_overview.md#schema-extensions)を作成して、メッセージ インスタンスにカスタム データを追加します。
- Outlook MAPI プロパティが Microsoft Graph API メタデータでまだ公開されていない場合は、メッセージ インスタンスで[拡張プロパティ](../api-reference/v1.0/resources/extended-properties-overview.md)を作成して、それらのプロパティのカスタム データを保存します。

## <a name="next-steps"></a>次の手順

詳細情報:

- [Outlook メールと統合する理由](outlook-mail-concept-overview.md)
- Microsoft Graph v1.0 の[メール API](../api-reference/v1.0/resources/mail_api_overview.md) とその[用途](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)