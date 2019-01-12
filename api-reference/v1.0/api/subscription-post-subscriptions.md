---
title: サブスクリプションを作成する
description: Microsoft Graph のデータが変更されたときに通知を受信するため、リスナー アプリケーションに登録します。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 7b23968620abcb8f9a20e4a7b3598c21dec72980
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913887"
---
# <a name="create-subscription"></a><span data-ttu-id="800df-103">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="800df-103">Create subscription</span></span>

<span data-ttu-id="800df-104">Microsoft Graph のデータが変更されたときに通知を受信するため、リスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="800df-104">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="800df-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="800df-105">Permissions</span></span>

<span data-ttu-id="800df-p101">サブスクリプションを作成するにはリソースへの読み取りスコープが必要です。たとえば、通知メッセージを受信するには、アプリに `Mail.Read` アクセス許可が必要です。次の表に、各リソースに必要な、推奨されるアクセス許可を示します。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="800df-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="800df-110">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="800df-110">Resource type / Item</span></span>        | <span data-ttu-id="800df-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="800df-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="800df-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="800df-112">Contacts</span></span>                    | <span data-ttu-id="800df-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="800df-113">Contacts.Read</span></span>       |
| <span data-ttu-id="800df-114">スレッド</span><span class="sxs-lookup"><span data-stu-id="800df-114">Conversations</span></span>               | <span data-ttu-id="800df-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="800df-115">Group.Read.All</span></span>      |
| <span data-ttu-id="800df-116">イベント</span><span class="sxs-lookup"><span data-stu-id="800df-116">Events</span></span>                      | <span data-ttu-id="800df-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="800df-117">Calendars.Read</span></span>      |
| <span data-ttu-id="800df-118">メッセージ</span><span class="sxs-lookup"><span data-stu-id="800df-118">Messages</span></span>                    | <span data-ttu-id="800df-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="800df-119">Mail.Read</span></span>           |
| <span data-ttu-id="800df-120">グループ</span><span class="sxs-lookup"><span data-stu-id="800df-120">Groups</span></span>                      | <span data-ttu-id="800df-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="800df-121">Group.Read.All</span></span>      |
| <span data-ttu-id="800df-122">ユーザー</span><span class="sxs-lookup"><span data-stu-id="800df-122">Users</span></span>                       | <span data-ttu-id="800df-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="800df-123">User.Read.All</span></span>       |
| <span data-ttu-id="800df-124">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="800df-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="800df-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="800df-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="800df-126">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="800df-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="800df-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800df-127">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="800df-128">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="800df-128">Security alert</span></span>| <span data-ttu-id="800df-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800df-129">SecurityEvents.ReadWrite.All</span></span> |

 > <span data-ttu-id="800df-130">**注:**/V1.0 エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="800df-130">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="800df-131">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="800df-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="800df-132">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="800df-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="800df-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="800df-133">Request headers</span></span>

| <span data-ttu-id="800df-134">名前</span><span class="sxs-lookup"><span data-stu-id="800df-134">Name</span></span>       | <span data-ttu-id="800df-135">型</span><span class="sxs-lookup"><span data-stu-id="800df-135">Type</span></span> | <span data-ttu-id="800df-136">説明</span><span class="sxs-lookup"><span data-stu-id="800df-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="800df-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="800df-137">Authorization</span></span>  | <span data-ttu-id="800df-138">string</span><span class="sxs-lookup"><span data-stu-id="800df-138">string</span></span>  | <span data-ttu-id="800df-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="800df-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="800df-141">応答</span><span class="sxs-lookup"><span data-stu-id="800df-141">Response</span></span>

<span data-ttu-id="800df-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="800df-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="800df-143">例</span><span class="sxs-lookup"><span data-stu-id="800df-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="800df-144">要求</span><span class="sxs-lookup"><span data-stu-id="800df-144">Request</span></span>

<span data-ttu-id="800df-145">ユーザーが新しいメールを受信したときに通知を送信する要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="800df-145">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="800df-146">要求の本文には、[サブスクリプション](../resources/subscription.md)オブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="800df-146">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="800df-147">`clientState`フィールドは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="800df-147">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="800df-148">リソースの例</span><span class="sxs-lookup"><span data-stu-id="800df-148">Resources examples</span></span>

<span data-ttu-id="800df-149">以下は、サブスクリプションのリソース プロパティの有効な値です。</span><span class="sxs-lookup"><span data-stu-id="800df-149">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="800df-150">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="800df-150">Resource type</span></span> | <span data-ttu-id="800df-151">例</span><span class="sxs-lookup"><span data-stu-id="800df-151">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="800df-152">メール</span><span class="sxs-lookup"><span data-stu-id="800df-152">Mail</span></span>|<span data-ttu-id="800df-153">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="800df-153">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="800df-154">me/messages</span><span class="sxs-lookup"><span data-stu-id="800df-154">me/messages</span></span>|
|<span data-ttu-id="800df-155">連絡先</span><span class="sxs-lookup"><span data-stu-id="800df-155">Contacts</span></span>|<span data-ttu-id="800df-156">me/contacts</span><span class="sxs-lookup"><span data-stu-id="800df-156">me/contacts</span></span>|
|<span data-ttu-id="800df-157">カレンダー</span><span class="sxs-lookup"><span data-stu-id="800df-157">Calendars</span></span>|<span data-ttu-id="800df-158">me/events</span><span class="sxs-lookup"><span data-stu-id="800df-158">me/events</span></span>|
|<span data-ttu-id="800df-159">ユーザー</span><span class="sxs-lookup"><span data-stu-id="800df-159">Users</span></span>|<span data-ttu-id="800df-160">users</span><span class="sxs-lookup"><span data-stu-id="800df-160">users</span></span>|
|<span data-ttu-id="800df-161">グループ</span><span class="sxs-lookup"><span data-stu-id="800df-161">Groups</span></span>|<span data-ttu-id="800df-162">グループ</span><span class="sxs-lookup"><span data-stu-id="800df-162">groups</span></span>|
|<span data-ttu-id="800df-163">会話</span><span class="sxs-lookup"><span data-stu-id="800df-163">Conversations</span></span>|<span data-ttu-id="800df-164">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="800df-164">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="800df-165">ドライブ</span><span class="sxs-lookup"><span data-stu-id="800df-165">Drives</span></span>|<span data-ttu-id="800df-166">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="800df-166">me/drive/root</span></span>|
|<span data-ttu-id="800df-167">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="800df-167">Security alert</span></span>|<span data-ttu-id="800df-168">セキュリティと警告? $filter eq のステータスを 'New' =</span><span class="sxs-lookup"><span data-stu-id="800df-168">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="800df-169">応答</span><span class="sxs-lookup"><span data-stu-id="800df-169">Response</span></span>

<span data-ttu-id="800df-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="800df-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="800df-173">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="800df-173">Notification endpoint validation</span></span>

<span data-ttu-id="800df-174">サブスクリプション通知エンドポイント (で指定されている、`notificationUrl`プロパティ) の[ユーザー データの変更の通知の設定](/graph/webhooks#notification-endpoint-validation)で説明したように、検証要求に応答できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="800df-174">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="800df-175">検証が失敗した場合、サブスクリプションを作成する要求は 400 不正な要求のエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="800df-175">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
