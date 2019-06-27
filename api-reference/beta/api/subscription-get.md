---
title: サブスクリプションを取得する
description: サブスクリプションのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c6fe48d3eb72743de368a363330b63976c21156e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271471"
---
# <a name="get-subscription"></a>サブスクリプションを取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

サブスクリプションのプロパティとリレーションシップを取得します。

## <a name="permissions"></a>アクセス許可

要求されたリソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、以下の表で指定されているアクセス許可がこの API を呼び出すため必要な最小限の特権となります。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

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

- 個人用 OneDrive では、そのドライブのルート フォルダーまたは任意のサブフォルダーにサブスクライブできます。 OneDrive for Business の場合、サブスクライブできるのはルート フォルダーだけです。 サブスクライブしたフォルダー、または階層内の任意のファイル、フォルダー、あるいは他の driveItem オブジェクトの要求された種類の変更について通知が送信されます。 **ドライブ**、または個々のファイルなどのフォルダーではない **driveItem** インスタンスをサブスクライブすることはできません。

- Outlook における委任されたアクセス許可では、サインインしているユーザーのメールボックス内のフォルダーにあるアイテムのみをサブスクライブできます。 つまり、委任されたアクセス許可 Calendars.Read を使用して、別のユーザーのメールボックス内のイベントをサブスクライブすることなどはできません。
- _共有または委任_フォルダーの Outlook 連絡先、イベント、メッセージの変更通知をサブスクライブするには、次のようにします。

  - 対応するアプリケーション アクセス許可を使用して、テナントの_任意_のユーザーのフォルダーまたはメールボックス内にあるアイテムの変更をサブスクライブします。
  - Outlook 共有アクセス許可 (Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared、および対応する読み取り/書き込み) は使用しないでください。それらは、共有フォルダーまたは委任フォルダーにあるアイテムの変更通知のサブスクライブをサポート**していない**からです。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:-----|:-----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a>応答

以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscription-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscription-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_subscription-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
