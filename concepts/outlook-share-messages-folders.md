---
title: 共有または委任されたフォルダー内の Outlook メッセージを取得する
description: イベントの一覧表示、イベントの取得、予定表の取得、連絡先の一覧表示、連絡先の取得、連絡先フォルダーの各トピックにも、同様のセクションがあります。
author: angelgolfer-ms
ms.openlocfilehash: d90fa5d37fd7a07e4069bd5bcc0eb46f0cae29a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320112"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>共有または委任されたフォルダー内の Outlook メッセージを取得する

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

Outlook では、ユーザーがメール フォルダーを互いに共有し、個々のフォルダーに対する "読み取り"、"作成"、"変更"、"削除" のアクセス権を与えることができます。 また、Outlook では、あるユーザーが別のユーザーの代理人としてふるまい、ユーザーのメールボックス全体の中にある特定のメール フォルダーにアクセスすることもできます。これは Outlook では "委任" とも呼ばれます。

Microsoft Graph では、他のユーザーと共有するメール フォルダーのメッセージを取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。 サポートは、委任されたフォルダーにも適用されます。

たとえば、Garth が自分の受信トレイを John と共有し、読み取りアクセス権を与えたとします。 John がアプリにサインインし、委任されたアクセス許可 (Mail.Read.Shared または Mail.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth のメールおよび Garth の受信トレイにアクセスすることができます。

## <a name="get-a-message-in-the-shared-folder"></a>共有フォルダーのメッセージを取得

Garth の受信トレイの特定のメッセージを取得できます:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

正常に終了した場合、HTTP 200 OK となり、Garth の受信トレイから `{id}` によって識別される[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) インスタンスを取得します。

## <a name="get-all-messages-in-the-shared-folder"></a>共有フォルダー内の全メッセージを取得

Garth の受信トレイの全メッセージを取得:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

正常に終了すると、HTTP 200 OK となり、Garth の受信トレイの[メッセージ](/graph/api/resources/message?view=graph-rest-1.0) インスタンスのコレクションを取得します。

## <a name="get-the-shared-folder"></a>共有フォルダーを取得

Garth が John と共有したフォルダー (受信トレイ) を取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

正常に終了すると、HTTP 200 OK となり、Garth の受信トレイ フォルダーを表す [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) インスタンスを取得します。

Garth が John に対して、Garth の受信トレイへのさらに多くのアクセス権を委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。

Garth が John と受信トレイを共有しておらず、メールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。 


## <a name="next-steps"></a>次のステップ

詳細情報:

- [Outlook メールと統合する理由](outlook-mail-concept-overview.md)
- Microsoft Graph v1.0 の[メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とその[用途](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)