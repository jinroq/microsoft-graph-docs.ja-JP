# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="4a016-101">共有または委任された予定表に Outlook のイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="4a016-101">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="4a016-102">Outlook では、お客様は他のユーザーと予定表を共有し、これらのユーザーは共有した予定表のイベントを表示または変更することができます。</span><span class="sxs-lookup"><span data-stu-id="4a016-102">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="4a016-103">また、お客様は、権限を委任し、会議出席依頼の受信や応答、または予定表のアイテムの作成や変更を代行してもらうこともできます。</span><span class="sxs-lookup"><span data-stu-id="4a016-103">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="4a016-104">Microsoft Graph では、他のユーザーと共有する予定表のイベントを取得したり、共有予定表自体を取得したりする機能がプログラムとしてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="4a016-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="4a016-105">サポートは、委任された予定表にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="4a016-105">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="4a016-106">たとえば、Garth が予定表を John と共有している場合、John は読み取りアクセスが可能になります。</span><span class="sxs-lookup"><span data-stu-id="4a016-106">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="4a016-107">John がアプリにサインインし、委任されたアクセス許可 (Calendars.Read.Shared または Calendars.ReadWrite.Share) を提供した場合、アプリでは、下記のようにして Garth の規定の予定表とその予定表にあるイベントにアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="4a016-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="4a016-108">共有予定表のイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="4a016-108">Get an event in the shared calendar</span></span>

<span data-ttu-id="4a016-109">Garth が共有している既定の予定表にある、特定のイベントを取得できます。</span><span class="sxs-lookup"><span data-stu-id="4a016-109">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="4a016-110">正常に終了すると、HTTP 200 OK となり、[ Garth](../api-reference/v1.0/resources/event.md)  の規定の予定表から `{id}` によって識別されるイベント インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="4a016-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/event.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="4a016-111">共有予定表のすべてのイベントを取得する</span><span class="sxs-lookup"><span data-stu-id="4a016-111">Get all the events in the shared calendar</span></span>

<span data-ttu-id="4a016-112">Garth が John  と共有している既定の予定表にあるすべてのイベントを取得します。</span><span class="sxs-lookup"><span data-stu-id="4a016-112">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="4a016-113">正常に終了すると、HTTP 200 OK となり、Garth の規定の予定表の [event](../api-reference/v1.0/resources/event.md) インスタンスのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4a016-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/event.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="4a016-114">共有予定表を取得する</span><span class="sxs-lookup"><span data-stu-id="4a016-114">Get the shared folder</span></span>

<span data-ttu-id="4a016-115">Garth が John と共有している既定の予定表を取得します。</span><span class="sxs-lookup"><span data-stu-id="4a016-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="4a016-116">正常に終了すると、HTTP 200 OK となり、Garth の規定のフォルダーを表す [calendar](../api-reference/v1.0/resources/calendar.md) インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="4a016-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/calendar.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="4a016-117">Garth が、自分の規定の予定表へのアクセス権をさらに多く John  に委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。</span><span class="sxs-lookup"><span data-stu-id="4a016-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="4a016-118">Garth が John と規定の予定表を共有していない、またはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="4a016-118">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="4a016-119">次の手順</span><span class="sxs-lookup"><span data-stu-id="4a016-119">Next steps</span></span>

<span data-ttu-id="4a016-120">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="4a016-120">Find out more about:</span></span>

- [<span data-ttu-id="4a016-121">Outlook カレンダーと統合する理由</span><span class="sxs-lookup"><span data-stu-id="4a016-121">Why integrate with Outlook calendar?</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="4a016-122">Microsoft Graph v1.0 の[カレンダー API](../api-reference/v1.0/resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="4a016-122">The [calendar API](../api-reference/v1.0/resources/calendar.md) in Microsoft Graph v1.0.</span></span>