---
title: 共有または委任された予定表内の Outlook イベントを取得する
description: Outlook では、ユーザーが予定表を他のユーザーと共有し、他のユーザーがその予定表でイベントの表示や変更を行うことができます。 また、ユーザーは、会議出席依頼の受信と返信や、予定表項目の作成と変更を自分に代わって実行する代理人を許可することができます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 773d996e8343c69028a7cbbe8a1a4283f5470108
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554696"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>共有または委任された予定表内の Outlook イベントを取得する

Outlook では、ユーザーが予定表を他のユーザーと共有し、他のユーザーがその予定表でイベントの表示や変更を行うことができます。 また、ユーザーは、会議出席依頼の受信と返信や、予定表項目の作成と変更を自分に代わって実行する代理人を許可することができます。

Microsoft Graph では、他のユーザーによって共有された予定表のイベントを取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。 サポートは、委任された予定表にも適用されます。

たとえば、Garth が John と既定の予定表を共有し、John に読み取りアクセス権を与えたとします。 John がアプリにサインインし、委任されたアクセス許可 (Calendars.Read.Shared または Calendars.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth の既定の予定表フォルダーと、その予定表内にあるイベントにアクセスすることができます。

> **注** 共有アクセス許可 (Calendars.Read.Shared または Calendars.ReadWrite.Shared) が与えられると、共有または委任されたカレンダーでイベントを読み書きできます。 そのようなフォルダーでアイテムの[変更通知をサブスクライブする](webhooks.md)ことはできません。 テナントで共有カレンダー、委任カレンダー、その他のユーザーまたはリソース カレンダーに含まれているイベントに変更通知サブスクリプションを設定するには、アプリケーション アクセス許可の Calendars.Read を使用します。

## <a name="get-an-event-in-the-shared-calendar"></a>共有予定表内のイベントを取得する

Garth が共有している既定の予定表にある特定のイベントを取得できます。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

正常に終了すると、HTTP 200 OK となり、Garth の既定の予定表から `{id}` によって識別される[イベント](/graph/api/resources/event?view=graph-rest-1.0) インスタンスが取得されます。

## <a name="get-all-the-events-in-the-shared-calendar"></a>共有予定表内のすべてのイベントを取得する

Garth が John と共有した既定の予定表にあるすべてのイベントを取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

正常に終了すると、HTTP 200 OK となり、Garth の既定の予定表にある[イベント](/graph/api/resources/event?view=graph-rest-1.0) インスタンスのコレクションが取得されます。

## <a name="get-the-shared-calendar"></a>共有予定表を取得する

Garth が John と共有した既定の予定表を取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

正常に終了すると、HTTP 200 OK となり、Garth の既定のフォルダーを表す [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) インスタンスが取得します。

Garth が John に対して、Garth の既定の予定表に対するさらに多くのアクセス権を委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。

Garth が John と既定の予定表を共有しておらず、メールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。 


## <a name="next-steps"></a>次のステップ

詳細情報:

- [Outlook カレンダーと統合する理由](outlook-calendar-concept-overview.md)
- Microsoft Graph v1.0 の[予定表 API](/graph/api/resources/calendar?view=graph-rest-1.0)
