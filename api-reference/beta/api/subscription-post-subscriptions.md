---
title: サブスクリプションを作成する
description: Microsoft Graph リソース上のデータが変更されたときに通知を受信するリスナーアプリケーションをサブスクライブします。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: a8b8189780ac0b820551fb885adcf843c9ebe8f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545300"
---
# <a name="create-subscription"></a><span data-ttu-id="62cc8-103">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="62cc8-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62cc8-104">変更の要求された種類が Microsoft Graph の指定されたリソースに発生したときに通知を受信するため、リスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="62cc8-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="62cc8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="62cc8-105">Permissions</span></span>

<span data-ttu-id="62cc8-106">サブスクリプションを作成するにはリソースへの読み取りスコープが必要です。</span><span class="sxs-lookup"><span data-stu-id="62cc8-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="62cc8-107">たとえば、メッセージに関する通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="62cc8-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="62cc8-108">要求されたリソースとアクセス許可の種類 (委任またはアプリケーション) に応じて、以下の表で指定されているアクセス許可がこの API を呼び出すため必要な最小限の特権となります。</span><span class="sxs-lookup"><span data-stu-id="62cc8-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="62cc8-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62cc8-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62cc8-110">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="62cc8-110">Supported resource</span></span> | <span data-ttu-id="62cc8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62cc8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="62cc8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62cc8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62cc8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62cc8-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="62cc8-114">連絡先</span><span class="sxs-lookup"><span data-stu-id="62cc8-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="62cc8-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-115">Contacts.Read</span></span> | <span data-ttu-id="62cc8-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-116">Contacts.Read</span></span> | <span data-ttu-id="62cc8-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-117">Contacts.Read</span></span> |
|<span data-ttu-id="62cc8-118">[driveItem](../resources/driveitem.md) (ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="62cc8-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="62cc8-119">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="62cc8-119">Not supported</span></span> | <span data-ttu-id="62cc8-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="62cc8-120">Files.ReadWrite</span></span> | <span data-ttu-id="62cc8-121">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="62cc8-121">Not supported</span></span> |
|<span data-ttu-id="62cc8-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="62cc8-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="62cc8-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="62cc8-124">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="62cc8-124">Not supported</span></span> | <span data-ttu-id="62cc8-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="62cc8-126">イベント</span><span class="sxs-lookup"><span data-stu-id="62cc8-126">event</span></span>](../resources/event.md) | <span data-ttu-id="62cc8-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-127">Calendars.Read</span></span> | <span data-ttu-id="62cc8-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-128">Calendars.Read</span></span> | <span data-ttu-id="62cc8-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-129">Calendars.Read</span></span> |
|[<span data-ttu-id="62cc8-130">グループ</span><span class="sxs-lookup"><span data-stu-id="62cc8-130">group</span></span>](../resources/group.md) | <span data-ttu-id="62cc8-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-131">Group.Read.All</span></span> | <span data-ttu-id="62cc8-132">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="62cc8-132">Not supported</span></span> | <span data-ttu-id="62cc8-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-133">Group.Read.All</span></span> |
|[<span data-ttu-id="62cc8-134">グループ会話</span><span class="sxs-lookup"><span data-stu-id="62cc8-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="62cc8-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-135">Group.Read.All</span></span> | <span data-ttu-id="62cc8-136">非サポート</span><span class="sxs-lookup"><span data-stu-id="62cc8-136">Not supported</span></span> | <span data-ttu-id="62cc8-137">非サポート</span><span class="sxs-lookup"><span data-stu-id="62cc8-137">Not supported</span></span> |
|[<span data-ttu-id="62cc8-138">メッセージ</span><span class="sxs-lookup"><span data-stu-id="62cc8-138">message</span></span>](../resources/message.md) | <span data-ttu-id="62cc8-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-139">Mail.Read</span></span> | <span data-ttu-id="62cc8-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-140">Mail.Read</span></span> | <span data-ttu-id="62cc8-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="62cc8-141">Mail.Read</span></span> |
|[<span data-ttu-id="62cc8-142">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="62cc8-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="62cc8-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="62cc8-144">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="62cc8-144">Not supported</span></span> | <span data-ttu-id="62cc8-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="62cc8-146">ユーザー</span><span class="sxs-lookup"><span data-stu-id="62cc8-146">user</span></span>](../resources/user.md) | <span data-ttu-id="62cc8-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-147">User.Read.All</span></span> | <span data-ttu-id="62cc8-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-148">User.Read.All</span></span> | <span data-ttu-id="62cc8-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="62cc8-149">User.Read.All</span></span> |

> <span data-ttu-id="62cc8-150">**注:** OneDrive と Outlook のアイテムのサブスクリプションについては、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="62cc8-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="62cc8-151">この制限は、サブスクリプションの作成および管理 (サブスクリプションの取得、更新、削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="62cc8-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="62cc8-152">個人用 OneDrive では、そのドライブのルート フォルダーまたは任意のサブフォルダーにサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="62cc8-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="62cc8-153">OneDrive for Business の場合、サブスクライブできるのはルート フォルダーだけです。</span><span class="sxs-lookup"><span data-stu-id="62cc8-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="62cc8-154">サブスクライブしたフォルダー、または階層内の任意のファイル、フォルダー、あるいは他の **driveItem** インスタンスに関する変更の要求された種類についての通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="62cc8-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="62cc8-155">**ドライブ**、または個々のファイルなどのフォルダーではない **driveItem** インスタンスをサブスクライブすることはできません。</span><span class="sxs-lookup"><span data-stu-id="62cc8-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="62cc8-156">Outlook における委任されたアクセス許可では、サインインしているユーザーのメールボックス内のフォルダーにあるアイテムのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="62cc8-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="62cc8-157">つまり、委任されたアクセス許可 Calendars.Read を使用して、別のユーザーのメールボックス内のイベントをサブスクライブすることなどはできません。</span><span class="sxs-lookup"><span data-stu-id="62cc8-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="62cc8-158">_共有または委任_フォルダーの Outlook 連絡先、イベント、メッセージの変更通知をサブスクライブするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="62cc8-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="62cc8-159">対応するアプリケーション アクセス許可を使用して、テナントの_任意_のユーザーのフォルダーまたはメールボックス内にあるアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="62cc8-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="62cc8-160">Outlook 共有アクセス許可 (Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared、および対応する読み取り/書き込み) は使用しないでください。それらは、共有フォルダーまたは委任フォルダーにあるアイテムの変更通知のサブスクライブをサポート**していない**からです。</span><span class="sxs-lookup"><span data-stu-id="62cc8-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="62cc8-161">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62cc8-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="62cc8-162">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62cc8-162">Request headers</span></span>

| <span data-ttu-id="62cc8-163">名前</span><span class="sxs-lookup"><span data-stu-id="62cc8-163">Name</span></span>       | <span data-ttu-id="62cc8-164">型</span><span class="sxs-lookup"><span data-stu-id="62cc8-164">Type</span></span> | <span data-ttu-id="62cc8-165">説明</span><span class="sxs-lookup"><span data-stu-id="62cc8-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="62cc8-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="62cc8-166">Authorization</span></span>  | <span data-ttu-id="62cc8-167">string</span><span class="sxs-lookup"><span data-stu-id="62cc8-167">string</span></span>  | <span data-ttu-id="62cc8-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="62cc8-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="62cc8-170">応答</span><span class="sxs-lookup"><span data-stu-id="62cc8-170">Response</span></span>

<span data-ttu-id="62cc8-171">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62cc8-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62cc8-172">例</span><span class="sxs-lookup"><span data-stu-id="62cc8-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="62cc8-173">要求</span><span class="sxs-lookup"><span data-stu-id="62cc8-173">Request</span></span>

<span data-ttu-id="62cc8-174">要求本文で、[subscription](../resources/subscription.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="62cc8-174">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="62cc8-175">`clientState` フィールドは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="62cc8-175">The `clientState` field is optional.</span></span>

<span data-ttu-id="62cc8-176">このサンプル要求は、現在サインインしているユーザーが受信した新着メールに関する通知のサブスクリプションを作成します。</span><span class="sxs-lookup"><span data-stu-id="62cc8-176">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="62cc8-177">resource プロパティの有効な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="62cc8-177">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="62cc8-178">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62cc8-178">Resource type</span></span> | <span data-ttu-id="62cc8-179">例</span><span class="sxs-lookup"><span data-stu-id="62cc8-179">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="62cc8-180">メール</span><span class="sxs-lookup"><span data-stu-id="62cc8-180">Mail</span></span>|<span data-ttu-id="62cc8-181">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="62cc8-181">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="62cc8-182">me/messages</span><span class="sxs-lookup"><span data-stu-id="62cc8-182">me/messages</span></span>|
|<span data-ttu-id="62cc8-183">連絡先</span><span class="sxs-lookup"><span data-stu-id="62cc8-183">Contacts</span></span>|<span data-ttu-id="62cc8-184">me/contacts</span><span class="sxs-lookup"><span data-stu-id="62cc8-184">me/contacts</span></span>|
|<span data-ttu-id="62cc8-185">カレンダー</span><span class="sxs-lookup"><span data-stu-id="62cc8-185">Calendars</span></span>|<span data-ttu-id="62cc8-186">me/events</span><span class="sxs-lookup"><span data-stu-id="62cc8-186">me/events</span></span>|
|<span data-ttu-id="62cc8-187">ユーザー</span><span class="sxs-lookup"><span data-stu-id="62cc8-187">Users</span></span>|<span data-ttu-id="62cc8-188">users</span><span class="sxs-lookup"><span data-stu-id="62cc8-188">users</span></span>|
|<span data-ttu-id="62cc8-189">グループ</span><span class="sxs-lookup"><span data-stu-id="62cc8-189">Groups</span></span>|<span data-ttu-id="62cc8-190">groups</span><span class="sxs-lookup"><span data-stu-id="62cc8-190">groups</span></span>|
|<span data-ttu-id="62cc8-191">会話</span><span class="sxs-lookup"><span data-stu-id="62cc8-191">Conversations</span></span>|<span data-ttu-id="62cc8-192">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="62cc8-192">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="62cc8-193">ドライブ</span><span class="sxs-lookup"><span data-stu-id="62cc8-193">Drives</span></span>|<span data-ttu-id="62cc8-194">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="62cc8-194">me/drive/root</span></span>|
|<span data-ttu-id="62cc8-195">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="62cc8-195">Security alert</span></span>|<span data-ttu-id="62cc8-196">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="62cc8-196">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="62cc8-197">応答</span><span class="sxs-lookup"><span data-stu-id="62cc8-197">Response</span></span>

<span data-ttu-id="62cc8-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62cc8-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="62cc8-201">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="62cc8-201">Notification endpoint validation</span></span>

<span data-ttu-id="62cc8-202">サブスクリプションの通知のエンドポイントは (`notificationUrl` プロパティで指定されている)、「[ユーザー データの変更に関する通知の設定](/graph/webhooks#notification-endpoint-validation)」での説明にあるように、検証依頼に応答できなければなりません。</span><span class="sxs-lookup"><span data-stu-id="62cc8-202">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="62cc8-203">検証に失敗した場合、サブスクリプションを作成する要求は「400 要求が正しくありません」というエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="62cc8-203">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
