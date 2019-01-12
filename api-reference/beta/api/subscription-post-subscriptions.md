---
title: サブスクリプションを作成する
description: Graph リソース上のデータが変更されたときに通知を受信するリスナー アプリケーションをサブスクライブします。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 0640a8de441a07e1abcc02a152f5a9812832db27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916545"
---
# <a name="create-subscription"></a>サブスクリプションを作成する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Graph リソース上のデータが変更されたときに通知を受信するリスナー アプリケーションをサブスクライブします。

## <a name="permissions"></a>アクセス許可

サブスクリプションを作成するには、アプリケーションが通知を受信するリソースの読み取り権限が必要です。 たとえば、メッセージに関する通知を取得するには、アプリが必要な`Mail.Read`のアクセス許可。 次の表に、各リソースに必要な、推奨されるアクセス許可を示します。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| リソースの種類/項目        | アクセス許可          |
|-----------------------------|---------------------|
| 連絡先                    | Contacts.Read       |
| スレッド               | Group.Read.All      |
| イベント                      | Calendars.Read      |
| メッセージ                    | Mail.Read           |
| グループ                      | Group.Read.All      |
| ユーザー                       | User.Read.All       |
| ドライブ (ユーザーの OneDrive)    | Files.ReadWrite     |
| ドライブ (共有、SharePoint コンテンツおよびドライブ) | Files.ReadWrite.All |
| セキュリティの警告              | SecurityEvents.ReadWrite.All |

> **注:**/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。 ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。

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

要求の本文には、[サブスクリプション](../resources/subscription.md)オブジェクトを JSON 表現したものを指定します。
`clientState`フィールドは省略可能です。

このサンプル リクエストは、現在サインインしているユーザーが受信したメールの通知のサブスクリプションを作成します。
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

リソース プロパティの設定値は、次のように。

| リソースの種類 | 例 |
|:------ |:----- |
|メール|me/mailfolders('inbox')/messages<br />me/messages|
|連絡先|me/contacts|
|カレンダー|me/events|
|ユーザー|users|
|グループ|グループ|
|会話|groups('*{id}*')/conversations|
|ドライブ|me/drive/root|
|セキュリティの警告|セキュリティと警告? $filter eq のステータスを 'New' =|

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

サブスクリプション通知エンドポイント (で指定されている、`notificationUrl`プロパティ) の[ユーザー データの変更の通知の設定](/graph/webhooks#notification-endpoint-validation)で説明したように、検証要求に応答できる必要があります。 検証が失敗した場合、サブスクリプションを作成する要求は 400 不正な要求のエラーを返します。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
