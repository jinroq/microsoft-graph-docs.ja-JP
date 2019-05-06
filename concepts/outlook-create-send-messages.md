---
title: メッセージの作成、送信、処理の自動化
description: Microsoft Graph では、メールは message リソースで表されます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 06074950ae1ea81be9546066ebff05825d44b700
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2019
ms.locfileid: "33440088"
---
# <a name="automate-creating-sending-and-processing-messages"></a>メッセージの作成、送信、処理の自動化

Microsoft Graph では、メールは [message](/graph/api/resources/message?view=graph-rest-1.0) リソースで表されます。

既定で、メッセージは **id** プロパティの一意のエントリ ID で識別されます。 ストア プロバイダーは、メッセージが最初に作成されて、下書きとして保存されるか送信されるときに、そのメッセージにエントリ ID を割り当てます。 既定でこの ID は、メッセージを別のフォルダー、ストア、.PST ファイルにコピーしたり移動したりすると、変更されます。 今後の処理のために、メッセージは現在の ID で参照されます。

## <a name="creating-and-sending-mail"></a>メールの作成と送信

Outlook では、同じ [sendMail](/graph/api/user-sendmail?view=graph-rest-1.0) アクションでメールを作成および送信できます。また、下書きを[作成](/graph/api/user-post-messages?view=graph-rest-1.0)してから[コンテンツを追加](/graph/api/message-update?view=graph-rest-1.0)し、その下書きを[送信](/graph/api/message-send?view=graph-rest-1.0)することもできます。

同様に、メールに返信する場合も、同じアクションで返信を送信できます ([返信](/graph/api/message-reply?view=graph-rest-1.0)、[全員に返信](/graph/api/message-replyall?view=graph-rest-1.0)、または[転送](/graph/api/message-forward?view=graph-rest-1.0))。 また、返信の下書きを作成 ([返信](/graph/api/message-createreply?view=graph-rest-1.0)、[全員に返信](/graph/api/message-createreplyall?view=graph-rest-1.0)、または[転送](/graph/api/message-createforward?view=graph-rest-1.0)) してから[コンテンツを追加](/graph/api/message-update?view=graph-rest-1.0)し、その下書きを後で[送信](/graph/api/message-send?view=graph-rest-1.0)することもできます。

下書きと送信済みメッセージをプログラムで区別するには、**isDraft** プロパティを確認します。

既定では、下書きメッセージは `Drafts` フォルダーに保存され、送信済みメッセージは `Sent Items` フォルダーに保存されます。 利便性のため、Drafts フォルダーと SentItems フォルダーを、それぞれに対応する[わかりやすいフォルダー名](/graph/api/resources/mailfolder?view=graph-rest-1.0)で指定することもできます。 

### <a name="setting-the-from-and-sender-properties"></a>from プロパティと sender プロパティの設定

メッセージの作成中、Outlook はたいてい **from** プロパティと **sender** プロパティを同じサインイン ユーザーに設定しています。 次のシナリオでは、これらのプロパティを更新できます。

- **From** プロパティは、Exchange 管理者がメールボックスの **SendAs** 権限を他のユーザーに割り当てた場合には変更が可能です。管理者は、Azure ポータルでメールボックス所有者の **メールボックスのアクセス許可** を選択するか、Exchange 管理センターまたは Windows PowerShell Add-ADPermission コマンドレットを使用してこれを行えます。その後、プログラムを使用して、**From** プロパティを、対象メールボックスの **SendAs** 権限を持ついずれかのユーザーに自動的に設定できます。
- **sender** プロパティは、メールボックス所有者が 1 人以上のユーザーにそのメールボックスからメッセージを送信する権限を委任すると、変更できます。 メールボックス所有者は、Outlook で委任できます。 代理人がメールボックス所有者に代わってメッセージを送信する場合、Outlook は **sender** プロパティを代理人のアカウントに設定し、**from** プロパティはメールボックス所有者のままになります。 プログラムを使用して、対象メールボックスの委任アクセス許可を取得したユーザーに **sender** プロパティを設定することができます。

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a>MailTips を使用して受信者の状態を確認し、時間を節約する (プレビュー)

[MailTips](/graph/api/resources/mailtips?view=graph-rest-beta) を使用すると、メールを送信する前にスマートに意思決定できます。
MailTips を使用すると、受信者のメールボックスが特定の送信者のみに制限されているかどうかや、その受信者にメールを送信するには承認が必要かなどの情報を取得できます。


## <a name="reading-messages-with-control-over-the-body-format-returned"></a>返される本文の形式を制御したメッセージの読み取り

ID を参照してメールボックス内の[メッセージを読み取る](/graph/api/message-get?view=graph-rest-1.0)ことができます。

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["AAMkADhMGAAA="]
}-->
```http
GET /me/messages/AAMkADhMGAAA=
```

または、特定のフォルダー内の[メッセージを取得する](/graph/api/user-list-messages?view=graph-rest-1.0)ことができます。 たとえば、サインインしたユーザーの下書きフォルダーにあるメッセージを読み取るには、以下を行います。

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailfolders('Drafts')
```

Outlook メッセージの本文には、HTML 形式かテキスト形式を使用できます。GET 応答で返される既定のメッセージ本文の種類は HTML 形式です。

メッセージを取得する際に、次の要求ヘッダーで、**body** プロパティと **uniqueBody** プロパティがテキスト形式で返されるように指定できます。

```http
Prefer: outlook.body-content-type="text"
```

HTML 形式でメッセージ本文を取得するには、次のヘッダーを指定するか、単にこのヘッダーをスキップします。

```http
Prefer: outlook.body-content-type="html"
```

いずれかのヘッダーを指定した場合、成功応答には対応する `Preference-Applied` ヘッダーが含まれます。

- テキスト形式要求の場合: `Preference-Applied: outlook.body-content-type="text"`
- HTML 形式要求の場合: `Preference-Applied: outlook.body-content-type="html"`

本文が HTML の場合、既定では、Outlook は **body** プロパティに埋め込まれている安全でない可能性のある HTML (JavaScript など) を削除してから、本文の内容を REST 応答で返します。

元の HTML コンテンツ全体を取得するには、次の HTTP 要求ヘッダーを含めます。

```http
Prefer: outlook.allow-unsafe-html
```

## <a name="integrating-with--social-gesture-preview"></a>@ ソーシャル ジェスチャとの統合 (プレビュー)

@ メンションとは、それらがメッセージに含まれている場合にユーザーに警告する通知のことです。 [mention](/graph/api/resources/mention?view=graph-rest-beta) リソースを使用すると、メールに含まれる一般的なオンライン ソーシャル ジェスチャである @ プレフィックスを、アプリで設定および取得できます。
次の操作を実行できます。

- [メッセージを作成](/graph/api/user-post-messages?view=graph-rest-beta#request-2)する際に @ メンションを作成する
- [ユーザーのメールボックス内にある、そのユーザーの @ メンションを含むすべてのメッセージを取得する](/graph/api/user-list-messages?view=graph-rest-beta#request-2)
- [メッセージ内の @ メンションすべてを取得する](/graph/api/message-get?view=graph-rest-beta#request-2)

## <a name="other-shared-capabilities"></a>その他の共有機能

Microsoft Graph エンティティ間で共有されている次の一般的な機能を活用します。

- メッセージの作成や更新など、1 つ以上の種類の変更が発生した場合の、メッセージの[変更通知](/graph/api/resources/webhooks?view=graph-rest-1.0)を受信登録します。
- [フォルダー内のメッセージへの増分の変更を追跡](delta-query-messages.md)します。
- [オープン拡張機能](extensibility-overview.md#open-extensions)や[スキーマ拡張機能](extensibility-overview.md#schema-extensions)を作成して、メッセージ インスタンスにカスタム データを追加します。
- Outlook MAPI プロパティが Microsoft Graph API メタデータでまだ公開されていない場合は、メッセージ インスタンスで[拡張プロパティ](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0)を作成して、それらのプロパティのカスタム データを保存します。

## <a name="next-steps"></a>次の手順

詳細情報:

- [Outlook メールと統合する理由](outlook-mail-concept-overview.md)
- [MIME コンテンツを取得する](outlook-get-mime-message.md)
- [共有メッセージを取得する](outlook-share-messages-folders.md)
- [別のユーザーを差出人として Outlook メッセージを送信する](outlook-send-mail-from-other-user.md)
- [Outlook リソースの不変 ID の取得 (プレビュー)](outlook-immutable-id.md)
- Microsoft Graph v1.0 の[メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とその[用途](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。
