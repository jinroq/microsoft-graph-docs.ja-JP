---
title: サブスクリプションを作成する
description: Graph リソース上のデータが変更されたときに通知を受信するリスナー アプリケーションをサブスクライブします。
localization_priority: Normal
ms.openlocfilehash: 5b7f465e556d1fb752bcb2d3c962fd6444d462c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805055"
---
# <a name="create-subscription"></a><span data-ttu-id="96e25-103">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="96e25-103">Create subscription</span></span>

> <span data-ttu-id="96e25-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="96e25-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96e25-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96e25-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96e25-106">Graph リソース上のデータが変更されたときに通知を受信するリスナー アプリケーションをサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="96e25-106">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="96e25-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="96e25-107">Permissions</span></span>

<span data-ttu-id="96e25-108">サブスクリプションを作成するには、アプリケーションが通知を受信するリソースの読み取り権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="96e25-108">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="96e25-109">たとえば、メッセージに関する通知を取得するには、アプリが必要な`Mail.Read`のアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="96e25-109">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="96e25-110">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="96e25-110">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="96e25-111">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96e25-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96e25-112">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="96e25-112">Resource type / Item</span></span>        | <span data-ttu-id="96e25-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="96e25-113">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="96e25-114">連絡先</span><span class="sxs-lookup"><span data-stu-id="96e25-114">Contacts</span></span>                    | <span data-ttu-id="96e25-115">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="96e25-115">Contacts.Read</span></span>       |
| <span data-ttu-id="96e25-116">スレッド</span><span class="sxs-lookup"><span data-stu-id="96e25-116">Conversations</span></span>               | <span data-ttu-id="96e25-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e25-117">Group.Read.All</span></span>      |
| <span data-ttu-id="96e25-118">イベント</span><span class="sxs-lookup"><span data-stu-id="96e25-118">Events</span></span>                      | <span data-ttu-id="96e25-119">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="96e25-119">Calendars.Read</span></span>      |
| <span data-ttu-id="96e25-120">メッセージ</span><span class="sxs-lookup"><span data-stu-id="96e25-120">Messages</span></span>                    | <span data-ttu-id="96e25-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="96e25-121">Mail.Read</span></span>           |
| <span data-ttu-id="96e25-122">グループ</span><span class="sxs-lookup"><span data-stu-id="96e25-122">Groups</span></span>                      | <span data-ttu-id="96e25-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e25-123">Group.Read.All</span></span>      |
| <span data-ttu-id="96e25-124">ユーザー</span><span class="sxs-lookup"><span data-stu-id="96e25-124">Users</span></span>                       | <span data-ttu-id="96e25-125">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e25-125">User.Read.All</span></span>       |
| <span data-ttu-id="96e25-126">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="96e25-126">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="96e25-127">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96e25-127">Files.ReadWrite</span></span>     |
| <span data-ttu-id="96e25-128">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="96e25-128">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="96e25-129">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e25-129">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="96e25-130">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="96e25-130">Security alert</span></span>              | <span data-ttu-id="96e25-131">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96e25-131">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="96e25-132">**注:**/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="96e25-132">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="96e25-133">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96e25-133">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="96e25-134">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96e25-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="96e25-135">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96e25-135">Request headers</span></span>

| <span data-ttu-id="96e25-136">名前</span><span class="sxs-lookup"><span data-stu-id="96e25-136">Name</span></span>       | <span data-ttu-id="96e25-137">種類</span><span class="sxs-lookup"><span data-stu-id="96e25-137">Type</span></span> | <span data-ttu-id="96e25-138">説明</span><span class="sxs-lookup"><span data-stu-id="96e25-138">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96e25-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="96e25-139">Authorization</span></span>  | <span data-ttu-id="96e25-140">string</span><span class="sxs-lookup"><span data-stu-id="96e25-140">string</span></span>  | <span data-ttu-id="96e25-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="96e25-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="96e25-143">応答</span><span class="sxs-lookup"><span data-stu-id="96e25-143">Response</span></span>

<span data-ttu-id="96e25-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="96e25-144">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96e25-145">例</span><span class="sxs-lookup"><span data-stu-id="96e25-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="96e25-146">要求</span><span class="sxs-lookup"><span data-stu-id="96e25-146">Request</span></span>

<span data-ttu-id="96e25-147">要求の本文には、[サブスクリプション](../resources/subscription.md)オブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="96e25-147">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="96e25-148">`clientState`フィールドは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="96e25-148">The `clientState` field is optional.</span></span>

<span data-ttu-id="96e25-149">このサンプル リクエストは、現在サインインしているユーザーが受信したメールの通知のサブスクリプションを作成します。</span><span class="sxs-lookup"><span data-stu-id="96e25-149">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="96e25-150">リソース プロパティの設定値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="96e25-150">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="96e25-151">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96e25-151">Resource type</span></span> | <span data-ttu-id="96e25-152">例</span><span class="sxs-lookup"><span data-stu-id="96e25-152">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="96e25-153">メール</span><span class="sxs-lookup"><span data-stu-id="96e25-153">Mail</span></span>|<span data-ttu-id="96e25-154">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="96e25-154">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="96e25-155">me/messages</span><span class="sxs-lookup"><span data-stu-id="96e25-155">me/messages</span></span>|
|<span data-ttu-id="96e25-156">連絡先</span><span class="sxs-lookup"><span data-stu-id="96e25-156">Contacts</span></span>|<span data-ttu-id="96e25-157">me/contacts</span><span class="sxs-lookup"><span data-stu-id="96e25-157">me/contacts</span></span>|
|<span data-ttu-id="96e25-158">カレンダー</span><span class="sxs-lookup"><span data-stu-id="96e25-158">Calendars</span></span>|<span data-ttu-id="96e25-159">me/events</span><span class="sxs-lookup"><span data-stu-id="96e25-159">me/events</span></span>|
|<span data-ttu-id="96e25-160">ユーザー</span><span class="sxs-lookup"><span data-stu-id="96e25-160">Users</span></span>|<span data-ttu-id="96e25-161">users</span><span class="sxs-lookup"><span data-stu-id="96e25-161">users</span></span>|
|<span data-ttu-id="96e25-162">グループ</span><span class="sxs-lookup"><span data-stu-id="96e25-162">Groups</span></span>|<span data-ttu-id="96e25-163">グループ</span><span class="sxs-lookup"><span data-stu-id="96e25-163">groups</span></span>|
|<span data-ttu-id="96e25-164">会話</span><span class="sxs-lookup"><span data-stu-id="96e25-164">Conversations</span></span>|<span data-ttu-id="96e25-165">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="96e25-165">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="96e25-166">ドライブ</span><span class="sxs-lookup"><span data-stu-id="96e25-166">Drives</span></span>|<span data-ttu-id="96e25-167">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="96e25-167">me/drive/root</span></span>|
|<span data-ttu-id="96e25-168">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="96e25-168">Security alert</span></span>|<span data-ttu-id="96e25-169">セキュリティと警告? $filter eq のステータスを 'New' =</span><span class="sxs-lookup"><span data-stu-id="96e25-169">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="96e25-170">応答</span><span class="sxs-lookup"><span data-stu-id="96e25-170">Response</span></span>

<span data-ttu-id="96e25-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="96e25-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="96e25-174">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="96e25-174">Notification endpoint validation</span></span>

<span data-ttu-id="96e25-175">サブスクリプション通知エンドポイント (で指定されている、`notificationUrl`プロパティ) の[ユーザー データの変更の通知の設定](/graph/webhooks#notification-endpoint-validation)で説明したように、検証要求に応答できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="96e25-175">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="96e25-176">検証が失敗した場合、サブスクリプションを作成する要求は 400 不正な要求のエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="96e25-176">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
