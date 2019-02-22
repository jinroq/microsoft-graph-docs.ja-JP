---
title: サブスクリプションを削除する
description: サブスクリプションを削除します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 97df6f59d4a8acfacec479e718970feef0c77632
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161433"
---
# <a name="delete-subscription"></a>サブスクリプションを削除する

サブスクリプションを削除します。

## <a name="permissions"></a>アクセス許可

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

- 個人用 OneDrive では、ルートフォルダーまたはそのドライブの任意のサブフォルダーを購読できます。 OneDrive for business では、ルートフォルダーのみをサブスクライブできます。 通知は、サブスクライブされたフォルダー、または、階層内の任意のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他のファイル、フォルダー、またはその他の 個別のファイルなど、フォルダーではない**drive**または**drive アイテム**のインスタンスを購読することはできません。

- Outlook では、委任されたアクセス許可は、サインインしているユーザーのメールボックス内のフォルダー内のアイテムのサブスクライブをサポートします。 つまり、委任されたアクセス許可のカレンダーを使用することはできません。別のユーザーのメールボックス内のイベントをサブスクライブするには、をお読みください。
- Outlook の連絡先、イベント、または_共有フォルダーまたは委任_されたフォルダー内のメッセージの変更通知を購読するには、次のようにします。

  - 対応するアプリケーションのアクセス許可を使用して、テナント内の_任意_のユーザーのフォルダーまたはメールボックス内のアイテムの変更をサブスクライブします。
  - 共有または委任されたフォルダー内のアイテムの通知を変更するためのサブスクライブをサポートして**い**ないため、Outlook 共有のアクセス許可 (連絡先. 共有、読み取り/書き込み可能) を使用しないでください。


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
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
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

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
