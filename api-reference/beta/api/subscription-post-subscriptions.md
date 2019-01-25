---
title: サブスクリプションを作成する
description: Graph リソース上のデータが変更されたときに通知を受信するリスナー アプリケーションをサブスクライブします。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 002dd88c7db2650be2303e7df6f86ce9a5fbdaa9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527578"
---
# <a name="create-subscription"></a><span data-ttu-id="4784e-103">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="4784e-103">Create subscription</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4784e-104">Graph リソース上のデータが変更されたときに通知を受信するリスナー アプリケーションをサブスクライブします。</span><span class="sxs-lookup"><span data-stu-id="4784e-104">Subscribes a listener application to receive notifications when data on a Microsoft Graph resource changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="4784e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4784e-105">Permissions</span></span>

<span data-ttu-id="4784e-106">サブスクリプションを作成するには、アプリケーションが通知を受信するリソースの読み取り権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="4784e-106">Creating a subscription requires read permission to the resource for which the app will receive notifications.</span></span> <span data-ttu-id="4784e-107">たとえば、メッセージに関する通知を取得するには、アプリが必要な`Mail.Read`のアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="4784e-107">For example, to get notifications about Messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="4784e-108">次の表に、各リソースに必要な、推奨されるアクセス許可を示します。</span><span class="sxs-lookup"><span data-stu-id="4784e-108">The following table lists the suggested permission needed for each resource.</span></span> <span data-ttu-id="4784e-109">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4784e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4784e-110">リソースの種類/項目</span><span class="sxs-lookup"><span data-stu-id="4784e-110">Resource type / Item</span></span>        | <span data-ttu-id="4784e-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4784e-111">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="4784e-112">連絡先</span><span class="sxs-lookup"><span data-stu-id="4784e-112">Contacts</span></span>                    | <span data-ttu-id="4784e-113">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4784e-113">Contacts.Read</span></span>       |
| <span data-ttu-id="4784e-114">スレッド</span><span class="sxs-lookup"><span data-stu-id="4784e-114">Conversations</span></span>               | <span data-ttu-id="4784e-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4784e-115">Group.Read.All</span></span>      |
| <span data-ttu-id="4784e-116">イベント</span><span class="sxs-lookup"><span data-stu-id="4784e-116">Events</span></span>                      | <span data-ttu-id="4784e-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4784e-117">Calendars.Read</span></span>      |
| <span data-ttu-id="4784e-118">メッセージ</span><span class="sxs-lookup"><span data-stu-id="4784e-118">Messages</span></span>                    | <span data-ttu-id="4784e-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4784e-119">Mail.Read</span></span>           |
| <span data-ttu-id="4784e-120">グループ</span><span class="sxs-lookup"><span data-stu-id="4784e-120">Groups</span></span>                      | <span data-ttu-id="4784e-121">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4784e-121">Group.Read.All</span></span>      |
| <span data-ttu-id="4784e-122">ユーザー</span><span class="sxs-lookup"><span data-stu-id="4784e-122">Users</span></span>                       | <span data-ttu-id="4784e-123">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4784e-123">User.Read.All</span></span>       |
| <span data-ttu-id="4784e-124">ドライブ (ユーザーの OneDrive)</span><span class="sxs-lookup"><span data-stu-id="4784e-124">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="4784e-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4784e-125">Files.ReadWrite</span></span>     |
| <span data-ttu-id="4784e-126">ドライブ (共有、SharePoint コンテンツおよびドライブ)</span><span class="sxs-lookup"><span data-stu-id="4784e-126">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="4784e-127">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4784e-127">Files.ReadWrite.All</span></span> |
| <span data-ttu-id="4784e-128">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="4784e-128">Security alert</span></span>              | <span data-ttu-id="4784e-129">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4784e-129">SecurityEvents.ReadWrite.All</span></span> |

> <span data-ttu-id="4784e-130">**注:**/Beta エンドポイントでは、リソースのほとんどのアプリケーションのアクセス許可を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4784e-130">**Note:** The /beta endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="4784e-131">ドライブ ルート アイテムがグループ化して OneDrive での会話は、アプリケーションのアクセス許可ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4784e-131">Conversations in a Group and OneDrive drive root items are not supported with application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="4784e-132">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4784e-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="4784e-133">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4784e-133">Request headers</span></span>

| <span data-ttu-id="4784e-134">名前</span><span class="sxs-lookup"><span data-stu-id="4784e-134">Name</span></span>       | <span data-ttu-id="4784e-135">型</span><span class="sxs-lookup"><span data-stu-id="4784e-135">Type</span></span> | <span data-ttu-id="4784e-136">説明</span><span class="sxs-lookup"><span data-stu-id="4784e-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4784e-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="4784e-137">Authorization</span></span>  | <span data-ttu-id="4784e-138">string</span><span class="sxs-lookup"><span data-stu-id="4784e-138">string</span></span>  | <span data-ttu-id="4784e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4784e-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4784e-141">応答</span><span class="sxs-lookup"><span data-stu-id="4784e-141">Response</span></span>

<span data-ttu-id="4784e-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文に入った [subscription](../resources/subscription.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4784e-142">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4784e-143">例</span><span class="sxs-lookup"><span data-stu-id="4784e-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4784e-144">要求</span><span class="sxs-lookup"><span data-stu-id="4784e-144">Request</span></span>

<span data-ttu-id="4784e-145">要求の本文には、[サブスクリプション](../resources/subscription.md)オブジェクトを JSON 表現したものを指定します。</span><span class="sxs-lookup"><span data-stu-id="4784e-145">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="4784e-146">`clientState`フィールドは省略可能です。</span><span class="sxs-lookup"><span data-stu-id="4784e-146">The `clientState` field is optional.</span></span>

<span data-ttu-id="4784e-147">このサンプル リクエストは、現在サインインしているユーザーが受信したメールの通知のサブスクリプションを作成します。</span><span class="sxs-lookup"><span data-stu-id="4784e-147">This sample request creates a subscription for notifications about new mail received by the currently signed in user.</span></span>
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

<span data-ttu-id="4784e-148">リソース プロパティの設定値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="4784e-148">The following are valid values for the resource property:</span></span>

| <span data-ttu-id="4784e-149">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4784e-149">Resource type</span></span> | <span data-ttu-id="4784e-150">例</span><span class="sxs-lookup"><span data-stu-id="4784e-150">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="4784e-151">メール</span><span class="sxs-lookup"><span data-stu-id="4784e-151">Mail</span></span>|<span data-ttu-id="4784e-152">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="4784e-152">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="4784e-153">me/messages</span><span class="sxs-lookup"><span data-stu-id="4784e-153">me/messages</span></span>|
|<span data-ttu-id="4784e-154">連絡先</span><span class="sxs-lookup"><span data-stu-id="4784e-154">Contacts</span></span>|<span data-ttu-id="4784e-155">me/contacts</span><span class="sxs-lookup"><span data-stu-id="4784e-155">me/contacts</span></span>|
|<span data-ttu-id="4784e-156">カレンダー</span><span class="sxs-lookup"><span data-stu-id="4784e-156">Calendars</span></span>|<span data-ttu-id="4784e-157">me/events</span><span class="sxs-lookup"><span data-stu-id="4784e-157">me/events</span></span>|
|<span data-ttu-id="4784e-158">ユーザー</span><span class="sxs-lookup"><span data-stu-id="4784e-158">Users</span></span>|<span data-ttu-id="4784e-159">users</span><span class="sxs-lookup"><span data-stu-id="4784e-159">users</span></span>|
|<span data-ttu-id="4784e-160">グループ</span><span class="sxs-lookup"><span data-stu-id="4784e-160">Groups</span></span>|<span data-ttu-id="4784e-161">グループ</span><span class="sxs-lookup"><span data-stu-id="4784e-161">groups</span></span>|
|<span data-ttu-id="4784e-162">会話</span><span class="sxs-lookup"><span data-stu-id="4784e-162">Conversations</span></span>|<span data-ttu-id="4784e-163">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="4784e-163">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="4784e-164">ドライブ</span><span class="sxs-lookup"><span data-stu-id="4784e-164">Drives</span></span>|<span data-ttu-id="4784e-165">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="4784e-165">me/drive/root</span></span>|
|<span data-ttu-id="4784e-166">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="4784e-166">Security alert</span></span>|<span data-ttu-id="4784e-167">セキュリティと警告? $filter eq のステータスを 'New' =</span><span class="sxs-lookup"><span data-stu-id="4784e-167">security/alerts?$filter=status eq ‘New’</span></span>|

##### <a name="response"></a><span data-ttu-id="4784e-168">応答</span><span class="sxs-lookup"><span data-stu-id="4784e-168">Response</span></span>

<span data-ttu-id="4784e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4784e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="notification-endpoint-validation"></a><span data-ttu-id="4784e-172">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="4784e-172">Notification endpoint validation</span></span>

<span data-ttu-id="4784e-173">サブスクリプション通知エンドポイント (で指定されている、`notificationUrl`プロパティ) の[ユーザー データの変更の通知の設定](/graph/webhooks#notification-endpoint-validation)で説明したように、検証要求に応答できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="4784e-173">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="4784e-174">検証が失敗した場合、サブスクリプションを作成する要求は 400 不正な要求のエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="4784e-174">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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
