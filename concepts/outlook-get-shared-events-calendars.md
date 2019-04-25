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
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="b7aa7-104">共有または委任された予定表内の Outlook イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="b7aa7-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="b7aa7-105">Outlook では、ユーザーが予定表を他のユーザーと共有し、他のユーザーがその予定表でイベントの表示や変更を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="b7aa7-106">また、ユーザーは、会議出席依頼の受信と返信や、予定表項目の作成と変更を自分に代わって実行する代理人を許可することができます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="b7aa7-107">Microsoft Graph では、他のユーザーによって共有された予定表のイベントを取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="b7aa7-108">サポートは、委任された予定表にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="b7aa7-109">たとえば、Garth が John と既定の予定表を共有し、John に読み取りアクセス権を与えたとします。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="b7aa7-110">John がアプリにサインインし、委任されたアクセス許可 (Calendars.Read.Shared または Calendars.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth の既定の予定表フォルダーと、その予定表内にあるイベントにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

> <span data-ttu-id="b7aa7-111">**注** 共有アクセス許可 (Calendars.Read.Shared または Calendars.ReadWrite.Shared) が与えられると、共有または委任されたカレンダーでイベントを読み書きできます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-111">**Note** The sharing permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared) allow you to read or write events in a shared or delegated calendar.</span></span> <span data-ttu-id="b7aa7-112">そのようなフォルダーでアイテムの[変更通知をサブスクライブする](webhooks.md)ことはできません。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="b7aa7-113">テナントで共有カレンダー、委任カレンダー、その他のユーザーまたはリソース カレンダーに含まれているイベントに変更通知サブスクリプションを設定するには、アプリケーション アクセス許可の Calendars.Read を使用します。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-113">To set up change notification subscriptions on events in a shared, delegated, or any other user or resource calendar in the tenant, use the application permission, Calendars.Read.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="b7aa7-114">共有予定表内のイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="b7aa7-114">Get an event in the shared calendar</span></span>

<span data-ttu-id="b7aa7-115">Garth が共有している既定の予定表にある特定のイベントを取得できます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-115">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="b7aa7-116">正常に終了すると、HTTP 200 OK となり、Garth の既定の予定表から `{id}` によって識別される[イベント](/graph/api/resources/event?view=graph-rest-1.0) インスタンスが取得されます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-116">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="b7aa7-117">共有予定表内のすべてのイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="b7aa7-117">Get all the events in the shared calendar</span></span>

<span data-ttu-id="b7aa7-118">Garth が John と共有した既定の予定表にあるすべてのイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-118">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="b7aa7-119">正常に終了すると、HTTP 200 OK となり、Garth の既定の予定表にある[イベント](/graph/api/resources/event?view=graph-rest-1.0) インスタンスのコレクションが取得されます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-119">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="b7aa7-120">共有予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="b7aa7-120">Get the shared calendar</span></span>

<span data-ttu-id="b7aa7-121">Garth が John と共有した既定の予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-121">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="b7aa7-122">正常に終了すると、HTTP 200 OK となり、Garth の既定のフォルダーを表す [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) インスタンスが取得します。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-122">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="b7aa7-123">Garth が John に対して、Garth の既定の予定表に対するさらに多くのアクセス権を委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-123">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="b7aa7-124">Garth が John と既定の予定表を共有しておらず、メールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="b7aa7-124">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="b7aa7-125">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b7aa7-125">Next steps</span></span>

<span data-ttu-id="b7aa7-126">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="b7aa7-126">Find out more about:</span></span>

- [<span data-ttu-id="b7aa7-127">Outlook カレンダーと統合する理由</span><span class="sxs-lookup"><span data-stu-id="b7aa7-127">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="b7aa7-128">Microsoft Graph v1.0 の[予定表 API](/graph/api/resources/calendar?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="b7aa7-128">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>
