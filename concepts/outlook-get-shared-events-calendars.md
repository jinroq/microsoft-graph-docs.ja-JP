---
title: 共有または委任された予定表内の Outlook イベントを取得する
description: Outlook では、ユーザーが予定表を他のユーザーと共有し、他のユーザーがその予定表でイベントの表示や変更を行うことができます。 また、ユーザーは、会議出席依頼の受信と返信や、予定表項目の作成と変更を自分に代わって実行する代理人を許可することができます。
author: angelgolfer-ms
ms.openlocfilehash: 8ceb6a49b971c5ad01f27b53c0f3cd3cf047865d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346565"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="82fca-104">共有または委任された予定表内の Outlook イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="82fca-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="82fca-105">Outlook では、ユーザーが予定表を他のユーザーと共有し、他のユーザーがその予定表でイベントの表示や変更を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="82fca-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="82fca-106">また、ユーザーは、会議出席依頼の受信と返信や、予定表項目の作成と変更を自分に代わって実行する代理人を許可することができます。</span><span class="sxs-lookup"><span data-stu-id="82fca-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="82fca-107">Microsoft Graph では、他のユーザーによって共有された予定表のイベントを取得したり、共有フォルダー自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="82fca-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="82fca-108">サポートは、委任された予定表にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="82fca-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="82fca-109">たとえば、Garth が John と既定の予定表を共有し、John に読み取りアクセス権を与えたとします。</span><span class="sxs-lookup"><span data-stu-id="82fca-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="82fca-110">John がアプリにサインインし、委任されたアクセス許可 (Calendars.Read.Shared または Calendars.ReadWrite.Shared) を与えた場合、アプリでは、下記のようにして Garth の既定の予定表フォルダーと、その予定表内にあるイベントにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="82fca-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="82fca-111">共有予定表内のイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="82fca-111">Get an event in the shared calendar</span></span>

<span data-ttu-id="82fca-112">Garth が共有している既定の予定表にある特定のイベントを取得できます。</span><span class="sxs-lookup"><span data-stu-id="82fca-112">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="82fca-113">正常に終了すると、HTTP 200 OK となり、Garth の既定の予定表から `{id}` によって識別される[イベント](/graph/api/resources/event?view=graph-rest-1.0) インスタンスが取得されます。</span><span class="sxs-lookup"><span data-stu-id="82fca-113">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="82fca-114">共有予定表内のすべてのイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="82fca-114">Get all the events in the shared calendar</span></span>

<span data-ttu-id="82fca-115">Garth が John と共有した既定の予定表にあるすべてのイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="82fca-115">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="82fca-116">正常に終了すると、HTTP 200 OK となり、Garth の既定の予定表にある[イベント](/graph/api/resources/event?view=graph-rest-1.0) インスタンスのコレクションが取得されます。</span><span class="sxs-lookup"><span data-stu-id="82fca-116">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="82fca-117">共有予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="82fca-117">Get the shared calendar</span></span>

<span data-ttu-id="82fca-118">Garth が John と共有した既定の予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="82fca-118">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="82fca-119">正常に終了すると、HTTP 200 OK となり、Garth の既定のフォルダーを表す [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) インスタンスが取得します。</span><span class="sxs-lookup"><span data-stu-id="82fca-119">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="82fca-120">Garth が John に対して、Garth の既定の予定表に対するさらに多くのアクセス権を委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="82fca-120">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="82fca-121">Garth が John と既定の予定表を共有しておらず、メールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="82fca-121">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="82fca-122">次のステップ</span><span class="sxs-lookup"><span data-stu-id="82fca-122">Next steps</span></span>

<span data-ttu-id="82fca-123">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="82fca-123">Find out more about:</span></span>

- [<span data-ttu-id="82fca-124">Outlook カレンダーと統合する理由</span><span class="sxs-lookup"><span data-stu-id="82fca-124">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="82fca-125">Microsoft Graph v1.0 の[予定表 API](/graph/api/resources/calendar?view=graph-rest-1.0)</span><span class="sxs-lookup"><span data-stu-id="82fca-125">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>