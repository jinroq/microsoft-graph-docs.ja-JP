---
title: Outlook リソースのサブスクリプションと通知の喪失を減らす (プレビュー)
description: ユーザーのパスワードのリセットなどのセキュリティ イベントが原因で、Outlook で変更通知の配信が一時的に停止されることがあります。 通知の配信が中断されないよう、特殊なライフサイクル イベントである `subscriptionRemoved` および `missed` を処理する必要があります。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 1c430743f860536ef20fa2ad9974e580c78a6f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32683981"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a><span data-ttu-id="64463-104">Outlook リソースのサブスクリプションと通知の喪失を減らす (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="64463-104">Reduce missing subscriptions and notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="64463-105">Outlook リソースの通知の受信登録をしてあるアプリでは、サブスクリプションが削除され、通知が配信されない場合があります。</span><span class="sxs-lookup"><span data-stu-id="64463-105">Apps subscribing to notifications for Outlook resources may get their subscriptions removed and miss some notifications.</span></span> <span data-ttu-id="64463-106">通知の継続的な配信を再開させるには、そのような消失を検出し、設定を復元するためのロジックをアプリで実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="64463-106">Apps should implement logic to detect and recover from the loss, and resume a continuous notification flow.</span></span>

<span data-ttu-id="64463-107">Outlook で特定のイベントが発生すると、サブスクリプションが削除されることがあります。</span><span class="sxs-lookup"><span data-stu-id="64463-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="64463-108">これらのイベントには次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="64463-108">These events include:</span></span>

- <span data-ttu-id="64463-109">ユーザーのパスワードがリセットされた場合</span><span class="sxs-lookup"><span data-stu-id="64463-109">User's password has been reset</span></span>
- <span data-ttu-id="64463-110">ユーザーのデバイスが準拠しなくなった場合</span><span class="sxs-lookup"><span data-stu-id="64463-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="64463-111">ユーザーのアカウントが取り消された場合</span><span class="sxs-lookup"><span data-stu-id="64463-111">User's account has been revoked</span></span>

<span data-ttu-id="64463-112">このようなイベントが発生すると、Outlook は特殊なライフサイクル通知である `subscriptionRemoved` を送信します。</span><span class="sxs-lookup"><span data-stu-id="64463-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="64463-113">通知をアプリに配信できない場合、Outlook は `missed` という別のライフサイクル通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="64463-113">Outlook also sends another lifecycle notification, `missed`, if a notification cannot be delivered to an app.</span></span>

<span data-ttu-id="64463-114">**メッセージ**や**イベント**などの Outlook リソースの受信登録をしてあるアプリでは、`subscriptionRemoved` と `missed` のシグナルが検出されます。</span><span class="sxs-lookup"><span data-stu-id="64463-114">An app subscribing to notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals:</span></span>

- <span data-ttu-id="64463-115">`subscriptionRemoved` 通知を受信すると、継続的な受信を維持できるよう、アプリでサブスクリプションが再作成されます。</span><span class="sxs-lookup"><span data-stu-id="64463-115">Upon receiving a `subscriptionRemoved` notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="64463-116">`missed` 通知を受信した場合は、アプリでは Microsoft Graphを使用してリソース データが再同期されます。</span><span class="sxs-lookup"><span data-stu-id="64463-116">On receiving a `missed` notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="64463-117">ライフサイクル通知を受信するには、すでにリソース通知を受信している既存の **notificationUrl** エンドポイントを使用するか、`subscriptionRemoved` と `missed` 通知を異なるエンドポイントで受信できるように別の **lifecycleNotificationUrl** を登録するかのいずれを行います。</span><span class="sxs-lookup"><span data-stu-id="64463-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives resource notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="64463-118">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="64463-118">Creating a subscription</span></span>

<span data-ttu-id="64463-119">サブスクリプションを作成する際は、**lifecycleNotificationUrl** プロパティを使用して異なる通知エンドポイントを指定できます。</span><span class="sxs-lookup"><span data-stu-id="64463-119">When creating a subscription, you can specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="64463-120">エンドポイントを指定すると、現在および将来のすべてのタイプのライフサイクル通知がそのエンドポイントに配信されます。</span><span class="sxs-lookup"><span data-stu-id="64463-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="64463-121">指定しない場合、既存のすべてのサブスクリプションに関連する `subscriptionRemoved` と `missed` 通知は既存の **notificationUrl** に配信されます。</span><span class="sxs-lookup"><span data-stu-id="64463-121">Otherwise, `subscriptionRemoved` and `missed` notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="64463-122">**注:** 現時点では、**lifecycleNotificationUrl** プロパティの設定または読み取りは、Microsoft Graph APIの `beta` バージョンを使用した場合のみ行えます。</span><span class="sxs-lookup"><span data-stu-id="64463-122">**Note:** At the moment, the **lifecycleNotificationUrl** property can only be set or read using the `beta` version of Microsoft Graph APIs.</span></span> <span data-ttu-id="64463-123">ただし、`beta` を使用して作成されたサブスクリプションは `v1.0`と同じ運用環境に格納されるため、`v1.0` の通常の他のサブスクリプションの使用に加えて、ここで説明する新しい Outlook のフローを実装できます。</span><span class="sxs-lookup"><span data-stu-id="64463-123">However, subscriptions created using `beta` are stored in the same production environment as `v1.0` so you can implement the new Outlook flow described here in addition to your regular usage of `v1.0` with other subscriptions.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="64463-124">サブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="64463-124">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2019-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> <span data-ttu-id="64463-125">**重要:** 両方の通知 URL で同じホスト名を使用します。</span><span class="sxs-lookup"><span data-stu-id="64463-125">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="64463-126">**注:** [通知に関する一般的な記事](webhooks.md#managing-subscriptions)で説明されているように、両方の通知エンドポイントを検証する必要があります。　　</span><span class="sxs-lookup"><span data-stu-id="64463-126">**Note:** You need to validate both notification endpoints as described in [the generic notification article](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="64463-127">両方のエンドポイントに同じ URL を使用することを選択した場合は、検証要求が 2 つ配信されるので、それらに応答します。</span><span class="sxs-lookup"><span data-stu-id="64463-127">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="64463-128">**注:** 既存のサブスクリプションを更新 (`PATCH`) して **lifecycleNotificationUrl** プロパティを追加することはできません。 </span><span class="sxs-lookup"><span data-stu-id="64463-128">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="64463-129">そのような既存のサブスクリプションは削除し、新しいサブスクリプションを作成して **lifecycleNotificationUrl** プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="64463-129">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="64463-130">**lifecycleNotificationUrl** プロパティのない既存のサブスクリプションは、**notificationUrl** 経由で `subscriptionRemoved` と `missed` 通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="64463-130">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="64463-131">SubscriptionRemoved 通知に応答する</span><span class="sxs-lookup"><span data-stu-id="64463-131">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="64463-132">`subscriptionRemoved` 通知は、サブスクリプションが削除され、通知の受信を継続するにはサブスクリプションを再作成する必要があることを通知します。</span><span class="sxs-lookup"><span data-stu-id="64463-132">The `subscriptionRemoved` notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving notifications.</span></span> 

<span data-ttu-id="64463-133">有効期限が長いサブスクリプション（例: 3 日）を作成すると、リソース データの通知の **notificationUrl** への送信が開始されます。</span><span class="sxs-lookup"><span data-stu-id="64463-133">You can create a long-lived subscription (e.g. 3 days), and resource data notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="64463-134">ただし、リソース データへのアクセスの条件は時間の経過とともに変化する可能性があるので注意が必要です。</span><span class="sxs-lookup"><span data-stu-id="64463-134">However, the conditions of access to the resource data may change over time.</span></span> <span data-ttu-id="64463-135">たとえば、アプリでユーザーの再認証が必要になるイベントが Outlook サービスで発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="64463-135">For example, an event in the Outlook service may occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="64463-136">そのような場合、フローは次のようになります。</span><span class="sxs-lookup"><span data-stu-id="64463-136">In such a case, the flow looks as follows:</span></span>

1. <span data-ttu-id="64463-137">Outlook で、Microsoft Graph からサブスクリプションを削除する必要があることが検出されます。</span><span class="sxs-lookup"><span data-stu-id="64463-137">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    1. <span data-ttu-id="64463-138">これらのイベントは、決まった頻度で発生するわけではありません。</span><span class="sxs-lookup"><span data-stu-id="64463-138">There is no set cadence for these events.</span></span> <span data-ttu-id="64463-139">イベントが頻繁に発生するリソースもあれば、ほとんど発生しないリソースもあります。</span><span class="sxs-lookup"><span data-stu-id="64463-139">They may occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="64463-140">Microsoft Graph が `subscriptionRemoved` 通知を **lifecycleNotificationUrl** (指定されている場合) または **notificationUrl** に送信します。</span><span class="sxs-lookup"><span data-stu-id="64463-140">Microsoft Graph sends a `subscriptionRemoved` notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="64463-141">この通知には、同じリソースに対して新しいサブスクリプションを作成することにより応答できます。</span><span class="sxs-lookup"><span data-stu-id="64463-141">You can respond to this notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="64463-142">これを行うには、有効なアクセス トークンを提示する必要があります。新しい有効なアクセス トークンを取得するために、アプリでユーザーを再認証する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="64463-142">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="64463-143">新しいサブスクリプションを正常に作成すると、リソース通知の配信が再開されます。</span><span class="sxs-lookup"><span data-stu-id="64463-143">If you successfully create a new subscription, resource notifications will start flowing again.</span></span> <span data-ttu-id="64463-144">作成に失敗した場合 (たとえば、アプリが有効なアクセス トークンを取得できなかった場合)、リソース通知は送信されません。</span><span class="sxs-lookup"><span data-stu-id="64463-144">However, if you fail (for example, the app could not obtain a valid access token), resource notifications will not be sent.</span></span>

5. <span data-ttu-id="64463-145">新しいサブスクリプションを作成したら、喪失した変更を特定するためにリソース データを同期できます。</span><span class="sxs-lookup"><span data-stu-id="64463-145">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="64463-146">SubscriptionRemoved 通知の例</span><span class="sxs-lookup"><span data-stu-id="64463-146">subscriptionRemoved notification example</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "subscriptionRemoved"
    }
  ]
}
```

<span data-ttu-id="64463-147">このタイプの通知にはいくつかの注意点があります。</span><span class="sxs-lookup"><span data-stu-id="64463-147">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="64463-148">`"lifecycleEvent": "subscriptionRemoved"` フィールドは、この通知はサブスクリプションの削除に関連したものであることを示します。</span><span class="sxs-lookup"><span data-stu-id="64463-148">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="64463-149">他の種類のライフサイクル通知が配信される可能性もあり、今後は新しい通知が導入される予定です。</span><span class="sxs-lookup"><span data-stu-id="64463-149">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="64463-150">通知には特定のリソースに関する情報は含まれていません。通知はサブスクリプションの状態の変更に関するもので、リソースの変更とは関係がないためです。</span><span class="sxs-lookup"><span data-stu-id="64463-150">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="64463-151">リソース通知と同様に、ライフサイクル通知はバッチ処理でき (**value** 配列内で)、それぞれの通知は異なる **lifecycleEvent** 値を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="64463-151">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="64463-152">バッチ内の各通知を適切に処理します。</span><span class="sxs-lookup"><span data-stu-id="64463-152">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="64463-153">必要なアクション</span><span class="sxs-lookup"><span data-stu-id="64463-153">Actions to take</span></span>

1. <span data-ttu-id="64463-154">POST 呼び出しに `202 - Accepted` で応答し、通知の受信を[確認通知](webhooks.md#notifications)します。</span><span class="sxs-lookup"><span data-stu-id="64463-154">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="64463-155">通知の信頼性を[検証します](webhooks.md#notifications)。</span><span class="sxs-lookup"><span data-stu-id="64463-155">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="64463-156">次のステップに進むために必要な有効なアクセス トークンがアプリにあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="64463-156">Ensure the app has a valid access token to take the next step.</span></span> 
> <span data-ttu-id="64463-157">**注:** いずれかの[認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)を使用している場合、その認証ライブラリは、有効なキャッシュされたトークンを再利用するか、ユーザーに再度ログイン (新しいパスワードなどで) するよう要求するなどして新しいトークンを取得することにより、トークンを処理します。</span><span class="sxs-lookup"><span data-stu-id="64463-157">**Note:** If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to login again (e.g. with a new password).</span></span> <span data-ttu-id="64463-158">アクセスの状況の変化などの理由により呼び出し側がリソース データへのアクセス許可を失っている場合があるため、新しいトークンの取得が失敗する可能性があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="64463-158">Note that obtaining a new token may fail, since the conditions of access may have changed, and the caller may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="64463-159">[こちら](webhooks.md#subscription-request-example)に記載されている標準的な手順に従って、新しいサブスクリプションを作成します。</span><span class="sxs-lookup"><span data-stu-id="64463-159">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

> <span data-ttu-id="64463-160">**注:** システムが実行する承認チェックによりアプリまたはユーザーのリソースへのアクセスが拒否される可能性があるため、このアクションは失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="64463-160">**Note:** This action may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="64463-161">サブスクリプションを正常に再認証するには、アプリはユーザーから新しいアクセス トークンを取得する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="64463-161">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="64463-162">アクセス条件に変更があった場合などは、これらのアクションはいつでも再試行できます。</span><span class="sxs-lookup"><span data-stu-id="64463-162">You may retry these actions later, at any time, for example when the conditions of access have change.</span></span> <span data-ttu-id="64463-163">ライフサイクル通知が送信されてからアプリがサブスクリプションを正常に再作成するまでの間に発生したリソースの変更は、すべて失われます。</span><span class="sxs-lookup"><span data-stu-id="64463-163">Any resource changes in the time period from when the lifecycle notification was sent, to when the app re-creates the subscription successfully, will be lost.</span></span> <span data-ttu-id="64463-164">アプリは、それらの変更を独自に取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="64463-164">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="64463-165">新しいサブスクリプションを作成した後、このリソースに関する通知を受け取った最後の既知の時間以降の受信できなかったリソース データを同期します。 例: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="64463-165">After creating the new subscription, sync any missing resource data from the last known time you received a notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="64463-166">受信できなかった通知への応答</span><span class="sxs-lookup"><span data-stu-id="64463-166">Responding to missed notifications</span></span>

<span data-ttu-id="64463-167">これらのシグナルは、配信されなかった可能性がある通知があることを知らせます。</span><span class="sxs-lookup"><span data-stu-id="64463-167">These signals inform you that some notifications may have not been delivered.</span></span> <span data-ttu-id="64463-168">これらのシグナルを無視するか対処するかを決めます。</span><span class="sxs-lookup"><span data-stu-id="64463-168">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="64463-169">通知の例</span><span class="sxs-lookup"><span data-stu-id="64463-169">Notification example</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "missed"
    }
  ]
}
```

<span data-ttu-id="64463-170">このタイプの通知にはいくつかの注意点があります。</span><span class="sxs-lookup"><span data-stu-id="64463-170">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="64463-171">この`"lifecycleEvent": "missed"` フィールドは、この通知は "missed" (受信出来なかった) 通知に関するシグナルであることを示します。</span><span class="sxs-lookup"><span data-stu-id="64463-171">The `"lifecycleEvent": "missed"` field designates this as a signal about missed notifications.</span></span> <span data-ttu-id="64463-172">他の種類のライフサイクル通知が配信される可能性もあり、今後は新しい通知が導入される予定です。</span><span class="sxs-lookup"><span data-stu-id="64463-172">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="64463-173">通知には特定のリソースに関する情報は含まれていません。通知はサブスクリプションの状態の変更に関するもので、リソースの変更とは関係がないためです。</span><span class="sxs-lookup"><span data-stu-id="64463-173">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change</span></span>
- <span data-ttu-id="64463-174">リソース通知と同様に、ライフサイクル通知はバッチ処理でき (**value** 配列内で)、それぞれの通知は異なる **lifecycleEvent** 値を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="64463-174">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="64463-175">バッチ内の各通知を適切に処理します。</span><span class="sxs-lookup"><span data-stu-id="64463-175">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="64463-176">必要なアクション</span><span class="sxs-lookup"><span data-stu-id="64463-176">Actions to take</span></span>

1. <span data-ttu-id="64463-177">POST 呼び出しに `202 - Accepted` で応答し、通知の受信を[確認通知](webhooks.md#notifications)します。</span><span class="sxs-lookup"><span data-stu-id="64463-177">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
  - <span data-ttu-id="64463-178">シグナルを無視する場合は、特に操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="64463-178">If you ignore these, signals, do nothing else.</span></span> <span data-ttu-id="64463-179">無視しない場合は:</span><span class="sxs-lookup"><span data-stu-id="64463-179">Otherwise,</span></span>
2. <span data-ttu-id="64463-180">通知の信頼性を[検証します](webhooks.md#notifications)。</span><span class="sxs-lookup"><span data-stu-id="64463-180">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="64463-181">通知として配信されなかった変更を特定するために、すべてのデータを対象にリソースの再同期を実行します。</span><span class="sxs-lookup"><span data-stu-id="64463-181">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="64463-182">コードが今後もライフサイクル通知を処理できるようにする</span><span class="sxs-lookup"><span data-stu-id="64463-182">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="64463-183">Microsoft Graph では今後、より多くの種類のサブスクリプション ライフサイクル通知が追加される予定です。</span><span class="sxs-lookup"><span data-stu-id="64463-183">In the future Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="64463-184">これらの通知はこれまでと同じエンドポイント (**lifecycleNotificationUrl**) にポストされますが、通知の **lifecycleEvent** の値が変更され、通知を発行する目的のシナリオに固有の、これまでとはわずかに異なるスキーマとプロパティが含まれる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="64463-184">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and may contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="64463-185">Microsoft Graph に新しい種類のライフサイクル通知が導入された場合でもコードが正常に動作するよう、コードは将来を見込んだ方法で実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="64463-185">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="64463-186">次のようなアプローチをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="64463-186">We recommend the following:</span></span>

1. <span data-ttu-id="64463-187">**lifecycleEvent** プロパティを使用して、サポートするイベントとして各通知を明示的に識別します。</span><span class="sxs-lookup"><span data-stu-id="64463-187">Explicitly identify each notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="64463-188">たとえば、特定のイベントを識別するために `"lifecycleEvent": "subscriptionRemoved"` プロパティを探し、それを処理します。</span><span class="sxs-lookup"><span data-stu-id="64463-188">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="64463-189">今後より多くの種類のライフサイクル通知が導入される可能性があるため、新しいシナリオの通知の発表を見まもるようにします。</span><span class="sxs-lookup"><span data-stu-id="64463-189">Watch for announcements of notifications for new scenarions, as there may be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="64463-190">アプリでは、アプリが認識しないすべてのライフサイクル イベントを無視するようにしますが、今後の参考にするために記録を残します。</span><span class="sxs-lookup"><span data-stu-id="64463-190">In your app, ignore any lifecycle events that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="64463-191">必要と判断する場合は、新しいライフサイクル通知に関連する資料を確認し、適切なサポートを実装します。</span><span class="sxs-lookup"><span data-stu-id="64463-191">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="64463-192">関連項目</span><span class="sxs-lookup"><span data-stu-id="64463-192">See also</span></span>

- [<span data-ttu-id="64463-193">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="64463-193">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="64463-194">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="64463-194">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="64463-195">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="64463-195">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="64463-196">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="64463-196">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="64463-197">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="64463-197">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
