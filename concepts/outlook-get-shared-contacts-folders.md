---
title: 共有フォルダー内にある Outlook の連絡先を取得する
description: Outlook では、ユーザーがフォルダーを互いに共有し、個々の連絡先フォルダーに対する読み取り、作成、変更、削除のアクセス権を与えることができます。 Outlook では、あるユーザーが、そのユーザーの代わりに操作する権限を別のユーザーに与えることもできます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86533a28c0af206458b63fd19f32f01c5b68710b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585441"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a>共有フォルダー内にある Outlook の連絡先を取得する

Outlook では、ユーザーがフォルダーを互いに共有し、個々の連絡先フォルダーに対する "読み取り"、"作成"、"変更"、"削除" のアクセス権を与えることができます。 また、Outlook では、あるユーザーが別のユーザーの代理人としてふるまい、ユーザーのメールボックス全体の中にある特定のフォルダーにアクセスすることもできます。これは Outlook では "委任" とも呼ばれます。

Microsoft Graph では、他のユーザーによって共有された連絡先フォルダーの連絡先を取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。 また、委任メールボックスのフォルダーにもサポートが適用されます。

たとえば、Garth が John とカスタム連絡先フォルダーを共有し、John に読み取りアクセス権を与えたとします。 John がアプリにサインインし、委任されたアクセス許可 (Contacts.Read.Shared または Contacts.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth のカスタム連絡先フォルダーと、そのフォルダー内にある連絡先にアクセスすることができます。

> **注** 共有アクセス許可 (Contacts.Read.Shared または Contacts.ReadWrite.Shared) が与えられると、共有または委任されたフォルダーで連絡先を読み書きできます。 そのようなフォルダーでアイテムの[変更通知をサブスクライブする](webhooks.md)ことはできません。 テナントで共有フォルダー、委任フォルダー、その他のユーザーの連絡先フォルダーに含まれている連絡先に変更通知サブスクリプションを設定するには、アプリケーション アクセス許可の Contacts.Read を使用します。

## <a name="get-a-contact-in-the-shared-folder"></a>共有フォルダー内の連絡先を取得

Garth が John と共有したカスタム連絡先フォルダーの特定の連絡先を取得できます。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダー`{id}`によって識別される[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)インスタンスが取得されます。

## <a name="get-all-contacts-in-the-shared-folder"></a>共有フォルダー内の全連絡先を取得

Garth の共有フォルダー内の全連絡先を取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダーにある[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)インスタンスのコレクションが取得されます。

## <a name="get-the-shared-folder"></a>共有フォルダーを取得

Garth が John と共有した連絡先フォルダーを取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

正常に終了すると、HTTP 200 OK となり、Garth の共有連絡先フォルダーを表す [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) インスタンスを取得します。

Garth が John に対して自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。

Garth が John と連絡先フォルダーを共有しておらず、自分のメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。 


## <a name="next-steps"></a>次のステップ

詳細情報:

- [Outlook 個人用連絡先を統合する理由](outlook-contacts-concept-overview.md)
- Microsoft Graph v1.0 の[連絡先](/graph/api/resources/contact?view=graph-rest-1.0) API。
