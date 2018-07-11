# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="9644d-101">Microsoft Graph に関する既知の問題</span><span class="sxs-lookup"><span data-stu-id="9644d-101">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="9644d-p101">この記事では、Microsoft Graph に関する既知の問題について説明します。最新の更新プログラムについては、「[Microsoft Graph の変更ログ](changelog.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9644d-p101">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="9644d-104">ユーザー</span><span class="sxs-lookup"><span data-stu-id="9644d-104">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="9644d-105">作成後にすぐにアクセスできない</span><span class="sxs-lookup"><span data-stu-id="9644d-105">No instant access after creation</span></span>

<span data-ttu-id="9644d-p102">ユーザーは、ユーザー エンティティの POST ですぐに作成できます。Office 365 サービスにアクセスするには、まず Office 365 ライセンスをユーザーに割り当てる必要があります。それでも、サービスが分散しているという性質上、Microsoft Graph API を介してこのユーザーがファイル、メッセージ、イベント エンティティを使用できるようになるまで 15 分かかる場合があります。この間、アプリには HTTP 404 エラー応答が送られてきます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p102">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="9644d-110">写真の制限</span><span class="sxs-lookup"><span data-stu-id="9644d-110">Photo restrictions</span></span>

<span data-ttu-id="9644d-p103">ユーザーのプロフィール写真の読み取りと更新は、ユーザーがメールボックスを持っている場合にのみ使用できます。さらに、以前 **thumbnailPhoto** プロパティを使用して (Office 365 統合 API のプレビュー、または Azure AD Graph、AD 接続同期を使用して) 保存*された*いかなる写真も[ユーザー](../api-reference/v1.0/resources/user.md) リソースの Microsoft Graph の**写真**プロパティを使用してアクセスできなくなります。写真の読み取りまたは更新が失敗すると、この例では次のエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="9644d-p103">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](../api-reference/v1.0/resources/user.md) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```


### <a name="using-delta-query"></a><span data-ttu-id="9644d-114">デルタ クエリの使用</span><span class="sxs-lookup"><span data-stu-id="9644d-114">Using delta query</span></span>

<span data-ttu-id="9644d-115">デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9644d-115">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="groups-and-microsoft-teams"></a><span data-ttu-id="9644d-116">グループと Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9644d-116">Groups and Microsoft Teams</span></span>

><span data-ttu-id="9644d-117">**注**: Microsoft Teams は現在プレビュー段階で、Microsoft Graph ベータ版のエンドポイントでのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="9644d-117">**Note** Microsoft Teams is currently in preview and is available only in the Microsoft Graph beta endpoint.</span></span>

### <a name="policy"></a><span data-ttu-id="9644d-118">ポリシー</span><span class="sxs-lookup"><span data-stu-id="9644d-118">Policy</span></span>

<span data-ttu-id="9644d-119">Microsoft Graph を使用して Office 365 グループを作成および名前付けすると、Outlook Web App で構成されたすべての Office 365 のグループ ポリシーがバイパスされます。</span><span class="sxs-lookup"><span data-stu-id="9644d-119">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="9644d-120">グループと Microsoft Teams のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="9644d-120">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="9644d-p104">Microsoft Graph では、グループと Microsoft Teams API にアクセスするために 2 つのアクセス許可 (*Group.Read.All* と *Group.ReadWrite.All*) を公開します。これらのアクセス許可は、管理者による同意が必要です (これがプレビューとの違いです)。将来的には、ユーザーが同意するグループとチームのための新しいアクセス許可を追加する予定です。</span><span class="sxs-lookup"><span data-stu-id="9644d-p104">Microsoft Graph exposes two permissions (*Group.Read.All* and *Group.ReadWrite.All*) for access to the APIs for groups and Microsoft Teams. These permissions must be consented to by an administrator (which is a change from preview).  In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="9644d-p105">また、コア グループの管理とマネージメントのための API だけが、委任されたアクセス許可とアプリ専用のアクセス許可によるアクセスをサポートします。グループ API の他のすべての機能は、委任されたアクセス許可のみサポートします。</span><span class="sxs-lookup"><span data-stu-id="9644d-p105">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="9644d-126">委任されたアクセス許可およびアプリ専用のアクセス許可をサポートするグループの機能の例:</span><span class="sxs-lookup"><span data-stu-id="9644d-126">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="9644d-127">グループの作成と削除</span><span class="sxs-lookup"><span data-stu-id="9644d-127">Creating and deleting groups</span></span>
* <span data-ttu-id="9644d-128">グループの管理とマネージメントに関するグループ プロパティの取得と更新</span><span class="sxs-lookup"><span data-stu-id="9644d-128">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="9644d-129">グループの[ディレクトリ設定](../api-reference/v1.0/resources/directoryobject.md)、型、同期</span><span class="sxs-lookup"><span data-stu-id="9644d-129">Group [directory settings](../api-reference/v1.0/resources/directoryobject.md), type, and synchronization</span></span>
* <span data-ttu-id="9644d-130">グループの所有者とメンバーシップ</span><span class="sxs-lookup"><span data-stu-id="9644d-130">Group owners and membership</span></span>

<span data-ttu-id="9644d-131">委任されたアクセス許可だけをサポートするグループ機能の例:</span><span class="sxs-lookup"><span data-stu-id="9644d-131">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="9644d-132">グループの会話、イベント、写真</span><span class="sxs-lookup"><span data-stu-id="9644d-132">Group conversations, events, photo</span></span>
* <span data-ttu-id="9644d-133">外部の送信者、承認済みまたは拒否された送信者、グループのサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="9644d-133">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="9644d-134">ユーザーのお気に入り、見えないカウント</span><span class="sxs-lookup"><span data-stu-id="9644d-134">User favorites and unseen count</span></span>
* <span data-ttu-id="9644d-135">Microsoft Teams チャンネルおよびチャット</span><span class="sxs-lookup"><span data-stu-id="9644d-135">Microsoft Teams channels and chats</span></span>

### <a name="teams-in-microsoft-teams-preview"></a><span data-ttu-id="9644d-136">Microsoft Teams のチーム (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="9644d-136">Teams in Microsoft Teams (preview)</span></span>

<span data-ttu-id="9644d-p106">Microsoft Teams と Office 365 グループは、[同じような機能を共有します](../api-reference/beta/resources/teams_api_overview.md)。グループ API はすべてチームで使用できますが、グループの作成 API は例外で、現在これを使ってのチーム作成はできません。将来的に、API リリースでこの機能がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p106">Microsoft Teams and Office 365 groups [share similar functionality](../api-reference/beta/resources/teams_api_overview.md). All group APIs can be used with teams, with the exception that the Create group API does not currently allow you to create a team.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-channels-preview"></a><span data-ttu-id="9644d-140">Microsoft Teams チャンネル (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="9644d-140">Microsoft Teams channels (preview)</span></span>

<span data-ttu-id="9644d-p107">現在のところ、チャンネルの読み込みと作成が可能ですが、更新と削除はできません。将来的に、API リリースでこの機能がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p107">Currently, you can read and create channels, but you cannot update or delete them.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-chat-threads-and-chat-messages-preview"></a><span data-ttu-id="9644d-143">Microsoft Teams チャット スレッドとチャット メッセージ (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="9644d-143">Microsoft Teams chat threads and chat messages (preview)</span></span>

<span data-ttu-id="9644d-p108">現時点では、チャンネルにチャット スレッドを作成できますが、既存のチャンネル スレッドを読み込む、または返信を付加することができません。また、チームまたはチャンネルの範囲外のユーザー間での読み取り、書き込みもできません。将来の API リリースでこの部分の機能がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p108">Currently, you can create chat threads in channels, but you cannot read existing chat threads or add replies to them. Also, you cannot read or write direct chats between users that are outside the scope of a team or channel.  Future API releases will add additional capabilities in this area.</span></span>

### <a name="microsoft-teams-users-list-of-joined-teams-preview"></a><span data-ttu-id="9644d-147">Microsoft Teams ユーザーが参加しているチームのリスト (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="9644d-147">Microsoft Teams user's list of joined teams (preview)</span></span>

<span data-ttu-id="9644d-p109">現在、[ユーザーが参加しているチームの一覧表示](../api-reference/beta/api/user_list_joinedteams.md)は、呼び出し元に[代理人アクセス許可](permissions_reference.md)がある 'me' (自分) ユーザーでのみ機能します。今後のリリースでは、指定した任意のユーザー ID に対してこの操作がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p109">Currrently, [listing the teams a user has joined](../api-reference/beta/api/user_list_joinedteams.md) only works for the 'me' user for which the caller has [delegated permissions](permissions_reference.md).  Future releases will support this operation for any specified user ID.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="9644d-150">グループの投稿の添付ファイルの追加と取得</span><span class="sxs-lookup"><span data-stu-id="9644d-150">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="9644d-p110">現在のところ、グループの投稿への添付ファイルの[追加](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/post_post_attachments)、グループの投稿の添付ファイルの[一覧表示](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/post_list_attachments)と取得を行うと、"OData 要求がサポートされていません" というエラー メッセージが返されます。`/v1.0` と `/beta` の両方のバージョンに対する修正プログラムが準備されており、2016 年 1 月の終わりまでには一般に利用可能になると予測されます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p110">[Adding](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/post_post_attachments) attachments to group posts, [listing](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/post_list_attachments) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="9644d-153">allowExternalSenders プロパティの設定</span><span class="sxs-lookup"><span data-stu-id="9644d-153">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="9644d-154">現在、`/v1.0` と `/beta` の両方で、POST または PATCH 操作の際にグループの **allowExternalSenders** プロパティを設定できないという問題が発生しています。</span><span class="sxs-lookup"><span data-stu-id="9644d-154">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="9644d-155">デルタ クエリの使用</span><span class="sxs-lookup"><span data-stu-id="9644d-155">Using delta query</span></span>

<span data-ttu-id="9644d-156">デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9644d-156">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>


## <a name="bookings"></a><span data-ttu-id="9644d-157">予約</span><span class="sxs-lookup"><span data-stu-id="9644d-157">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="9644d-158">bookingBusinesses のクエリ時の ErrorExceededFindCountLimit</span><span class="sxs-lookup"><span data-stu-id="9644d-158">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="9644d-159">組織が複数のビジネスを予約しており、要求を発行するアカウントが管理者でない場合に、`bookingBusinesses` のリストを取得しようとすると、次のエラー コードのエラーになります:</span><span class="sxs-lookup"><span data-stu-id="9644d-159">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several booking businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="9644d-160">回避策としては、`query` パラメーターを含めることによって、要求から返されるビジネスのセットを制限できます。たとえば:</span><span class="sxs-lookup"><span data-stu-id="9644d-160">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a><span data-ttu-id="9644d-161">予定表</span><span class="sxs-lookup"><span data-stu-id="9644d-161">Calendars</span></span>

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="9644d-162">ユーザーのメールボックスに ICS ベースの予定表を追加してアクセスする</span><span class="sxs-lookup"><span data-stu-id="9644d-162">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="9644d-163">現在、インターネット予定表購読 (ICS) に基づく予定表の部分的なサポートがあります。</span><span class="sxs-lookup"><span data-stu-id="9644d-163">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="9644d-164">ユーザー インターフェイスを経由して ICS ベースの予定表をユーザーのメールボックスに追加できますが、Microsoft Graph API を経由してこれを行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="9644d-164">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="9644d-p111">[ユーザーの予定表の一覧表示](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_list_calendars)を行うと、ICS ベースの予定表を含む、ユーザーの既定の予定表のグループ、または指定した予定表のグループにある各[予定表](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/calendar)の**名前**、**色**、**ID** のプロパティを取得できます。予定表リソースの ICS URL を保存したり、アクセスしたりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="9644d-p111">[Listing the user's calendars](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_list_calendars) lets you get the **name**, **color** and **id** properties of each [calendar](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/calendar) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="9644d-167">また、ICS ベースの予定表の[イベントを一覧表示](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/calendar_list_events)することもできます。</span><span class="sxs-lookup"><span data-stu-id="9644d-167">You can also [list the events](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/calendar_list_events) of an ICS-based calendar.</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="9644d-168">共有された予定表にアクセスする</span><span class="sxs-lookup"><span data-stu-id="9644d-168">Accessing a shared calendar</span></span>

<span data-ttu-id="9644d-169">別のユーザーによって共有されている予定表で、次の操作によってイベントにアクセスするとします。</span><span class="sxs-lookup"><span data-stu-id="9644d-169">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="9644d-p112">エラー コード `ErrorInternalServerTransientError` で HTTP 500 を受け取る可能性があります。エラーが発生する理由は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9644d-p112">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="9644d-172">従来、予定表共有を実装するための 2 つの方法がありました。それらを区別するために、"古い" アプローチと "新しい" アプローチと呼びます。</span><span class="sxs-lookup"><span data-stu-id="9644d-172">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="9644d-173">新しいアプローチは、表示または編集のアクセス許可による予定表の共有に使用できますが、委任のアクセス許可には使用できません。</span><span class="sxs-lookup"><span data-stu-id="9644d-173">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="9644d-174">予定表が**新しい**アプローチによって共有されている場合のみ、予定表 REST API を使用して、共有された予定表を表示または編集できます。</span><span class="sxs-lookup"><span data-stu-id="9644d-174">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="9644d-175">予定表が**古い**アプローチによって共有されている場合、予定表 REST API を使用して、このような予定表を表示または編集することはできません。</span><span class="sxs-lookup"><span data-stu-id="9644d-175">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="9644d-176">予定表が表示または編集のアクセス許可で共有されていても、古いアプローチを使用している場合、エラーを回避して手動で予定表共有をアップグレードし、新しいアプローチを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="9644d-176">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="9644d-177">時間の経過とともに、Outlook では共有されているすべての予定表が、委任アクセス許可で共有されている予定表を含め、新しいアプローチを使用できるように自動的にアップグレードされます。</span><span class="sxs-lookup"><span data-stu-id="9644d-177">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="9644d-178">新しいアプローチを使用できるように共有されている予定表を手動でアップグレードするには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="9644d-178">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="9644d-179">受信者は、それまで共有されていた予定表を削除します。</span><span class="sxs-lookup"><span data-stu-id="9644d-179">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="9644d-180">予定表の所有者は、Outlook on the web、iOS 版 Outlook または Android 版 Outlook で予定表を再共有します。</span><span class="sxs-lookup"><span data-stu-id="9644d-180">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="9644d-p114">受信者は Outlook on the web を使用して共有された予定表を再度受け取ります。(まもなくその他の Outlook クライアントも使用可能になります)</span><span class="sxs-lookup"><span data-stu-id="9644d-p114">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="9644d-183">受信者は、新しいアプローチを使用して iOS 版 Outlook または Android 版 Outlook で共有されている予定表を表示可能にすることで、予定表が正しく再共有されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="9644d-183">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="9644d-p115">新しいアプローチで共有した予定表は、全く別の予定表のようにメールボックスで表示されます。共有された予定表では、予定表 REST API を使用して自分の予定表のようにイベントを表示または編集できます。次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="9644d-p115">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```


## <a name="contacts"></a><span data-ttu-id="9644d-187">連絡先</span><span class="sxs-lookup"><span data-stu-id="9644d-187">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="9644d-188">ベータ版でのみ利用可能な組織の連絡先</span><span class="sxs-lookup"><span data-stu-id="9644d-188">Organization contacts available in only beta</span></span>

<span data-ttu-id="9644d-p116">現在、個人用連絡先しかサポートされていません。組織の連絡先は現在 `/v1.0` でサポートされていませんが、`/beta` で参照できます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p116">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="9644d-191">既定の連絡先フォルダー</span><span class="sxs-lookup"><span data-stu-id="9644d-191">Default contacts folder</span></span>

<span data-ttu-id="9644d-192">`/v1.0` バージョンでは、`GET /me/contactFolders` にユーザーの既定の連絡先フォルダーは含まれません。</span><span class="sxs-lookup"><span data-stu-id="9644d-192">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="9644d-p117">修正プログラムが用意される予定です。それまでは、回避策として次の[連絡先一覧表示](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_list_contacts)クエリと **parentFolderId** プロパティを使用して、既定の連絡先フォルダーのフォルダー ID を取得できます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p117">A fix will be made available. Meanwhile, you can use the following [list contacts](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/user_list_contacts) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="9644d-195">上記のクエリで、</span><span class="sxs-lookup"><span data-stu-id="9644d-195">In the above query:</span></span>

1. <span data-ttu-id="9644d-196">`/me/contacts?$top=1` は既定の連絡先フォルダーの[連絡先](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/contact)のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="9644d-196">`/me/contacts?$top=1` gets the properties of a [contact](http://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/contact) in the default contacts folder.</span></span>
2. <span data-ttu-id="9644d-197">`&$select=parentFolderId` を追加すると、連絡先の **parentFolderId** プロパティ (既定の連絡先フォルダーの ID) のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="9644d-197">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="9644d-198">ベータ版の連絡先フォルダーから連絡先にアクセスする</span><span class="sxs-lookup"><span data-stu-id="9644d-198">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="9644d-199">以下の 2 つのシナリオで示されているように、`/beta` バージョンでは、REST 要求 URL で親フォルダーを指定して[連絡先](../api-reference/beta/resources/contact.md)にアクセスすることができないという問題が発生しています。</span><span class="sxs-lookup"><span data-stu-id="9644d-199">In the `/beta` version, there is currently an issue that prevents accessing a [contact](../api-reference/beta/resources/contact.md) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="9644d-200">ユーザーの最上位レベル [contactFolder](../api-reference/beta/resources/contactfolder.md) から連絡先にアクセスする。</span><span class="sxs-lookup"><span data-stu-id="9644d-200">Accessing a contact from a top level [contactFolder](../api-reference/beta/resources/contactfolder.md) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="9644d-p118">**contactFolder** の子フォルダーに含まれている連絡先にアクセスする。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p118">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="9644d-203">あるいは、以下に示すように、ID を指定するだけで連絡先を[取得](../api-reference/beta/api/contact_get.md)することもできます。これは、`/beta` バージョンの GET /contacts が、ユーザーのメールボックス内のすべての連絡先に適用されるためです。</span><span class="sxs-lookup"><span data-stu-id="9644d-203">As an alternative, you can simply [get](../api-reference/beta/api/contact_get.md) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="9644d-204">メッセージ</span><span class="sxs-lookup"><span data-stu-id="9644d-204">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="9644d-205">下書きを作成するためのコメント パラメーター</span><span class="sxs-lookup"><span data-stu-id="9644d-205">The comment parameter for creating a draft</span></span>

<span data-ttu-id="9644d-206">返信または転送用の下書きを作成するための**コメント** パラメーター ([createReply](../api-reference/v1.0/api/message_createreply.md)、[createReplyAll](../api-reference/v1.0/api/message_createreplyall.md)、[createForward](../api-reference/v1.0/api/message_createforward.md)) は、結果メッセージの下書き本文の一部にはなりません。</span><span class="sxs-lookup"><span data-stu-id="9644d-206">The **comment** parameter for creating a reply or forward draft ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) does not become part of the body of the resultant message draft.</span></span>


## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="9644d-207">ドライブ、ファイルおよびコンテンツのストリーミング</span><span class="sxs-lookup"><span data-stu-id="9644d-207">Drives, files and content streaming</span></span>

* <span data-ttu-id="9644d-208">ユーザーが自分の個人用サイトにブラウザーでアクセスする前に、Microsoft Graph でユーザーの個人ドライブに初めてアクセスした場合、401 応答になります。</span><span class="sxs-lookup"><span data-stu-id="9644d-208">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="9644d-209">クエリ パラメーターの制限事項</span><span class="sxs-lookup"><span data-stu-id="9644d-209">Query parameter limitations</span></span>

* <span data-ttu-id="9644d-210">複数の名前空間はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9644d-210">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="9644d-211">`$ref` の GET とキャストはユーザー、グループ、デバイス、サービス プリンシパル、アプリケーションではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9644d-211">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="9644d-p119">`@odata.bind` はサポートされていません。つまり、開発者は `Accepted` や `RejectedSenders` を適切にグループに設定することができません。</span><span class="sxs-lookup"><span data-stu-id="9644d-p119">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="9644d-214">`@odata.id` は最低限のメタデータを使用する場合、非包含構造のナビゲーション (メッセージなど) には存在しません。</span><span class="sxs-lookup"><span data-stu-id="9644d-214">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="9644d-215">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="9644d-215">`$expand`:</span></span>
  * <span data-ttu-id="9644d-216">`nextLink` はサポートされていません</span><span class="sxs-lookup"><span data-stu-id="9644d-216">No support for `nextLink`</span></span>
  * <span data-ttu-id="9644d-217">1 レベルを超える展開はサポートされていません</span><span class="sxs-lookup"><span data-stu-id="9644d-217">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="9644d-218">余分なパラメーターはサポートされていません (`$filter`、`$select`)</span><span class="sxs-lookup"><span data-stu-id="9644d-218">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="9644d-219">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="9644d-219">`$filter`:</span></span>
  * <span data-ttu-id="9644d-220">`/attachments` エンドポイントは、フィルターをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="9644d-220">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="9644d-221">存在する場合、`$filter` パラメーターは無視されます。</span><span class="sxs-lookup"><span data-stu-id="9644d-221">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="9644d-222">ワークロード間でのフィルターはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9644d-222">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="9644d-223">`$search`:</span><span class="sxs-lookup"><span data-stu-id="9644d-223">`$search`:</span></span>
  * <span data-ttu-id="9644d-224">フルテキスト検索はメッセージなどのエンティティのサブセットに対してのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="9644d-224">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="9644d-225">ワークロード間での検索はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9644d-225">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="9644d-226">デルタ クエリ</span><span class="sxs-lookup"><span data-stu-id="9644d-226">Delta query</span></span>

* <span data-ttu-id="9644d-227">リレーションシップの追跡では、誤った OData コンテキストが返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9644d-227">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="9644d-228">スキーマ拡張情報 (レガシー) は $select ステートメントをつけては返されず、$select なしで返されます。</span><span class="sxs-lookup"><span data-stu-id="9644d-228">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="9644d-229">クライアントはオープン拡張機能または登録済みスキーマ拡張機能の変更を追跡できません。</span><span class="sxs-lookup"><span data-stu-id="9644d-229">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="9644d-230">application API と servicePrincipal API の変更</span><span class="sxs-lookup"><span data-stu-id="9644d-230">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="9644d-p121">現在開発中の [application](../api-reference/beta/resources/application.md) エンティティおよび [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) エンティティに対して変更点があります。現在の制限事項と開発中の API の機能の概要を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9644d-p121">There are changes to the [application](../api-reference/beta/resources/application.md) and [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="9644d-233">現在の制限事項:</span><span class="sxs-lookup"><span data-stu-id="9644d-233">Current limitations:</span></span>

* <span data-ttu-id="9644d-234">一部のアプリケーション プロパティ (appRoles、addIns など) は、すべての変更が完了するまで利用できません。</span><span class="sxs-lookup"><span data-stu-id="9644d-234">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="9644d-235">登録できるのは、マルチ テナント アプリだけです。</span><span class="sxs-lookup"><span data-stu-id="9644d-235">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="9644d-236">アプリの更新は、初期ベータ更新後に登録されたアプリに限定されます。</span><span class="sxs-lookup"><span data-stu-id="9644d-236">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="9644d-237">Azure Active Directory ユーザーは、アプリの登録と所有者の追加を行えます。</span><span class="sxs-lookup"><span data-stu-id="9644d-237">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="9644d-238">OpenID Connect と OAuth プロトコルをサポートします。</span><span class="sxs-lookup"><span data-stu-id="9644d-238">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="9644d-239">アプリケーションへのポリシーの割り当てが失敗します。</span><span class="sxs-lookup"><span data-stu-id="9644d-239">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="9644d-240">アプリ ID を必要とする ownedObjects に対する操作 (たとえば、users/{id|userPrincipalName}/ownedObjects/{id}/...) が失敗します。</span><span class="sxs-lookup"><span data-stu-id="9644d-240">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="9644d-241">開発中:</span><span class="sxs-lookup"><span data-stu-id="9644d-241">In development:</span></span>

* <span data-ttu-id="9644d-242">単一テナント アプリを登録する機能。</span><span class="sxs-lookup"><span data-stu-id="9644d-242">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="9644d-243">servicePrincipal に対する更新。</span><span class="sxs-lookup"><span data-stu-id="9644d-243">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="9644d-244">更新されたモデルへの既存の Azure AD アプリへの移行。</span><span class="sxs-lookup"><span data-stu-id="9644d-244">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="9644d-245">appRoles、事前承認済みクライアント、オプションのクレーム、グループ メンバーシップのクレーム、ブランド化のサポート。</span><span class="sxs-lookup"><span data-stu-id="9644d-245">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="9644d-246">Microsoft アカウント (MSA) ユーザーによるアプリの登録。</span><span class="sxs-lookup"><span data-stu-id="9644d-246">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="9644d-247">SAML および WsFed プロトコルのサポート。</span><span class="sxs-lookup"><span data-stu-id="9644d-247">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="9644d-248">拡張機能</span><span class="sxs-lookup"><span data-stu-id="9644d-248">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="9644d-249">変更履歴はサポートされていません</span><span class="sxs-lookup"><span data-stu-id="9644d-249">Change tracking is not supported</span></span>

<span data-ttu-id="9644d-250">変更の追跡 (デルタ クエリ) はオープン拡張機能またはスキーマ拡張機能のプロパティではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9644d-250">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="9644d-251">リソースとオープン拡張機能の同時作成</span><span class="sxs-lookup"><span data-stu-id="9644d-251">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="9644d-p122">**管理単位**、**デバイス**、**グループ**、**組織**、または**ユーザー**のインスタンスを作成するのと同時に、オープン拡張機能を指定することはできません。最初にインスタンスを作成し、次にそのインスタンスの後続の ``POST`` 要求でオープン拡張機能データを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9644d-p122">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="9644d-254">リソースのインスタンスを作成し、同時にスキーマ拡張機能データを追加します。</span><span class="sxs-lookup"><span data-stu-id="9644d-254">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="9644d-255">**連絡先**、**イベント**、**メッセージ**、**投稿**のインスタンスを作成する場合と同じ操作では、スキーマ拡張機能を指定できません。</span><span class="sxs-lookup"><span data-stu-id="9644d-255">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="9644d-256">リソースのインスタンスを作成してから、そのインスタンスに`PATCH` 操作を行い、スキーマ拡張機能とカスタム データを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9644d-256">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="9644d-257">スキーマ拡張機能のプロパティ値はリソースのインスタンスごとに 100 に制限されています。</span><span class="sxs-lookup"><span data-stu-id="9644d-257">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="9644d-258">現在、**デバイス**、**グループ**、**ユーザー**などのディレクトリ リソースでは、1 つのリソース インスタンスで設定可能なスキーマ拡張機能のプロパティ値の合計数が 100 に制限されています。</span><span class="sxs-lookup"><span data-stu-id="9644d-258">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="9644d-259">スキーマ拡張プロパティによるフィルター処理はすべてのエンティティ タイプでサポートされているわけではありません</span><span class="sxs-lookup"><span data-stu-id="9644d-259">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="9644d-260">スキーマ拡張プロパティによるフィルター処理 (`$filter` 式を使用する) は、Outlook エンティティ タイプ - **contact**、**event**、**message**、または **post** ではサポートされません。</span><span class="sxs-lookup"><span data-stu-id="9644d-260">Filtering on schema extension properties (using the `$filter` expresssion) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="9644d-261">JSON バッチ処理</span><span class="sxs-lookup"><span data-stu-id="9644d-261">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="9644d-262">入れ子状のバッチ不可</span><span class="sxs-lookup"><span data-stu-id="9644d-262">No nested batch</span></span>

<span data-ttu-id="9644d-263">JSON のバッチ要求には、入れ子になったバッチは一切含めることはできません。</span><span class="sxs-lookup"><span data-stu-id="9644d-263">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="9644d-264">個々の要求はすべて同期要求とします。</span><span class="sxs-lookup"><span data-stu-id="9644d-264">All individual requests must be synchronous</span></span>

<span data-ttu-id="9644d-p124">バッチ要求に含まれるすべての要求は同期して実行する必要があります。存在する場合、`respond-async` の設定は無視されます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p124">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="9644d-267">トランザクション未対応</span><span class="sxs-lookup"><span data-stu-id="9644d-267">No transactions</span></span>

<span data-ttu-id="9644d-p125">Microsoft Graph は現段階では個々の要求のトランザクション処理をサポートしていません。個々の要求で `atomicityGroup` プロパティを指定しても無視されます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p125">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="9644d-270">URI は相対 URI である必要があります。</span><span class="sxs-lookup"><span data-stu-id="9644d-270">URIs must be relative</span></span>

<span data-ttu-id="9644d-p126">バッチ要求では、必ず相対 URI を指定してください。Microsoft Graph はバッチ要求の URL に含まれているバージョン エンドポイントを使い、これらを絶対 URL に変換します。</span><span class="sxs-lookup"><span data-stu-id="9644d-p126">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="9644d-273">バッチ サイズの制限</span><span class="sxs-lookup"><span data-stu-id="9644d-273">Limit on batch size</span></span>

<span data-ttu-id="9644d-274">現段階では、JSON バッチ要求は 20 個までの個別要求に限られています。</span><span class="sxs-lookup"><span data-stu-id="9644d-274">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="9644d-275">簡略化された依存関係</span><span class="sxs-lookup"><span data-stu-id="9644d-275">Simplified dependencies</span></span>

<span data-ttu-id="9644d-p127">個々の要求は、他の個々の要求に依存することがあります。現在、各要求は他の要求一つだけに依存でき、以下のパターンのどれかにあてはまることが必要です。</span><span class="sxs-lookup"><span data-stu-id="9644d-p127">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="9644d-278">並行:依存する要求が `dependsOn` プロパティに指定されていない場合。</span><span class="sxs-lookup"><span data-stu-id="9644d-278">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="9644d-279">直列:個々の要求のすべてが前の個々の要求に依存する場合。</span><span class="sxs-lookup"><span data-stu-id="9644d-279">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="9644d-280">同列:`dependsOn` プロパティに依存を示した個々の要求のすべてが同じ依存を指定している場合。</span><span class="sxs-lookup"><span data-stu-id="9644d-280">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="9644d-281">JSON バッチ処理が完成に近づくにつれて、これらの制限は削除されます。</span><span class="sxs-lookup"><span data-stu-id="9644d-281">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="9644d-282">クラウド ソリューション プロバイダー アプリ</span><span class="sxs-lookup"><span data-stu-id="9644d-282">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="9644d-283">CSP アプリは Azure AD エンドポイントを使用する必要がある</span><span class="sxs-lookup"><span data-stu-id="9644d-283">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="9644d-p128">クラウド ソリューション プロバイダー (CSP) のアプリケーションは、パートナー管理の顧客から Microsoft Graph を正常に呼び出すには、Azure AD (v1) のエンドポイントからトークンを取得する必要があります。現時点では、新しい Azure AD バージョン 2.0 エンドポイントからのトークン取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9644d-p128">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="9644d-286">CSP アプリの事前同意が一部の顧客テナントで機能しない</span><span class="sxs-lookup"><span data-stu-id="9644d-286">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="9644d-287">状況によっては、CSP アプリの事前同意が一部の顧客テナントで機能しない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9644d-287">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="9644d-288">代理アクセス許可を使用するアプリでは、新しい顧客テナントで初めてアプリを使用すると、サインイン後に次のエラーを受け取る可能性があります。`AADSTS50000: There was an error issuing a token`。</span><span class="sxs-lookup"><span data-stu-id="9644d-288">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="9644d-289">アプリケーションのアクセス許可を使用するアプリでは、アプリはトークンを取得できますが、Microsoft Graph を呼び出すときに予期せずにアクセス拒否メッセージを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="9644d-289">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="9644d-290">事前同意をすべての顧客テナントで機能させるために、できるだけ早くこの問題を解決するべく取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="9644d-290">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="9644d-291">それまでの間、開発とテストのブロックを解除するために次の回避策を取ってください。</span><span class="sxs-lookup"><span data-stu-id="9644d-291">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="9644d-p129">**注:** これは永続的なソリューションではなく、開発のブロックを解除するためのものです。前述の問題が解決されたら、この回避策は必要なくなります。解決された後にこの回避策を元に戻す必要はありません。</span><span class="sxs-lookup"><span data-stu-id="9644d-p129">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="9644d-p130">Azure AD v2 PowerShell セッションを開き、サインイン ウィンドウに、管理者資格情報を入力して `customer` テナントに接続します。Azure AD PowerShell V2 は、[ここ](https://www.powershellgallery.com/packages/AzureAD)からダウンロードし、インストールできます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p130">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="9644d-297">Microsoft Graph サービス プリンシパルを作成します。</span><span class="sxs-lookup"><span data-stu-id="9644d-297">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="9644d-298">Office 365 REST と Azure AD Graph API でのみ使用可能な機能</span><span class="sxs-lookup"><span data-stu-id="9644d-298">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="9644d-p131">Microsoft Graph では一部の機能はまだ利用できません。探している機能が表示されない場合は、エンドポイント固有の [Office 365 REST API](https://msdn.microsoft.com/ja-JP/office/office365/api/api-catalog) を使用することができます。Azure Active Directory において、Azure AD と Graph API を介してのみ使用可能な機能については、[Microsoft Graph または Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) のブログの投稿を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9644d-p131">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/ja-JP/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

## <a name="feedback"></a><span data-ttu-id="9644d-302">フィードバック</span><span class="sxs-lookup"><span data-stu-id="9644d-302">Feedback</span></span>

> <span data-ttu-id="9644d-p132">お客様からのフィードバックを重視しています。[スタック オーバーフロー](http://stackoverflow.com/questions/tagged/microsoftgraph)でご連絡いただけます。</span><span class="sxs-lookup"><span data-stu-id="9644d-p132">Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph).</span></span>
