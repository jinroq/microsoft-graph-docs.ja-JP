---
title: サブスクリプションを作成する
description: Microsoft Graph リソース上のデータが変更されたときに通知を受信するリスナーアプリケーションをサブスクライブします。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: b23cfa1eec29ed77f822cdaa0ff3073100df722b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458200"
---
# <a name="create-subscription"></a><span data-ttu-id="30b1a-103">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="30b1a-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30b1a-104">変更の要求された種類が Microsoft Graph の指定されたリソースに発生したときに通知を受信するため、リスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="30b1a-104">Subscribes a listener application to receive notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

## <a name="permissions"></a><span data-ttu-id="30b1a-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="30b1a-105">Permissions</span></span>

<span data-ttu-id="30b1a-106">サブスクリプションを作成するにはリソースへの読み取りスコープが必要です。</span><span class="sxs-lookup"><span data-stu-id="30b1a-106">Creating a subscription requires read scope to the resource.</span></span> <span data-ttu-id="30b1a-107">たとえば、メッセージに関する通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="30b1a-107">For example, to get notifications on messages, your app needs the `Mail.Read` permission.</span></span> 
 
 <span data-ttu-id="30b1a-108">要求されたリソースとアクセス許可の種類 (委任およびアプリケーション) によっては、以下の表で指定されているアクセス許可がこの API を呼び出すために最小限必要な特権となります。</span><span class="sxs-lookup"><span data-stu-id="30b1a-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="30b1a-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30b1a-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30b1a-110">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="30b1a-110">Supported resource</span></span> | <span data-ttu-id="30b1a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="30b1a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="30b1a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="30b1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30b1a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="30b1a-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="30b1a-114">連絡先</span><span class="sxs-lookup"><span data-stu-id="30b1a-114">contact</span></span>](../resources/contact.md) | <span data-ttu-id="30b1a-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-115">Contacts.Read</span></span> | <span data-ttu-id="30b1a-116">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-116">Contacts.Read</span></span> | <span data-ttu-id="30b1a-117">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-117">Contacts.Read</span></span> |
|<span data-ttu-id="30b1a-118">[driveItem](../resources/driveitem.md) (ユーザーの個人用 OneDrive)</span><span class="sxs-lookup"><span data-stu-id="30b1a-118">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="30b1a-119">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="30b1a-119">Not supported</span></span> | <span data-ttu-id="30b1a-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30b1a-120">Files.ReadWrite</span></span> | <span data-ttu-id="30b1a-121">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="30b1a-121">Not supported</span></span> |
|<span data-ttu-id="30b1a-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span><span class="sxs-lookup"><span data-stu-id="30b1a-122">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="30b1a-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-123">Files.ReadWrite.All</span></span> | <span data-ttu-id="30b1a-124">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="30b1a-124">Not supported</span></span> | <span data-ttu-id="30b1a-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-125">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="30b1a-126">イベント</span><span class="sxs-lookup"><span data-stu-id="30b1a-126">event</span></span>](../resources/event.md) | <span data-ttu-id="30b1a-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-127">Calendars.Read</span></span> | <span data-ttu-id="30b1a-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-128">Calendars.Read</span></span> | <span data-ttu-id="30b1a-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-129">Calendars.Read</span></span> |
|[<span data-ttu-id="30b1a-130">グループ</span><span class="sxs-lookup"><span data-stu-id="30b1a-130">group</span></span>](../resources/group.md) | <span data-ttu-id="30b1a-131">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-131">Group.Read.All</span></span> | <span data-ttu-id="30b1a-132">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="30b1a-132">Not supported</span></span> | <span data-ttu-id="30b1a-133">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-133">Group.Read.All</span></span> |
|[<span data-ttu-id="30b1a-134">グループ会話</span><span class="sxs-lookup"><span data-stu-id="30b1a-134">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="30b1a-135">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-135">Group.Read.All</span></span> | <span data-ttu-id="30b1a-136">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="30b1a-136">Not supported</span></span> | <span data-ttu-id="30b1a-137">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="30b1a-137">Not supported</span></span> |
|[<span data-ttu-id="30b1a-138">メッセージ</span><span class="sxs-lookup"><span data-stu-id="30b1a-138">message</span></span>](../resources/message.md) | <span data-ttu-id="30b1a-139">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-139">Mail.Read</span></span> | <span data-ttu-id="30b1a-140">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-140">Mail.Read</span></span> | <span data-ttu-id="30b1a-141">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="30b1a-141">Mail.Read</span></span> |
|[<span data-ttu-id="30b1a-142">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="30b1a-142">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="30b1a-143">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-143">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="30b1a-144">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="30b1a-144">Not supported</span></span> | <span data-ttu-id="30b1a-145">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-145">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="30b1a-146">ユーザー</span><span class="sxs-lookup"><span data-stu-id="30b1a-146">user</span></span>](../resources/user.md) | <span data-ttu-id="30b1a-147">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-147">User.Read.All</span></span> | <span data-ttu-id="30b1a-148">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-148">User.Read.All</span></span> | <span data-ttu-id="30b1a-149">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="30b1a-149">User.Read.All</span></span> |

> <span data-ttu-id="30b1a-150">**注:** OneDrive と Outlook のアイテムのサブスクリプションについては、追加の制限があります。</span><span class="sxs-lookup"><span data-stu-id="30b1a-150">**Note:** There are additional limitations for subscriptions on OneDrive and Outlook items.</span></span> <span data-ttu-id="30b1a-151">この制限は、サブスクリプションの作成および管理 (サブスクリプションの取得、更新、削除) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="30b1a-151">The limitations apply to creating as well as managing subscriptions (getting, updating, and deleting subscriptions).</span></span>

- <span data-ttu-id="30b1a-152">個人用 OneDrive では、そのドライブのルート フォルダーまたは任意のサブフォルダーにサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="30b1a-152">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="30b1a-153">OneDrive for Business の場合、サブスクライブできるのはルート フォルダーのみです。</span><span class="sxs-lookup"><span data-stu-id="30b1a-153">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="30b1a-154">サブスクライブしたフォルダー、または階層内の任意のファイル、フォルダー、あるいは他の **driveItem** インスタンスに関する変更の要求された種類についての通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="30b1a-154">Notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="30b1a-155">個別のファイルなどのフォルダーではない、**ドライブ** インスタンスまたは **driveItem** インスタンスをサブスクライブすることはできません。</span><span class="sxs-lookup"><span data-stu-id="30b1a-155">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

- <span data-ttu-id="30b1a-156">Outlook における委任されたアクセス許可では、サインインしているユーザーのメールボックス内のフォルダーにあるアイテムのみをサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="30b1a-156">In Outlook, delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="30b1a-157">つまり、委任されたアクセス許可 Calendars.Read を使用して、別のユーザーのメールボックス内のイベントをサブスクライブすることなどはできません。</span><span class="sxs-lookup"><span data-stu-id="30b1a-157">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="30b1a-158">_共有または委任_フォルダーの Outlook 連絡先、イベント、メッセージの変更通知をサブスクライブするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="30b1a-158">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="30b1a-159">対応するアプリケーション アクセス許可を使用して、テナントの_任意_のユーザーのフォルダーまたはメールボックス内にあるアイテムの変更をサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="30b1a-159">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="30b1a-160">Outlook 共有アクセス許可 (Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared、および対応する読み取り/書き込み) は使用しないでください。それらは、共有フォルダーまたは委任フォルダーにあるアイテムの変更通知のサブスクライブをサポート**していない**からです。</span><span class="sxs-lookup"><span data-stu-id="30b1a-160">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="30b1a-161">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="30b1a-161">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="30b1a-162">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30b1a-162">Request headers</span></span>

| <span data-ttu-id="30b1a-163">名前</span><span class="sxs-lookup"><span data-stu-id="30b1a-163">Name</span></span>       | <span data-ttu-id="30b1a-164">型</span><span class="sxs-lookup"><span data-stu-id="30b1a-164">Type</span></span> | <span data-ttu-id="30b1a-165">説明</span><span class="sxs-lookup"><span data-stu-id="30b1a-165">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="30b1a-166">Authorization</span><span class="sxs-lookup"><span data-stu-id="30b1a-166">Authorization</span></span>  | <span data-ttu-id="30b1a-167">string</span><span class="sxs-lookup"><span data-stu-id="30b1a-167">string</span></span>  | <span data-ttu-id="30b1a-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="30b1a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="30b1a-170">応答</span><span class="sxs-lookup"><span data-stu-id="30b1a-170">Response</span></span>

<span data-ttu-id="30b1a-171">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="30b1a-171">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30b1a-172">例</span><span class="sxs-lookup"><span data-stu-id="30b1a-172">Example</span></span>

##### <a name="request"></a><span data-ttu-id="30b1a-173">要求</span><span class="sxs-lookup"><span data-stu-id="30b1a-173">Request</span></span>

<span data-ttu-id="30b1a-174">要求本文で、[subscription](../resources/subscription.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="30b1a-174">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="30b1a-175">`clientState` フィールドは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="30b1a-175">The `clientState` field is optional.</span></span>

<span data-ttu-id="30b1a-176">このサンプル要求は、現在サインインしているユーザーが受信した新着メールに関する通知のサブスクリプションを作成します。</span><span class="sxs-lookup"><span data-stu-id="30b1a-176">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30b1a-177">プロトコル</span><span class="sxs-lookup"><span data-stu-id="30b1a-177">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="30b1a-178">C#</span><span class="sxs-lookup"><span data-stu-id="30b1a-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30b1a-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="30b1a-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30b1a-180">目的-C</span><span class="sxs-lookup"><span data-stu-id="30b1a-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="30b1a-181">Resource プロパティの有効な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="30b1a-181">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="30b1a-182">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30b1a-182">Resource type</span></span> | <span data-ttu-id="30b1a-183">例</span><span class="sxs-lookup"><span data-stu-id="30b1a-183">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="30b1a-184">メール</span><span class="sxs-lookup"><span data-stu-id="30b1a-184">Mail</span></span>|<span data-ttu-id="30b1a-185">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="30b1a-185">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="30b1a-186">me/messages</span><span class="sxs-lookup"><span data-stu-id="30b1a-186">me/messages</span></span>|
|<span data-ttu-id="30b1a-187">連絡先</span><span class="sxs-lookup"><span data-stu-id="30b1a-187">Contacts</span></span>|<span data-ttu-id="30b1a-188">me/contacts</span><span class="sxs-lookup"><span data-stu-id="30b1a-188">me/contacts</span></span>|
|<span data-ttu-id="30b1a-189">カレンダー</span><span class="sxs-lookup"><span data-stu-id="30b1a-189">Calendars</span></span>|<span data-ttu-id="30b1a-190">me/events</span><span class="sxs-lookup"><span data-stu-id="30b1a-190">me/events</span></span>|
|<span data-ttu-id="30b1a-191">ユーザー</span><span class="sxs-lookup"><span data-stu-id="30b1a-191">Users</span></span>|<span data-ttu-id="30b1a-192">users</span><span class="sxs-lookup"><span data-stu-id="30b1a-192">users</span></span>|
|<span data-ttu-id="30b1a-193">グループ</span><span class="sxs-lookup"><span data-stu-id="30b1a-193">Groups</span></span>|<span data-ttu-id="30b1a-194">groups</span><span class="sxs-lookup"><span data-stu-id="30b1a-194">groups</span></span>|
|<span data-ttu-id="30b1a-195">会話</span><span class="sxs-lookup"><span data-stu-id="30b1a-195">Conversations</span></span>|<span data-ttu-id="30b1a-196">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="30b1a-196">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="30b1a-197">ドライブ</span><span class="sxs-lookup"><span data-stu-id="30b1a-197">Drives</span></span>|<span data-ttu-id="30b1a-198">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="30b1a-198">me/drive/root</span></span>|
|<span data-ttu-id="30b1a-199">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="30b1a-199">Security alert</span></span>|<span data-ttu-id="30b1a-200">security/alerts?$filter=status eq ‘New’</span><span class="sxs-lookup"><span data-stu-id="30b1a-200">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="30b1a-201">応答</span><span class="sxs-lookup"><span data-stu-id="30b1a-201">Response</span></span>

<span data-ttu-id="30b1a-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="30b1a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="30b1a-205">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="30b1a-205">Notification endpoint validation</span></span>

<span data-ttu-id="30b1a-206">サブスクリプションの通知のエンドポイントは (`notificationUrl` プロパティで指定されている)、「[ユーザー データの変更に関する通知の設定](/graph/webhooks#notification-endpoint-validation)」での説明にあるように、検証依頼に応答できなければなりません。</span><span class="sxs-lookup"><span data-stu-id="30b1a-206">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="30b1a-207">検証に失敗した場合、サブスクリプションを作成する要求は「400 要求が正しくありません」というエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="30b1a-207">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
  ]
}
-->
