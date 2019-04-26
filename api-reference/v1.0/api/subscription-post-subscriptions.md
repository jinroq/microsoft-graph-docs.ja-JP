---
title: サブスクリプションを作成する
description: Microsoft Graph のデータが変更されたときに通知を受信するため、リスナー アプリケーションに登録します。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 6d06e230dd85aadaa4d2b3a4f851b339b34793eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560978"
---
# <a name="create-subscription"></a>サブスクリプションを作成する

変更の要求された種類が Microsoft Graph の指定されたリソースに発生したときに通知を受信するため、リスナー アプリケーションに登録します。

## <a name="permissions"></a>アクセス許可

 サブスクリプションを作成するにはリソースへの読み取りスコープが必要です。 たとえば、メッセージに関する通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。 
 
 要求されたリソースとアクセス許可の種類 (委任およびアプリケーション) によっては、以下の表で指定されているアクセス許可がこの API を呼び出すために最小限必要な特権となります。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| サポートされているリソース | 委任 (職場または学校のアカウント) | 委任 (個人用 Microsoft アカウント) | アプリケーション |
|:-----|:-----|:-----|:-----|
|[連絡先](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (ユーザーの個人用 OneDrive) | サポート対象外 | Files.ReadWrite | サポート対象外 |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | サポート対象外 | Files.ReadWrite.All |
|[イベント](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[グループ](../resources/group.md) | Group.Read.All | サポート対象外 | Group.Read.All |
|[グループ会話](../resources/conversation.md) | Group.Read.All | サポート対象外 | サポート対象外 |
|[メッセージ](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[セキュリティの警告](../resources/alert.md) | SecurityEvents.ReadWrite.All | サポート対象外 | SecurityEvents.ReadWrite.All |
|[ユーザー](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **注:** OneDrive と Outlook のアイテムのサブスクリプションについては、追加の制限があります。 この制限は、サブスクリプションの作成および管理 (サブスクリプションの取得、更新、削除) に適用されます。

- 個人用 OneDrive では、そのドライブのルート フォルダーまたは任意のサブフォルダーにサブスクライブできます。 OneDrive for Business の場合、サブスクライブできるのはルート フォルダーのみです。 サブスクライブしたフォルダー、または階層内の任意のファイル、フォルダー、あるいは他の **driveItem** インスタンスに関する変更の要求された種類についての通知が送信されます。 個別のファイルなどのフォルダーではない、**ドライブ** インスタンスまたは **driveItem** インスタンスをサブスクライブすることはできません。

- Outlook における委任されたアクセス許可では、サインインしているユーザーのメールボックス内のフォルダーにあるアイテムのみをサブスクライブできます。 つまり、委任されたアクセス許可 Calendars.Read を使用して、別のユーザーのメールボックス内のイベントをサブスクライブすることなどはできません。
- _共有または委任_フォルダーの Outlook 連絡先、イベント、メッセージの変更通知をサブスクライブするには、次のようにします。

  - 対応するアプリケーション アクセス許可を使用して、テナントの_任意_のユーザーのフォルダーまたはメールボックス内にあるアイテムの変更をサブスクライブします。
  - Outlook 共有アクセス許可 (Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared、および対応する読み取り/書き込み) は使用しないでください。それらは、共有フォルダーまたは委任フォルダーにあるアイテムの変更通知のサブスクライブをサポート**していない**からです。 


## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

ユーザーが新しいメールを受信したときに通知を送信する要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

要求本文で、[subscription](../resources/subscription.md) オブジェクトの JSON 表記を指定します。
`clientState` フィールドは省略可能です。

##### <a name="resources-examples"></a>リソースの例

以下は、サブスクリプションのリソース プロパティの有効な値です。

| リソースの種類 | 例 |
|:------ |:----- |
|メール|me/mailfolders('inbox')/messages<br />me/messages|
|連絡先|me/contacts|
|カレンダー|me/events|
|ユーザー|users|
|グループ|groups|
|会話|groups('*{id}*')/conversations|
|ドライブ|me/drive/root|
|セキュリティの警告|security/alerts?$filter=status eq ‘New’|

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a>通知エンドポイントの検証

サブスクリプションの通知のエンドポイントは (`notificationUrl` プロパティで指定されている)、「[ユーザー データの変更に関する通知の設定](/graph/webhooks#notification-endpoint-validation)」での説明にあるように、検証依頼に応答できなければなりません。 検証に失敗した場合、サブスクリプションを作成する要求は「400 要求が正しくありません」というエラーを返します。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
