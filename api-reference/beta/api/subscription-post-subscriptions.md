---
title: サブスクリプションを作成する
description: Microsoft Graph リソース上のデータが変更されたときに通知を受信するリスナーアプリケーションをサブスクライブします。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a8b8189780ac0b820551fb885adcf843c9ebe8f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140167"
---
# <a name="create-subscription"></a>サブスクリプションを作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

リスナーアプリケーションをサブスクライブして、要求された種類の変更が Microsoft Graph の指定したリソースに対して発生したときに通知を受信します。

## <a name="permissions"></a>アクセス許可

サブスクリプションを作成するには、リソースに対する読み取りスコープが必要です。 たとえば、メッセージに関する通知を取得するには、アプリ`Mail.Read`にアクセス許可が必要です。 
 
 リソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可は、この API を呼び出すために必要な最低限の特権です。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| サポートされているリソース | 委任 (職場または学校のアカウント) | 委任 (個人用 Microsoft アカウント) | Application |
|:-----|:-----|:-----|:-----|
|[連絡先](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[ドライブ項目](../resources/driveitem.md)(ユーザーの個人用 OneDrive) | サポートされていません | Files.ReadWrite | サポートされていません |
|[ドライブ項目](../resources/driveitem.md)(OneDrive for business) | Files.ReadWrite.All | サポートされていません | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | サポートされていません | Group.Read.All |
|[グループ会話](../resources/conversation.md) | Group.Read.All | 使用不可 | 使用不可 |
|[message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[セキュリティの警告](../resources/alert.md) | SecurityEvents.ReadWrite.All | サポートされていません | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **注:** OneDrive および Outlook アイテムのサブスクリプションには、追加の制限があります。 この制限は、サブスクリプションの作成と管理 (サブスクリプションの取得、更新、および削除) に適用されます。

- 個人用 OneDrive では、ルートフォルダーまたはそのドライブの任意のサブフォルダーを購読できます。 OneDrive for business では、ルートフォルダーのみをサブスクライブできます。 通知は、サブスクライブされたフォルダー、または、階層内の任意のファイル、フォルダー、またはその他の**ドライブのアイテム**インスタンスに対して、要求された種類の変更に対して送信されます。 個別のファイルなど、フォルダーではない**drive**または**drive アイテム**のインスタンスを購読することはできません。

- Outlook では、委任されたアクセス許可は、サインインしているユーザーのメールボックス内のフォルダー内のアイテムのサブスクライブをサポートします。 つまり、委任されたアクセス許可のカレンダーを使用することはできません。別のユーザーのメールボックス内のイベントをサブスクライブするには、をお読みください。
- Outlook の連絡先、イベント、または_共有フォルダーまたは委任_されたフォルダー内のメッセージの変更通知を購読するには、次のようにします。

  - 対応するアプリケーションのアクセス許可を使用して、テナント内の_任意_のユーザーのフォルダーまたはメールボックス内のアイテムの変更をサブスクライブします。
  - 共有または委任されたフォルダー内のアイテムの通知を変更するためのサブスクライブをサポートして**い**ないため、Outlook 共有のアクセス許可 (連絡先. 共有、読み取り/書き込み可能) を使用しないでください。

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

要求本文で、 [subscription](../resources/subscription.md)オブジェクトの JSON 表記を指定します。
この`clientState`フィールドは省略可能です。

このサンプル要求は、現在サインインしているユーザーが受信した新着メールに関する通知のサブスクリプションを作成します。
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

resource プロパティの有効な値は次のとおりです。

| リソースの種類 | 例 |
|:------ |:----- |
|メール|me/mailfolders('inbox')/messages<br />me/messages|
|連絡先|me/contacts|
|カレンダー|me/events|
|ユーザー|users|
|グループ|グループ|
|会話|groups('*{id}*')/conversations|
|ドライブ|me/drive/root|
|セキュリティの警告|セキュリティ/アラートの $filter = 状態 eq ' 新規 '|

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

「 `notificationUrl` [ユーザーデータの変更の通知を設定](/graph/webhooks#notification-endpoint-validation)する」の説明に従って、プロパティで指定されているサブスクリプション通知エンドポイントは、検証要求に応答できる必要があります。 検証が失敗した場合、サブスクリプションを作成する要求は、400不良要求エラーを返します。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
