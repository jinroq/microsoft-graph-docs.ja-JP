---
title: Outlook メール REST API を使用する
description: Microsoft Graph を使用すると、アプリは個人または組織のアカウントでユーザーの Outlook メール データに正当にアクセスできます。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: a42b1508ab022bfd530b9338dc8049c65f478727
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463797"
---
# <a name="use-the-outlook-mail-rest-api"></a>Outlook メール REST API を使用する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph では、個人または組織のアカウントにあるユーザーの Outlook メール データに、アプリからアクセスすることを許可できます。[適切な代理アクセス許可またはアプリケーション アクセス許可](/graph/permissions-reference)を使用すると、アプリはサインインしているユーザーまたはテナント内のユーザーのメール データにアクセスできます。メール データは、Office 365 の一部として Exchange Online 上のクラウド内に存在することも、[ハイブリッド展開](/graph/hybrid-rest-support)の Exchange On-Premise 上に存在することもあります。

## <a name="using-the-mail-rest-api"></a>メール REST API の使用

メール API 要求は、ユーザーの **id** プロパティ (一意の GUID)、電子メール アドレス、サインインしているユーザーの `me` ショートカット エイリアスで識別できる[ユーザー](../resources/user.md)に代わって実行されます。

電子メール メッセージは、[message](../resources/message.md) リソースによって表され、[mailFolder](../resources/mailfolder.md) で構成されています。メッセージとメール フォルダーは、`GET` 操作から取得できる **id** プロパティによって識別されます。

> **注:** 一般的に、メールボックス内で **message** と **mailfolder** ID が一意で不変であるとは想定しないでください。これは、コピー、移動、送信などの特定の操作の後に変更される可能性があります。

メッセージ本文は、HTML 形式またはテキスト形式になります。

`Inbox`、`Drafts`、`SentItems`、`DeletedItems` などの既知のフォルダー名を使用して、すべてのユーザーに既定で存在する特定のメール フォルダーを識別できます。 サポートされている既知のフォルダー名の一覧については、「[mailFolder リソースの種類](../resources/mailfolder.md)」を参照してください。

たとえば、最初にフォルダー ID を取得せずに、サインインしているユーザーの Outlook **送信済みアイテム** フォルダー内のメッセージを取得できます。

```http
GET /me/mailFolders('SentItems')/messages?$select=sender,subject
```

## <a name="common-use-cases"></a>一般的なユース ケース

**message** リソースは、UI で利用可能な機能に対応する **categories**、**conversationId**、**flag**、**importance** などのプロパティを公開し、アプリを自動化したり、組み込みの Outlook ユーザー エクスペリエンスを統合したりできるようにします。

Microsoft Graph API には、メッセージの一般的なユース ケースをサポートするメソッドとアクションも用意されています。

| ユース ケース | REST リソース | 関連項目 |
|:----------|:---------------|:---------|
| **ユーザー指向のアクション** | | |
| メッセージを下書き、読み取り、返信、転送、送信、更新、削除する | [message](../resources/message.md) | [message のメソッド](../resources/message.md#methods) |
| メールボックス所有者の代理としてメッセージを送信するように別のユーザーに委任する | [message](../resources/message.md) | [メッセージ](../resources/message.md)の **from** プロパティと **sender** プロパティの設定 |
| ユーザーがより重要なメッセージを最初に表示できるようにする | [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) | [優先受信トレイ](../resources/manage-focused-inbox.md) |
| メッセージまたはメッセージの添付ファイルの MIME コンテンツを取得する (プレビュー) | [message](../resources/message.md) | [MIME コンテンツを取得する](/graph/outlook-get-mime-message) |
| メッセージの添付ファイルを追加、取得、削除する | [attachment](../resources/attachment.md)、 <br> [fileAttachment](../resources/fileattachment.md)、 <br> [itemAttachment](../resources/itemattachment.md)、 <br> [referenceAttachment](../resources/referenceattachment.md)、 <br> [message](../resources/message.md) | [添付ファイルのメソッド](../resources/attachment.md#methods) |
| ユーザーの言語とタイムゾーンの選択肢を取得する | [localeInfo](localeinfo.md)、 <br> [timeZoneInformation](timezoneinformation.md) | [supportedLanguages](../api/outlookuser-supportedlanguages.md)、 <br> [supportedTimeZones](../api/outlookuser-supportedtimezones.md) |
| ユーザーの自動応答、ロケール、タイム ゾーン、就業時間を取得または更新する | [mailboxSettings](../resources/mailboxsettings.md)、 <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md)、 <br> [localeInfo](../resources/localeinfo.md)、 <br> [workingHours](../resources/workinghours.md) | [ユーザーのメールボックスの設定を取得する](../api/user-get-mailboxsettings.md)、 <br> [ユーザーのメールボックスの設定を更新する](../api/user-update-mailboxsettings.md) |
| 不在など、他の受信者の特別な状態のメールヒントを取得する | [user](../resources/user.md)、 <br> [mailTips](../resources/mailtips.md) | [メール ヒントを取得する](../api/user-getmailtips.md) |
| その他のメッセージに記載されている場合は、ユーザーに警告する (プレビュー) | [mention (プレビュー)](../resources/mention.md) | [メッセージ内の @-mentions の詳細を取得する](../api/message-get.md#request-2) |
| ユーザーを電子メール配布リストの登録から解除する (プレビュー) | [message (プレビュー)](../resources/message.md) | [登録を解除する](../api/message-unsubscribe.md) |
| **メールとフォルダーの管理** | | |
| メール フォルダー階層内のメッセージを整理する | [mailFolder](../resources/mailfolder.md)  | [mailFolder のメソッド](../resources/mailfolder.md#methods) |
| メッセージを分類する | [outlookCategory (プレビュー)](../resources/outlookcategory.md) | [outlookCategory のメソッド](../resources/outlookcategory.md#methods) |
| 受信トレイのルールを使用して、特定の着信メッセージを転送するなどの操作を自動化する | [messageRule (プレビュー)](../resources/messagerule.md) | [messageRule のメソッド](../resources/messagerule.md#methods) |
| メッセージのインターネット メッセージ ヘッダーを取得する | [message (プレビュー)](../resources/message.md) | [メッセージの **internetMessageHeaders** プロパティを取得します](../api/message-get.md#request-4)。 |
| メッセージの検索とフィルター処理 | [message](../resources/message.md) | [クエリ パラメーター](/graph/query-parameters)  |
| フォルダー内のメッセージに対する変更の通知を受け取る | [subscription](../resources/subscription.md) | [Microsoft Graph の Webhooks での作業](../resources/webhooks.md) |
| メッセージまたはメール フォルダーの階層を同期する | [message](../resources/message.md) | [フォルダー内のメッセージへの増分の変更を取得する](/graph/delta-query-messages) |
| **アプリ開発** | | |
| カスタム アプリのデータをメッセージのインターネット メッセージ ヘッダーとして追加する | [message](../resources/message.md) | メッセージの **internetMessageHeaders** コレクションにカスタム データを追加します。 |
| 拡張機能を使用してカスタム アプリのデータをメッセージに追加する | [openTypeExtension](../resources/opentypeextension.md)、 <br>[schemaExtension](../resources/schemaextension.md) | [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview) |
| 公開の度合いが不十分の Outlook MAPI プロパティのカスタム データにアクセスする | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)、 <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>次の手順

メール API は、ユーザーと連携するための新しい方法を開発することができます。

- [Outlook メール API の概要](/graph/outlook-mail-concept-overview)
- [message](../resources/message.md) リソースと [mailFolder](../resources/mailfolder.md) リソースの[メソッド](../resources/message.md#methods)、[プロパティ](../resources/message.md#properties)、[リレーションシップ](../resources/message.md#relationships)について詳しく説明します。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。

さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。
