---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 54922bfb6cd1c46c448a9cd75de3c66f94767fa3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271478"
---
# <a name="delete-subscription"></a>サブスクリプションを削除する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

サブスクリプションを削除します。

## <a name="permissions"></a>アクセス許可

要求されたリソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、以下の表で指定されているアクセス許可がこの API を呼び出すため必要な最小限の特権となります。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| サポートされているリソース | 委任 (職場または学校のアカウント) | 委任 (個人用 Microsoft アカウント) | アプリケーション |
|:-----|:-----|:-----|:-----|
|[連絡先](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (ユーザーの個人用 OneDrive) | サポートされていません | Files.ReadWrite | サポートされていません |
|[driveItem](../resources/driveitem.md) (OneDrive for Business) | Files.ReadWrite.All | サポートされていません | Files.ReadWrite.All |
|[イベント](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[グループ](../resources/group.md) | Group.Read.All | サポート対象外 | Group.Read.All |
|[グループ会話](../resources/conversation.md) | Group.Read.All | 非サポート | 非サポート |
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
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a>応答

以下は、応答の例です。
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>SDK サンプル コード
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_subscription-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_subscription-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_subscription-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscription-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
