---
title: Microsoft Graph に関する既知の問題
description: この記事では、Microsoft Graph に関する既知の問題について説明します。最新の更新プログラムについては、「Microsoft Graph の変更ログ」を参照してください。
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 65a38e8852c878811d609b56b0f7f0ad1d4e73ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820224"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="14ea3-104">Microsoft Graph に関する既知の問題</span><span class="sxs-lookup"><span data-stu-id="14ea3-104">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="14ea3-p102">この記事では、Microsoft Graph に関する既知の問題について説明します。最新の更新プログラムについては、「[Microsoft Graph の変更ログ](changelog.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p102">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="14ea3-107">ユーザー</span><span class="sxs-lookup"><span data-stu-id="14ea3-107">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="14ea3-108">作成後にすぐにアクセスできない</span><span class="sxs-lookup"><span data-stu-id="14ea3-108">No instant access after creation</span></span>

<span data-ttu-id="14ea3-p103">ユーザーは、ユーザー エンティティの POST ですぐに作成できます。Office 365 サービスにアクセスするには、まず Office 365 ライセンスをユーザーに割り当てる必要があります。それでも、サービスが分散しているという性質上、Microsoft Graph API を介してこのユーザーがファイル、メッセージ、イベント エンティティを使用できるようになるまで 15 分かかる場合があります。この間、アプリには HTTP 404 エラー応答が送られてきます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p103">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="14ea3-113">写真の制限</span><span class="sxs-lookup"><span data-stu-id="14ea3-113">Photo restrictions</span></span>

<span data-ttu-id="14ea3-p104">ユーザーのプロフィール写真の読み取りと更新は、ユーザーがメールボックスを持っている場合にのみ使用できます。さらに、以前 **thumbnailPhoto** プロパティを使用して (Office 365 統合 API のプレビュー、または Azure AD Graph、AD 接続同期を使用して) 保存*された*いかなる写真も[ユーザー](/graph/api/resources/user?view=graph-rest-1.0) リソースの Microsoft Graph の**写真**プロパティを使用してアクセスできなくなります。写真の読み取りまたは更新が失敗すると、この例では次のエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p104">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

### <a name="using-delta-query"></a><span data-ttu-id="14ea3-117">デルタ クエリの使用</span><span class="sxs-lookup"><span data-stu-id="14ea3-117">Using delta query</span></span>

<span data-ttu-id="14ea3-118">デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14ea3-118">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="microsoft-teams"></a><span data-ttu-id="14ea3-119">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="14ea3-119">Microsoft Teams</span></span>

### <a name="create-chat-thread-api"></a><span data-ttu-id="14ea3-120">チャット スレッドの作成 API</span><span class="sxs-lookup"><span data-stu-id="14ea3-120">Create chat thread API</span></span>

<span data-ttu-id="14ea3-121">[チャット スレッドを作成する](/graph/api/channel-post-chatthreads?view=graph-rest-beta)現在の API が、[チャネル メッセージのリスト作成](/graph/api/channel-list-messages?view=graph-rest-beta)のスキーマと整合性のある、より充実した API に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-121">The current API to [create a chat thread](/graph/api/channel-post-chatthreads?view=graph-rest-beta) will be replaced with a richer API that is consistent with the schema for [listing channel messages](/graph/api/channel-list-messages?view=graph-rest-beta).</span></span>

### <a name="graph-explorer-and-global-admins"></a><span data-ttu-id="14ea3-122">Graph エクスプローラーと全体管理者</span><span class="sxs-lookup"><span data-stu-id="14ea3-122">Graph Explorer and global admins</span></span>

<span data-ttu-id="14ea3-123">現在の Graph エクスプローラーでは、全体管理者は自分が所有者やメンバーではないチームを操作することができます。ただし、現在のユーザーがチームのメンバーや所有者ではない場合に、他のアプリが同じ API 呼び出しを行おうとすると、そのアプリは失敗します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-123">Currently, Graph Explorer allows global admins to manipulate teams they are not an owner or member of, but other apps attempting to make the same API calls will fail if the current user is not a member or owner of the team.</span></span>

### <a name="get-teams-and-post-teams-are-not-supported"></a><span data-ttu-id="14ea3-124">GET /teams と POST /teams はサポート対象外</span><span class="sxs-lookup"><span data-stu-id="14ea3-124">GET /teams and POST /teams are not supported</span></span>

<span data-ttu-id="14ea3-125">チームのリストを取得するには、「[すべてのチームのリスト](teams-list-all-teams.md)」と「[自分のチームのリスト](/graph/api/user-list-joinedteams?view=graph-rest-1.0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14ea3-125">See [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) to get a list of teams.</span></span>
<span data-ttu-id="14ea3-126">チームを作成するには、「[チームの作成](/graph/api/team-put-teams?view=graph-rest-1.0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14ea3-126">See [create team](/graph/api/team-put-teams?view=graph-rest-1.0) for creating teams.</span></span>

### <a name="missing-teams-in-list-all-teams"></a><span data-ttu-id="14ea3-127">すべてのチームのリストに含まれないチームがある</span><span class="sxs-lookup"><span data-stu-id="14ea3-127">Missing teams in list all teams</span></span>

<span data-ttu-id="14ea3-128">過去に作成され、Microsoft Teams ユーザーに最近使用されていないチームの一部は、[すべてのチームのリスト](teams-list-all-teams.md)に含まれません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-128">Some teams that were created in the past but haven't been used recently by a Microsoft Teams user aren't listed by [list all teams](teams-list-all-teams.md).</span></span>
<span data-ttu-id="14ea3-129">新しいチームはリストに含まれます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-129">New teams will be listed.</span></span>
<span data-ttu-id="14ea3-130">古いチームの一部には、**resourceProvisioningOptions** プロパティが存在しないものがあります。このプロパティには "Team" が含まれており、新しく作成され、Microsoft Teams 内でアクセスされたチームには設定されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-130">Certain old teams don't have a **resourceProvisioningOptions** property that contains "Team", which is set on newly created teams and teams that are visited in Microsoft Teams.</span></span>
<span data-ttu-id="14ea3-131">将来的には、Microsoft Teams で開かれたことのない既存のチームに対しても、**resourceProvisioningOptions** が設定される予定です。</span><span class="sxs-lookup"><span data-stu-id="14ea3-131">In the future, we will set **resourceProvisioningOptions** on existing teams that have not been opened in Microsoft Teams.</span></span>

## <a name="groups"></a><span data-ttu-id="14ea3-132">グループ</span><span class="sxs-lookup"><span data-stu-id="14ea3-132">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="14ea3-133">グループと Microsoft Teams のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="14ea3-133">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="14ea3-134">Microsoft Graph では、グループと Microsoft Teams API にアクセスするために 2 つのアクセス許可 ([*Group.Read.All*](permissions-reference.md#group-permissions) と [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) を公開します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-134">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="14ea3-135">これらのアクセス許可には、管理者による同意が必要です。</span><span class="sxs-lookup"><span data-stu-id="14ea3-135">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="14ea3-136">将来的には、ユーザーが同意するグループとチームのための新しいアクセス許可を追加する予定です。</span><span class="sxs-lookup"><span data-stu-id="14ea3-136">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="14ea3-p108">また、コア グループの管理とマネージメントのための API だけが、委任されたアクセス許可とアプリ専用のアクセス許可によるアクセスをサポートします。グループ API の他のすべての機能は、委任されたアクセス許可のみサポートします。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p108">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="14ea3-139">委任されたアクセス許可およびアプリ専用のアクセス許可をサポートするグループの機能の例:</span><span class="sxs-lookup"><span data-stu-id="14ea3-139">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="14ea3-140">グループの作成と削除</span><span class="sxs-lookup"><span data-stu-id="14ea3-140">Creating and deleting groups</span></span>
* <span data-ttu-id="14ea3-141">グループの管理とマネージメントに関するグループ プロパティの取得と更新</span><span class="sxs-lookup"><span data-stu-id="14ea3-141">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="14ea3-142">グループの[ディレクトリ設定](/graph/api/resources/directoryobject?view=graph-rest-1.0)、型、同期</span><span class="sxs-lookup"><span data-stu-id="14ea3-142">Group [directory settings](/graph/api/resources/directoryobject?view=graph-rest-1.0), type, and synchronization</span></span>
* <span data-ttu-id="14ea3-143">グループの所有者とメンバーシップ</span><span class="sxs-lookup"><span data-stu-id="14ea3-143">Group owners and membership</span></span>

<span data-ttu-id="14ea3-144">委任されたアクセス許可だけをサポートするグループ機能の例:</span><span class="sxs-lookup"><span data-stu-id="14ea3-144">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="14ea3-145">グループの会話、イベント、写真</span><span class="sxs-lookup"><span data-stu-id="14ea3-145">Group conversations, events, photo</span></span>
* <span data-ttu-id="14ea3-146">外部の送信者、承認済みまたは拒否された送信者、グループのサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="14ea3-146">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="14ea3-147">ユーザーのお気に入り、見えないカウント</span><span class="sxs-lookup"><span data-stu-id="14ea3-147">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="14ea3-148">ポリシー</span><span class="sxs-lookup"><span data-stu-id="14ea3-148">Policy</span></span>

<span data-ttu-id="14ea3-149">Microsoft Graph を使用して Office 365 グループを作成および名前付けすると、Outlook Web App で構成されたすべての Office 365 のグループ ポリシーがバイパスされます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-149">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="14ea3-150">グループの投稿の添付ファイルの追加と取得</span><span class="sxs-lookup"><span data-stu-id="14ea3-150">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="14ea3-p109">現在のところ、グループの投稿への添付ファイルの[追加](/graph/api/post-post-attachments?view=graph-rest-1.0)、グループの投稿の添付ファイルの[一覧表示](/graph/api/post-list-attachments?view=graph-rest-1.0)と取得を行うと、"OData 要求がサポートされていません" というエラー メッセージが返されます。`/v1.0` と `/beta` の両方のバージョンに対する修正プログラムが準備されており、2016 年 1 月の終わりまでには一般に利用可能になると予測されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p109">[Adding](/graph/api/post-post-attachments?view=graph-rest-1.0) attachments to group posts, [listing](/graph/api/post-list-attachments?view=graph-rest-1.0) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="14ea3-153">allowExternalSenders プロパティの設定</span><span class="sxs-lookup"><span data-stu-id="14ea3-153">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="14ea3-154">現在、`/v1.0` と `/beta` の両方で、POST または PATCH 操作の際にグループの **allowExternalSenders** プロパティを設定できないという問題が発生しています。</span><span class="sxs-lookup"><span data-stu-id="14ea3-154">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="14ea3-155">デルタ クエリの使用</span><span class="sxs-lookup"><span data-stu-id="14ea3-155">Using delta query</span></span>

<span data-ttu-id="14ea3-156">デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14ea3-156">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="bookings"></a><span data-ttu-id="14ea3-157">予約</span><span class="sxs-lookup"><span data-stu-id="14ea3-157">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="14ea3-158">bookingBusinesses のクエリ時の ErrorExceededFindCountLimit</span><span class="sxs-lookup"><span data-stu-id="14ea3-158">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="14ea3-159">組織が複数のビジネスを予約しており、要求を発行するアカウントが管理者でない場合に、`bookingBusinesses` のリストを取得しようとすると、次のエラー コードのエラーになります:</span><span class="sxs-lookup"><span data-stu-id="14ea3-159">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="14ea3-160">回避策としては、`query` パラメーターを含めることによって、要求から返されるビジネスのセットを制限できます。たとえば:</span><span class="sxs-lookup"><span data-stu-id="14ea3-160">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a><span data-ttu-id="14ea3-161">予定表</span><span class="sxs-lookup"><span data-stu-id="14ea3-161">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="14ea3-162">共有された予定表にアクセスする</span><span class="sxs-lookup"><span data-stu-id="14ea3-162">Accessing a shared calendar</span></span>

<span data-ttu-id="14ea3-163">別のユーザーによって共有されている予定表で、次の操作によってイベントにアクセスするとします。</span><span class="sxs-lookup"><span data-stu-id="14ea3-163">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="14ea3-p110">エラー コード `ErrorInternalServerTransientError` で HTTP 500 を受け取る可能性があります。エラーが発生する理由は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p110">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="14ea3-166">従来、予定表共有を実装するための 2 つの方法がありました。それらを区別するために、"古い" アプローチと "新しい" アプローチと呼びます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-166">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="14ea3-167">新しいアプローチは、表示または編集のアクセス許可による予定表の共有に使用できますが、委任のアクセス許可には使用できません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-167">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="14ea3-168">予定表が**新しい**アプローチによって共有されている場合のみ、予定表 REST API を使用して、共有された予定表を表示または編集できます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-168">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="14ea3-169">予定表が**古い**アプローチによって共有されている場合、予定表 REST API を使用して、このような予定表を表示または編集することはできません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-169">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="14ea3-170">予定表が表示または編集のアクセス許可で共有されていても、古いアプローチを使用している場合、エラーを回避して手動で予定表共有をアップグレードし、新しいアプローチを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-170">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="14ea3-171">時間の経過とともに、Outlook では共有されているすべての予定表が、委任アクセス許可で共有されている予定表を含め、新しいアプローチを使用できるように自動的にアップグレードされます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-171">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="14ea3-172">新しいアプローチを使用できるように共有されている予定表を手動でアップグレードするには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-172">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="14ea3-173">受信者は、それまで共有されていた予定表を削除します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-173">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="14ea3-174">予定表の所有者は、Outlook on the web、iOS 版 Outlook または Android 版 Outlook で予定表を再共有します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-174">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="14ea3-p112">受信者は Outlook on the web を使用して共有された予定表を再度受け取ります。(まもなくその他の Outlook クライアントも使用可能になります)</span><span class="sxs-lookup"><span data-stu-id="14ea3-p112">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="14ea3-177">受信者は、新しいアプローチを使用して iOS 版 Outlook または Android 版 Outlook で共有されている予定表を表示可能にすることで、予定表が正しく再共有されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-177">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="14ea3-p113">新しいアプローチで共有した予定表は、全く別の予定表のようにメールボックスで表示されます。共有された予定表では、予定表 REST API を使用して自分の予定表のようにイベントを表示または編集できます。次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p113">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="14ea3-181">ユーザーのメールボックスに ICS ベースの予定表を追加してアクセスする</span><span class="sxs-lookup"><span data-stu-id="14ea3-181">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="14ea3-182">現在、インターネット予定表購読 (ICS) に基づく予定表の部分的なサポートがあります。</span><span class="sxs-lookup"><span data-stu-id="14ea3-182">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="14ea3-183">ユーザー インターフェイスを経由して ICS ベースの予定表をユーザーのメールボックスに追加できますが、Microsoft Graph API を経由してこれを行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-183">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="14ea3-p114">[ユーザーの予定表の一覧表示](/graph/api/user-list-calendars?view=graph-rest-1.0)を行うと、ICS ベースの予定表を含む、ユーザーの既定の予定表のグループ、または指定した予定表のグループにある各[予定表](/graph/api/resources/calendar?view=graph-rest-1.0)の**名前**、**色**、**ID** のプロパティを取得できます。予定表リソースの ICS URL を保存したり、アクセスしたりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p114">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="14ea3-186">また、ICS ベースの予定表の[イベントを一覧表示](/graph/api/calendar-list-events?view=graph-rest-1.0)することもできます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-186">You can also [list the events](/graph/api/calendar-list-events?view=graph-rest-1.0) of an ICS-based calendar.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="14ea3-187">Microsoft Teams 向けの onlineMeetingUrl プロパティのサポート</span><span class="sxs-lookup"><span data-stu-id="14ea3-187">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="14ea3-188">現時点では、Skype 会議 [event](/graph/api/resources/event?view=graph-rest-1.0) の **onlineMeetingUrl** プロパティは、オンライン会議の URL を示します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-188">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event?view=graph-rest-1.0) would indicate the online meeting URL.</span></span> <span data-ttu-id="14ea3-189">ただし、Microsoft Teams の会議イベントの onlineMeetingUrl プロパティは Null に設定します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-189">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

## <a name="calls-and-online-meetings"></a><span data-ttu-id="14ea3-190">通話とオンライン会議</span><span class="sxs-lookup"><span data-stu-id="14ea3-190">Calls and online meetings</span></span>

> <span data-ttu-id="14ea3-191">**注**: 通話とオンライン会議は現在プレビュー段階で、Microsoft Graph ベータ版のエンドポイントでのみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="14ea3-191">**Note** Calling and online meetings are currently in preview and are available only in the Microsoft Graph beta endpoint.</span></span>

- <span data-ttu-id="14ea3-192">ナビゲーション パス `/applications/{id}` はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-192">Navigation path `/applications/{id}` is not supported.</span></span> <span data-ttu-id="14ea3-193">グローバル アプリケーション ノードを経由したアプリケーションへの移動は、自分が所有者である場合でも、許可されていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-193">Navigating through the global applications node to the application, even your own, is not allowed.</span></span> <span data-ttu-id="14ea3-194">`/app` ナビゲーションのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="14ea3-194">Please use the `/app` navigation only.</span></span>

## <a name="contacts"></a><span data-ttu-id="14ea3-195">連絡先</span><span class="sxs-lookup"><span data-stu-id="14ea3-195">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="14ea3-196">ベータ版でのみ利用可能な組織の連絡先</span><span class="sxs-lookup"><span data-stu-id="14ea3-196">Organization contacts available in only beta</span></span>

<span data-ttu-id="14ea3-p117">現在、個人用連絡先しかサポートされていません。組織の連絡先は現在 `/v1.0` でサポートされていませんが、`/beta` で参照できます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p117">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="14ea3-199">既定の連絡先フォルダー</span><span class="sxs-lookup"><span data-stu-id="14ea3-199">Default contacts folder</span></span>

<span data-ttu-id="14ea3-200">`/v1.0` バージョンでは、`GET /me/contactFolders` にユーザーの既定の連絡先フォルダーは含まれません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-200">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="14ea3-p118">修正プログラムが用意される予定です。それまでは、回避策として次の[連絡先一覧表示](/graph/api/user-list-contacts?view=graph-rest-1.0)クエリと **parentFolderId** プロパティを使用して、既定の連絡先フォルダーのフォルダー ID を取得できます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p118">A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="14ea3-203">上記のクエリで、</span><span class="sxs-lookup"><span data-stu-id="14ea3-203">In the above query:</span></span>

1. <span data-ttu-id="14ea3-204">`/me/contacts?$top=1` は既定の連絡先フォルダーの[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-204">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact?view=graph-rest-1.0) in the default contacts folder.</span></span>
2. <span data-ttu-id="14ea3-205">`&$select=parentFolderId` を追加すると、連絡先の **parentFolderId** プロパティ (既定の連絡先フォルダーの ID) のみが返されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-205">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="14ea3-206">ベータ版の連絡先フォルダーから連絡先にアクセスする</span><span class="sxs-lookup"><span data-stu-id="14ea3-206">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="14ea3-207">以下の 2 つのシナリオで示されているように、`/beta` バージョンでは、REST 要求 URL で親フォルダーを指定して[連絡先](/graph/api/resources/contact?view=graph-rest-beta)にアクセスすることができないという問題が発生しています。</span><span class="sxs-lookup"><span data-stu-id="14ea3-207">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="14ea3-208">ユーザーの最上位レベル [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) から連絡先にアクセスする。</span><span class="sxs-lookup"><span data-stu-id="14ea3-208">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="14ea3-p119">**contactFolder** の子フォルダーに含まれている連絡先にアクセスする。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p119">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="14ea3-211">あるいは、以下に示すように、ID を指定するだけで連絡先を[取得](/graph/api/contact-get?view=graph-rest-beta)することもできます。これは、`/beta` バージョンの GET /contacts が、ユーザーのメールボックス内のすべての連絡先に適用されるためです。</span><span class="sxs-lookup"><span data-stu-id="14ea3-211">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="14ea3-212">メッセージ</span><span class="sxs-lookup"><span data-stu-id="14ea3-212">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="14ea3-213">下書きを作成するためのコメント パラメーター</span><span class="sxs-lookup"><span data-stu-id="14ea3-213">The comment parameter for creating a draft</span></span>

<span data-ttu-id="14ea3-214">返信または転送用の下書きを作成するための**コメント** パラメーター ([createReply](/graph/api/message-createreply?view=graph-rest-1.0)、[createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0)、[createForward](/graph/api/message-createforward?view=graph-rest-1.0)) は、結果メッセージの下書き本文の一部にはなりません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-214">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="14ea3-215">Microsoft Teams でのメッセージ返信チャットの GET</span><span class="sxs-lookup"><span data-stu-id="14ea3-215">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="14ea3-216">V1 とベータ版の両方のエンドポイントで、`GET /users/id/messages` の応答には、チームまたはチャネルの範囲外で行われたユーザーの Microsoft Teams チャットが含まれています。</span><span class="sxs-lookup"><span data-stu-id="14ea3-216">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="14ea3-217">これらのチャット メッセージの件名は「IM」です。</span><span class="sxs-lookup"><span data-stu-id="14ea3-217">These chat messages have "IM" as their subject.</span></span>


## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="14ea3-218">ドライブ、ファイルおよびコンテンツのストリーミング</span><span class="sxs-lookup"><span data-stu-id="14ea3-218">Drives, files and content streaming</span></span>

* <span data-ttu-id="14ea3-219">ユーザーが自分の個人用サイトにブラウザーでアクセスする前に、Microsoft Graph でユーザーの個人ドライブに初めてアクセスした場合、401 応答になります。</span><span class="sxs-lookup"><span data-stu-id="14ea3-219">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="14ea3-220">クエリ パラメーターの制限事項</span><span class="sxs-lookup"><span data-stu-id="14ea3-220">Query parameter limitations</span></span>

* <span data-ttu-id="14ea3-221">複数の名前空間はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-221">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="14ea3-222">`$ref` の GET とキャストはユーザー、グループ、デバイス、サービス プリンシパル、アプリケーションではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-222">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="14ea3-p121">`@odata.bind` はサポートされていません。つまり、開発者は `Accepted` や `RejectedSenders` を適切にグループに設定することができません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p121">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="14ea3-225">`@odata.id` は最低限のメタデータを使用する場合、非包含構造のナビゲーション (メッセージなど) には存在しません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-225">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="14ea3-226">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="14ea3-226">`$expand`:</span></span>
  * <span data-ttu-id="14ea3-227">`nextLink` はサポートされていません</span><span class="sxs-lookup"><span data-stu-id="14ea3-227">No support for `nextLink`</span></span>
  * <span data-ttu-id="14ea3-228">1 レベルを超える展開はサポートされていません</span><span class="sxs-lookup"><span data-stu-id="14ea3-228">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="14ea3-229">余分なパラメーターはサポートされていません (`$filter`、`$select`)</span><span class="sxs-lookup"><span data-stu-id="14ea3-229">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="14ea3-230">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="14ea3-230">`$filter`:</span></span>
  * <span data-ttu-id="14ea3-231">`/attachments` エンドポイントは、フィルターをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-231">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="14ea3-232">存在する場合、`$filter` パラメーターは無視されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-232">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="14ea3-233">ワークロード間でのフィルターはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-233">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="14ea3-234">`$search`:</span><span class="sxs-lookup"><span data-stu-id="14ea3-234">`$search`:</span></span>
  * <span data-ttu-id="14ea3-235">フルテキスト検索はメッセージなどのエンティティのサブセットに対してのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-235">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="14ea3-236">ワークロード間での検索はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-236">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="14ea3-237">デルタ クエリ</span><span class="sxs-lookup"><span data-stu-id="14ea3-237">Delta query</span></span>

* <span data-ttu-id="14ea3-238">リレーションシップの追跡では、誤った OData コンテキストが返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14ea3-238">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="14ea3-239">スキーマ拡張情報 (レガシー) は $select ステートメントをつけては返されず、$select なしで返されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-239">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="14ea3-240">クライアントはオープン拡張機能または登録済みスキーマ拡張機能の変更を追跡できません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-240">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="14ea3-241">application API と servicePrincipal API の変更</span><span class="sxs-lookup"><span data-stu-id="14ea3-241">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="14ea3-p123">現在開発中の [application](/graph/api/resources/application?view=graph-rest-beta) エンティティおよび [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) エンティティに対して変更点があります。現在の制限事項と開発中の API の機能の概要を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p123">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="14ea3-244">現在の制限事項:</span><span class="sxs-lookup"><span data-stu-id="14ea3-244">Current limitations:</span></span>

* <span data-ttu-id="14ea3-245">一部のアプリケーション プロパティ (appRoles、addIns など) は、すべての変更が完了するまで利用できません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-245">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="14ea3-246">登録できるのは、マルチ テナント アプリだけです。</span><span class="sxs-lookup"><span data-stu-id="14ea3-246">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="14ea3-247">アプリの更新は、初期ベータ更新後に登録されたアプリに限定されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-247">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="14ea3-248">Azure Active Directory ユーザーは、アプリの登録と所有者の追加を行えます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-248">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="14ea3-249">OpenID Connect と OAuth プロトコルをサポートします。</span><span class="sxs-lookup"><span data-stu-id="14ea3-249">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="14ea3-250">アプリケーションへのポリシーの割り当てが失敗します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-250">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="14ea3-251">アプリ ID を必要とする ownedObjects に対する操作 (たとえば、users/{id|userPrincipalName}/ownedObjects/{id}/...) が失敗します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-251">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="14ea3-252">開発中:</span><span class="sxs-lookup"><span data-stu-id="14ea3-252">In development:</span></span>

* <span data-ttu-id="14ea3-253">単一テナント アプリを登録する機能。</span><span class="sxs-lookup"><span data-stu-id="14ea3-253">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="14ea3-254">servicePrincipal に対する更新。</span><span class="sxs-lookup"><span data-stu-id="14ea3-254">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="14ea3-255">更新されたモデルへの既存の Azure AD アプリへの移行。</span><span class="sxs-lookup"><span data-stu-id="14ea3-255">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="14ea3-256">appRoles、事前承認済みクライアント、オプションのクレーム、グループ メンバーシップのクレーム、ブランド化のサポート。</span><span class="sxs-lookup"><span data-stu-id="14ea3-256">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="14ea3-257">Microsoft アカウント (MSA) ユーザーによるアプリの登録。</span><span class="sxs-lookup"><span data-stu-id="14ea3-257">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="14ea3-258">SAML および WsFed プロトコルのサポート。</span><span class="sxs-lookup"><span data-stu-id="14ea3-258">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="14ea3-259">拡張機能</span><span class="sxs-lookup"><span data-stu-id="14ea3-259">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="14ea3-260">変更履歴はサポートされていません</span><span class="sxs-lookup"><span data-stu-id="14ea3-260">Change tracking is not supported</span></span>

<span data-ttu-id="14ea3-261">変更の追跡 (デルタ クエリ) はオープン拡張機能またはスキーマ拡張機能のプロパティではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-261">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="14ea3-262">リソースとオープン拡張機能の同時作成</span><span class="sxs-lookup"><span data-stu-id="14ea3-262">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="14ea3-p124">**管理単位**、**デバイス**、**グループ**、**組織**、または**ユーザー**のインスタンスを作成するのと同時に、オープン拡張機能を指定することはできません。最初にインスタンスを作成し、次にそのインスタンスの後続の ``POST`` 要求でオープン拡張機能データを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p124">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="14ea3-265">リソースのインスタンスを作成し、同時にスキーマ拡張機能データを追加します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-265">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="14ea3-266">**連絡先**、**イベント**、**メッセージ**、**投稿**のインスタンスを作成する場合と同じ操作では、スキーマ拡張機能を指定できません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-266">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="14ea3-267">リソースのインスタンスを作成してから、そのインスタンスに`PATCH` 操作を行い、スキーマ拡張機能とカスタム データを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="14ea3-267">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="14ea3-268">スキーマ拡張機能のプロパティ値はリソースのインスタンスごとに 100 に制限されています。</span><span class="sxs-lookup"><span data-stu-id="14ea3-268">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="14ea3-269">現在、**デバイス**、**グループ**、**ユーザー**などのディレクトリ リソースでは、1 つのリソース インスタンスで設定可能なスキーマ拡張機能のプロパティ値の合計数が 100 に制限されています。</span><span class="sxs-lookup"><span data-stu-id="14ea3-269">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="14ea3-270">スキーマ拡張プロパティによるフィルター処理はすべてのエンティティ タイプでサポートされているわけではありません</span><span class="sxs-lookup"><span data-stu-id="14ea3-270">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="14ea3-271">スキーマ拡張プロパティによるフィルター処理 (`$filter` 式を使用する) は、Outlook エンティティ タイプ - **contact**、**event**、**message**、または **post** ではサポートされません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-271">Filtering on schema extension properties (using the `$filter` expresssion) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="14ea3-272">JSON バッチ処理</span><span class="sxs-lookup"><span data-stu-id="14ea3-272">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="14ea3-273">入れ子状のバッチ不可</span><span class="sxs-lookup"><span data-stu-id="14ea3-273">No nested batch</span></span>

<span data-ttu-id="14ea3-274">JSON のバッチ要求には、入れ子になったバッチは一切含めることはできません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-274">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="14ea3-275">個々の要求はすべて同期要求とします。</span><span class="sxs-lookup"><span data-stu-id="14ea3-275">All individual requests must be synchronous</span></span>

<span data-ttu-id="14ea3-p126">バッチ要求に含まれるすべての要求は同期して実行する必要があります。存在する場合、`respond-async` の設定は無視されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p126">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="14ea3-278">トランザクション未対応</span><span class="sxs-lookup"><span data-stu-id="14ea3-278">No transactions</span></span>

<span data-ttu-id="14ea3-p127">Microsoft Graph は現段階では個々の要求のトランザクション処理をサポートしていません。個々の要求で `atomicityGroup` プロパティを指定しても無視されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p127">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="14ea3-281">URI は相対 URI である必要があります。</span><span class="sxs-lookup"><span data-stu-id="14ea3-281">URIs must be relative</span></span>

<span data-ttu-id="14ea3-p128">バッチ要求では、必ず相対 URI を指定してください。Microsoft Graph はバッチ要求の URL に含まれているバージョン エンドポイントを使い、これらを絶対 URL に変換します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p128">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="14ea3-284">バッチ サイズの制限</span><span class="sxs-lookup"><span data-stu-id="14ea3-284">Limit on batch size</span></span>

<span data-ttu-id="14ea3-285">現段階では、JSON バッチ要求は 20 個までの個別要求に限られています。</span><span class="sxs-lookup"><span data-stu-id="14ea3-285">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="14ea3-286">簡略化された依存関係</span><span class="sxs-lookup"><span data-stu-id="14ea3-286">Simplified dependencies</span></span>

<span data-ttu-id="14ea3-p129">個々の要求は、他の個々の要求に依存することがあります。現在、各要求は他の要求一つだけに依存でき、以下のパターンのどれかにあてはまることが必要です。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p129">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="14ea3-289">並行:依存する要求が `dependsOn` プロパティに指定されていない場合。</span><span class="sxs-lookup"><span data-stu-id="14ea3-289">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="14ea3-290">直列:個々の要求のすべてが前の個々の要求に依存する場合。</span><span class="sxs-lookup"><span data-stu-id="14ea3-290">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="14ea3-291">同列:`dependsOn` プロパティに依存を示した個々の要求のすべてが同じ依存を指定している場合。</span><span class="sxs-lookup"><span data-stu-id="14ea3-291">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="14ea3-292">JSON バッチ処理が完成に近づくにつれて、これらの制限は削除されます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-292">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="14ea3-293">クラウド ソリューション プロバイダー アプリ</span><span class="sxs-lookup"><span data-stu-id="14ea3-293">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="14ea3-294">CSP アプリは Azure AD エンドポイントを使用する必要がある</span><span class="sxs-lookup"><span data-stu-id="14ea3-294">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="14ea3-p130">クラウド ソリューション プロバイダー (CSP) のアプリケーションは、パートナー管理の顧客から Microsoft Graph を正常に呼び出すには、Azure AD (v1) のエンドポイントからトークンを取得する必要があります。現時点では、新しい Azure AD バージョン 2.0 エンドポイントからのトークン取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p130">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="14ea3-297">CSP アプリの事前同意が一部の顧客テナントで機能しない</span><span class="sxs-lookup"><span data-stu-id="14ea3-297">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="14ea3-298">状況によっては、CSP アプリの事前同意が一部の顧客テナントで機能しない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="14ea3-298">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="14ea3-299">代理アクセス許可を使用するアプリでは、新しい顧客テナントで初めてアプリを使用すると、サインイン後に次のエラーを受け取る可能性があります。`AADSTS50000: There was an error issuing a token`。</span><span class="sxs-lookup"><span data-stu-id="14ea3-299">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="14ea3-300">アプリケーションのアクセス許可を使用するアプリでは、アプリはトークンを取得できますが、Microsoft Graph を呼び出すときに予期せずにアクセス拒否メッセージを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="14ea3-300">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="14ea3-301">事前同意をすべての顧客テナントで機能させるために、できるだけ早くこの問題を解決するべく取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-301">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="14ea3-302">それまでの間、開発とテストのブロックを解除するために次の回避策を取ってください。</span><span class="sxs-lookup"><span data-stu-id="14ea3-302">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="14ea3-p131">**注:** これは永続的なソリューションではなく、開発のブロックを解除するためのものです。前述の問題が解決されたら、この回避策は必要なくなります。解決された後にこの回避策を元に戻す必要はありません。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p131">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="14ea3-p132">Azure AD v2 PowerShell セッションを開き、サインイン ウィンドウに、管理者資格情報を入力して `customer` テナントに接続します。Azure AD PowerShell V2 は、[ここ](https://www.powershellgallery.com/packages/AzureAD)からダウンロードし、インストールできます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p132">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="14ea3-308">Microsoft Graph サービス プリンシパルを作成します。</span><span class="sxs-lookup"><span data-stu-id="14ea3-308">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="14ea3-309">Office 365 REST と Azure AD Graph API でのみ使用可能な機能</span><span class="sxs-lookup"><span data-stu-id="14ea3-309">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="14ea3-p133">Microsoft Graph では一部の機能はまだ利用できません。探している機能が表示されない場合は、エンドポイント固有の [Office 365 REST API](https://msdn.microsoft.com/office/office365/api/api-catalog) を使用することができます。Azure Active Directory において、Azure AD と Graph API を介してのみ使用可能な機能については、[Microsoft Graph または Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) のブログの投稿を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p133">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

## <a name="feedback"></a><span data-ttu-id="14ea3-313">フィードバック</span><span class="sxs-lookup"><span data-stu-id="14ea3-313">Feedback</span></span>

> <span data-ttu-id="14ea3-p134">お客様からのフィードバックを重視しています。[スタック オーバーフロー](https://stackoverflow.com/questions/tagged/microsoftgraph)でご連絡いただけます。</span><span class="sxs-lookup"><span data-stu-id="14ea3-p134">Your feedback is important to us. Connect with us on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoftgraph).</span></span>
