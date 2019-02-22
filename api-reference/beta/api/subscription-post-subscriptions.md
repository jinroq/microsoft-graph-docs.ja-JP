---
title: サブスクリプションを作成する
description: Microsoft Graph リソース上のデータが変更されたときに通知を受信するリスナーアプリケーションをサブスクライブします。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a8b8189780ac0b820551fb885adcf843c9ebe8f4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140167"
---
# <a name="create-subscription"></a><span data-ttu-id="c5fc0-103">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="c5fc0-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5fc0-104">リスナーアプリケーションをサブスクライブして、要求された種類の変更が Microsoft Graph の指定したリソースに対して発生したときに通知を受信します。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5fc0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5fc0-105">Permissions</span></span>

<span data-ttu-id="c5fc0-106">サブスクリプションを作成するには、リソースに対する読み取りスコープが必要です。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="c5fc0-107">たとえば、メッセージに関する通知を取得するには、アプリ`Mail.Read`にアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="c5fc0-108">リソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可は、この API を呼び出すために必要な最低限の特権です。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c5fc0-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5fc0-110">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="c5fc0-110">Supported resource</span></span> | <span data-ttu-id="c5fc0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5fc0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c5fc0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5fc0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5fc0-113">Application</span><span class="sxs-lookup"><span data-stu-id="c5fc0-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="c5fc0-114">連絡先</span><span class="sxs-lookup"><span data-stu-id="c5fc0-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c5fc0-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-115">Contacts.Read</span></span> | <span data-ttu-id="c5fc0-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-116">Contacts.Read</span></span> | <span data-ttu-id="c5fc0-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-117">Contacts.Read</span></span> |
|<span data-ttu-id="c5fc0-118">[ドライブ項目](../resources/driveitem.md)(ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="c5fc0-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="c5fc0-119">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c5fc0-119">Not supported</span></span> | <span data-ttu-id="c5fc0-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5fc0-120">Files.ReadWrite</span></span> | <span data-ttu-id="c5fc0-121">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c5fc0-121">Not supported</span></span> |
|<span data-ttu-id="c5fc0-122">[ドライブ項目](../resources/driveitem.md)(OneDrive for business)</span><span class="sxs-lookup"><span data-stu-id="c5fc0-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="c5fc0-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="c5fc0-124">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c5fc0-124">Not supported</span></span> | <span data-ttu-id="c5fc0-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="c5fc0-126">event</span><span class="sxs-lookup"><span data-stu-id="c5fc0-126">event</span></span>](../resources/event.md) | <span data-ttu-id="c5fc0-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-127">Calendars.Read</span></span> | <span data-ttu-id="c5fc0-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-128">Calendars.Read</span></span> | <span data-ttu-id="c5fc0-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-129">Calendars.Read</span></span> |
|[<span data-ttu-id="c5fc0-130">group</span><span class="sxs-lookup"><span data-stu-id="c5fc0-130">group</span></span>](../resources/group.md) | <span data-ttu-id="c5fc0-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-131">Group.Read.All</span></span> | <span data-ttu-id="c5fc0-132">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c5fc0-132">Not supported</span></span> | <span data-ttu-id="c5fc0-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-133">Group.Read.All</span></span> |
|[<span data-ttu-id="c5fc0-134">グループ会話</span><span class="sxs-lookup"><span data-stu-id="c5fc0-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="c5fc0-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-135">Group.Read.All</span></span> | <span data-ttu-id="c5fc0-136">使用不可</span><span class="sxs-lookup"><span data-stu-id="c5fc0-136">Not supported</span></span> | <span data-ttu-id="c5fc0-137">使用不可</span><span class="sxs-lookup"><span data-stu-id="c5fc0-137">Not supported</span></span> |
|[<span data-ttu-id="c5fc0-138">message</span><span class="sxs-lookup"><span data-stu-id="c5fc0-138">message</span></span>](../resources/message.md) | <span data-ttu-id="c5fc0-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-139">Mail.Read</span></span> | <span data-ttu-id="c5fc0-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-140">Mail.Read</span></span> | <span data-ttu-id="c5fc0-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c5fc0-141">Mail.Read</span></span> |
|[<span data-ttu-id="c5fc0-142">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="c5fc0-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="c5fc0-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="c5fc0-144">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="c5fc0-144">Not supported</span></span> | <span data-ttu-id="c5fc0-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="c5fc0-146">user</span><span class="sxs-lookup"><span data-stu-id="c5fc0-146">user</span></span>](../resources/user.md) | <span data-ttu-id="c5fc0-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-147">User.Read.All</span></span> | <span data-ttu-id="c5fc0-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-148">User.Read.All</span></span> | <span data-ttu-id="c5fc0-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5fc0-149">User.Read.All</span></span> |

> <span data-ttu-id="c5fc0-150">**注:** OneDrive および Outlook アイテムのサブスクリプションには、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="c5fc0-151">この制限は、サブスクリプションの作成と管理 (サブスクリプションの取得、更新、および削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="c5fc0-152">個人用 OneDrive では、ルートフォルダーまたはそのドライブの任意のサブフォルダーを購読できます。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="c5fc0-153">OneDrive for business では、ルートフォルダーのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="c5fc0-154">通知は、サブスクライブされたフォルダー、または、階層内の任意のファイル、フォルダー、またはその他の**ドライブのアイテム**インスタンスに対して、要求された種類の変更に対して送信されます。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="c5fc0-155">個別のファイルなど、フォルダーではない**drive**または**drive アイテム**のインスタンスを購読することはできません。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="c5fc0-156">Outlook では、委任されたアクセス許可は、サインインしているユーザーのメールボックス内のフォルダー内のアイテムのサブスクライブをサポートします。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="c5fc0-157">つまり、委任されたアクセス許可のカレンダーを使用することはできません。別のユーザーのメールボックス内のイベントをサブスクライブするには、をお読みください。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="c5fc0-158">Outlook の連絡先、イベント、または_共有フォルダーまたは委任_されたフォルダー内のメッセージの変更通知を購読するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="c5fc0-159">対応するアプリケーションのアクセス許可を使用して、テナント内の_任意_のユーザーのフォルダーまたはメールボックス内のアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="c5fc0-160">共有または委任されたフォルダー内のアイテムの通知を変更するためのサブスクライブをサポートして**い**ないため、Outlook 共有のアクセス許可 (連絡先. 共有、読み取り/書き込み可能) を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="c5fc0-161">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5fc0-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="c5fc0-162">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5fc0-162">Request headers</span></span>

| <span data-ttu-id="c5fc0-163">名前</span><span class="sxs-lookup"><span data-stu-id="c5fc0-163">Name</span></span>       | <span data-ttu-id="c5fc0-164">型</span><span class="sxs-lookup"><span data-stu-id="c5fc0-164">Type</span></span> | <span data-ttu-id="c5fc0-165">説明</span><span class="sxs-lookup"><span data-stu-id="c5fc0-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5fc0-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5fc0-166">Authorization</span></span>  | <span data-ttu-id="c5fc0-167">string</span><span class="sxs-lookup"><span data-stu-id="c5fc0-167">string</span></span>  | <span data-ttu-id="c5fc0-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c5fc0-170">応答</span><span class="sxs-lookup"><span data-stu-id="c5fc0-170">Response</span></span>

<span data-ttu-id="c5fc0-171">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5fc0-172">例</span><span class="sxs-lookup"><span data-stu-id="c5fc0-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c5fc0-173">要求</span><span class="sxs-lookup"><span data-stu-id="c5fc0-173">Request</span></span>

<span data-ttu-id="c5fc0-174">要求本文で、 [subscription](../resources/subscription.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-174">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="c5fc0-175">この`clientState`フィールドは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-175">The `clientState` field is optional.</span></span>

<span data-ttu-id="c5fc0-176">このサンプル要求は、現在サインインしているユーザーが受信した新着メールに関する通知のサブスクリプションを作成します。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-176">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="c5fc0-177">resource プロパティの有効な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-177">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="c5fc0-178">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5fc0-178">Resource type</span></span> | <span data-ttu-id="c5fc0-179">例</span><span class="sxs-lookup"><span data-stu-id="c5fc0-179">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="c5fc0-180">メール</span><span class="sxs-lookup"><span data-stu-id="c5fc0-180">Mail</span></span>|<span data-ttu-id="c5fc0-181">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="c5fc0-181">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="c5fc0-182">me/messages</span><span class="sxs-lookup"><span data-stu-id="c5fc0-182">me/messages</span></span>|
|<span data-ttu-id="c5fc0-183">連絡先</span><span class="sxs-lookup"><span data-stu-id="c5fc0-183">Contacts</span></span>|<span data-ttu-id="c5fc0-184">me/contacts</span><span class="sxs-lookup"><span data-stu-id="c5fc0-184">me/contacts</span></span>|
|<span data-ttu-id="c5fc0-185">カレンダー</span><span class="sxs-lookup"><span data-stu-id="c5fc0-185">Calendars</span></span>|<span data-ttu-id="c5fc0-186">me/events</span><span class="sxs-lookup"><span data-stu-id="c5fc0-186">me/events</span></span>|
|<span data-ttu-id="c5fc0-187">ユーザー</span><span class="sxs-lookup"><span data-stu-id="c5fc0-187">Users</span></span>|<span data-ttu-id="c5fc0-188">users</span><span class="sxs-lookup"><span data-stu-id="c5fc0-188">users</span></span>|
|<span data-ttu-id="c5fc0-189">グループ</span><span class="sxs-lookup"><span data-stu-id="c5fc0-189">Groups</span></span>|<span data-ttu-id="c5fc0-190">グループ</span><span class="sxs-lookup"><span data-stu-id="c5fc0-190">groups</span></span>|
|<span data-ttu-id="c5fc0-191">会話</span><span class="sxs-lookup"><span data-stu-id="c5fc0-191">Conversations</span></span>|<span data-ttu-id="c5fc0-192">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="c5fc0-192">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="c5fc0-193">ドライブ</span><span class="sxs-lookup"><span data-stu-id="c5fc0-193">Drives</span></span>|<span data-ttu-id="c5fc0-194">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="c5fc0-194">me/drive/root</span></span>|
|<span data-ttu-id="c5fc0-195">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="c5fc0-195">Security alert</span></span>|<span data-ttu-id="c5fc0-196">セキュリティ/アラートの $filter = 状態 eq ' 新規 '</span><span class="sxs-lookup"><span data-stu-id="c5fc0-196">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="c5fc0-197">応答</span><span class="sxs-lookup"><span data-stu-id="c5fc0-197">Response</span></span>

<span data-ttu-id="c5fc0-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="c5fc0-201">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="c5fc0-201">Notification endpoint validation</span></span>

<span data-ttu-id="c5fc0-202">「 `notificationUrl` [ユーザーデータの変更の通知を設定](/graph/webhooks#notification-endpoint-validation)する」の説明に従って、プロパティで指定されているサブスクリプション通知エンドポイントは、検証要求に応答できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-202">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="c5fc0-203">検証が失敗した場合、サブスクリプションを作成する要求は、400不良要求エラーを返します。</span><span class="sxs-lookup"><span data-stu-id="c5fc0-203">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-post-subscriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
