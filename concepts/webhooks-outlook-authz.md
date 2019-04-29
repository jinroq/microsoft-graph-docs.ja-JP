---
title: Outlookリソースで、不足状態のサブスクリプションと通知を減らす（プレビュー）
description: ユーザーのパスワードのリセットなどのセキュリティイベントのため、Outlookは変更通知の配信を一時停止することがあります。 通知の中断のない配信を確保するために、特別なライフサイクルイベント - `subscriptionRemoved`および`missed`- を処理する必要があります。 　　
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 1c430743f860536ef20fa2ad9974e580c78a6f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32683981"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a><span data-ttu-id="46bd0-104">Outlookリソースで、不足状態のサブスクリプションと通知を減らす（プレビュー）</span><span class="sxs-lookup"><span data-stu-id="46bd0-104">Reduce missing subscriptions and notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="46bd0-105">Outlookリソースの通知を設定しているアプリが、通知設定を削除され通知を見逃すことがあります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-105">Apps subscribing to notifications for Outlook resources may get their subscriptions removed and miss some notifications.</span></span> <span data-ttu-id="46bd0-106">アプリは、検出し、損失から回復するためのロジックを実装して、継続的な通知のフローを再開する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-106">Apps should implement logic to detect and recover from the loss, and resume a continuous notification flow.</span></span>

<span data-ttu-id="46bd0-107">Outlook で特定のイベントでは、サブスクリプションが削除されることがあります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="46bd0-108">これらのイベントには次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-108">These events include:</span></span>

- <span data-ttu-id="46bd0-109">ユーザーパスワードのリセット</span><span class="sxs-lookup"><span data-stu-id="46bd0-109">User's password has been reset</span></span>
- <span data-ttu-id="46bd0-110">ユーザーデバイスの要件未準拠</span><span class="sxs-lookup"><span data-stu-id="46bd0-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="46bd0-111">ユーザーアカウントの取り消し</span><span class="sxs-lookup"><span data-stu-id="46bd0-111">User's account has been revoked</span></span>

<span data-ttu-id="46bd0-112">そのようなイベントが発生すると、Outlookは特別なライフサイクル通知`subscriptionRemoved`を送信します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="46bd0-113">通知をアプリに配信できない場合、Outlookはあらためてもう一度ライフサイクル通知、 `missed`を送信します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-113">Outlook also sends another lifecycle notification, `missed`, if a notification cannot be delivered to an app.</span></span>

<span data-ttu-id="46bd0-114">**メッセージ**や**イベント**などのOutlookリソースの通知を設定しているアプリは、`subscriptionRemoved`や `missed` シグナルを監視する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-114">An app subscribing to notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals:</span></span>

- <span data-ttu-id="46bd0-115">`subscriptionRemoved`通知を受信すると、アプリは継続的な流れを維持するためにサブスクリプションを再作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-115">Upon receiving a `subscriptionRemoved` notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="46bd0-116">`missed` 通知を受信すると、アプリはMicrosoft Graphを使用してリソースデータを再同期する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-116">On receiving a `missed` notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="46bd0-117">ライフサイクル通知を受信するには、既存の**notificationUrl**すでにリソース通知を受信しているエンドポイントを使用するか、あるいは別の**lifecycleNotificationUrl** を登録して、 `subscriptionRemoved` と`missed`通知を別のエンドポイントで受信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives resource notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="46bd0-118">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="46bd0-118">Creating a subscription</span></span>

<span data-ttu-id="46bd0-119">サブスクリプションを作成するときに、**lifecycleNotificationUrl**プロパティを使用して個別の通知エンドポイントを指定できます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-119">When creating a subscription, you can specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="46bd0-120">エンドポイントを指定すると、現在および将来のすべてのタイプのライフサイクル通知がそこに配信されます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="46bd0-121">それ以外の場合、`subscriptionRemoved`と`missed`通知は既存のすべてのサブスクリプションについて既存の**notificationUrl**に配信されます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-121">Otherwise, `subscriptionRemoved` and `missed` notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="46bd0-122">**注意:** 現時点では、 **lifecycleNotificationUrl**プロパティは、Microsoft Graph APIの `beta` バージョンを使用してのみ設定または読み取りができます。　</span><span class="sxs-lookup"><span data-stu-id="46bd0-122">**Note:** At the moment, the **lifecycleNotificationUrl** property can only be set or read using the `beta` version of Microsoft Graph APIs.</span></span> <span data-ttu-id="46bd0-123">ただし、`beta`を使用して作成されたサブスクリプションは `v1.0`と同じ運用環境に格納されるため、`v1.0`の通常の他のサブスクリプションとの使用に加えて、ここで説明する新しいOutlookフローを実装できます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-123">However, subscriptions created using `beta` are stored in the same production environment as `v1.0` so you can implement the new Outlook flow described here in addition to your regular usage of `v1.0` with other subscriptions.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="46bd0-124">サブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="46bd0-124">Subscription request example</span></span>

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
 
> <span data-ttu-id="46bd0-125">**重要:** 両方通知 Url に同じホスト名を使用します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-125">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="46bd0-126">**注意:** [一般的な通知の記事](webhooks.md#managing-subscriptions)で説明されているように、両方の通知エンドポイントを検証する必要があります。　　</span><span class="sxs-lookup"><span data-stu-id="46bd0-126">**Note:** You need to validate both notification endpoints as described in [the generic notification article](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="46bd0-127">両方のエンドポイントに同じURLを使用することを選択した場合は、2つの検証要求を受け取り応答します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-127">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="46bd0-128">**注意:** (`PATCH`) 既存のサブスクリプションを**lifecycleNotificationUrl**プロパティを追加するために更新することはできません。 </span><span class="sxs-lookup"><span data-stu-id="46bd0-128">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="46bd0-129">そのような既存のサブスクリプションを削除し、新しいサブスクリプションを作成して**lifecycleNotificationUrl**プロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-129">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="46bd0-130">**lifecycleNotificationUrl**プロパティのない既存のサブスクリプションは、**notificationUrl**を介して`subscriptionRemoved`および`missed`通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-130">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="46bd0-131">SubscriptionRemoved 通知に応答します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-131">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="46bd0-132">`subscriptionRemoved`通知によって、サブスクリプションが削除されたため再作成する必要があることが通知されますが、通知を継続して受け取りたい場合。</span><span class="sxs-lookup"><span data-stu-id="46bd0-132">The `subscriptionRemoved` notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving notifications.</span></span> 

<span data-ttu-id="46bd0-133">長期間のサブスクリプション（3日など）を作成すると、リソースデータの通知が**notificationUrl**に送信され始めます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-133">You can create a long-lived subscription (e.g. 3 days), and resource data notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="46bd0-134">しかしながら、リソースデータへのアクセスの条件は時間とともに変化し得るので注意が必要です。</span><span class="sxs-lookup"><span data-stu-id="46bd0-134">However, the conditions of access to the resource data may change over time.</span></span> <span data-ttu-id="46bd0-135">たとえば、Outlookサービスでイベントが発生し、アプリでユーザーの再認証が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-135">For example, an event in the Outlook service may occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="46bd0-136">そのような場合、フローは次のようになります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-136">In such a case, the flow looks as follows:</span></span>

1. <span data-ttu-id="46bd0-137">Outlookは、サブスクリプションをMicrosoft Graphから削除する必要があることを検出しました。</span><span class="sxs-lookup"><span data-stu-id="46bd0-137">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    1. <span data-ttu-id="46bd0-138">これらのイベントには決まった頻度があるわけではありません。</span><span class="sxs-lookup"><span data-stu-id="46bd0-138">There is no set cadence for these events.</span></span> <span data-ttu-id="46bd0-139">いくつかのリソースでは頻繁に発生し、他のリソースではほとんど発生しません。</span><span class="sxs-lookup"><span data-stu-id="46bd0-139">They may occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="46bd0-140">Microsoft Graphは `subscriptionRemoved`通知を **lifecycleNotificationUrl** （指定されている場合）、または**notificationUrl**に送信します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-140">Microsoft Graph sends a `subscriptionRemoved` notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="46bd0-141">同じリソースに対して新しいサブスクリプションを作成することで、この通知に応答することができます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-141">You can respond to this notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="46bd0-142">これを行うには、有効なアクセス トークンを提示する必要があります。 場合によっては、アプリは新しい有効なアクセス トークンを取得するためにユーザーを再認証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-142">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="46bd0-143">新しいサブスクリプションを正常に作成すると、リソースの通知が再開されます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-143">If you successfully create a new subscription, resource notifications will start flowing again.</span></span> <span data-ttu-id="46bd0-144">ただし、作成に失敗した場合（たとえば、アプリが有効なアクセス トークンを取得できなかった場合）、リソース通知は送信されません。</span><span class="sxs-lookup"><span data-stu-id="46bd0-144">However, if you fail (for example, the app could not obtain a valid access token), resource notifications will not be sent.</span></span>

5. <span data-ttu-id="46bd0-145">新しいサブスクリプションを作成したら、リソースデータを同期して、不足している変更を特定できます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-145">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="46bd0-146">SubscriptionRemoved 通知の例</span><span class="sxs-lookup"><span data-stu-id="46bd0-146">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="46bd0-147">このタイプの通知について注意することがいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-147">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="46bd0-148">この`"lifecycleEvent": "subscriptionRemoved"`フィールドは、サブスクリプションの削除に関連するものとしてこの通知を指定します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-148">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="46bd0-149">他の種類のライフサイクル通知も可能であり、新しいものが将来導入予定です。</span><span class="sxs-lookup"><span data-stu-id="46bd0-149">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="46bd0-150">通知には特定のリソースに関する情報は含まれていません。リソースの変更とは関係がなく、サブスクリプションの状態の変更のみに関するためです。</span><span class="sxs-lookup"><span data-stu-id="46bd0-150">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="46bd0-151">リソース通知と同様に、ライフサイクル通知はまとめてバッチ処理することができ(**value** 配列内で)、それぞれが異なる**lifecycleEvent**値を持つことがあります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-151">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="46bd0-152">それに応じてバッチ内の各通知を処理します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-152">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="46bd0-153">取るべきアクション</span><span class="sxs-lookup"><span data-stu-id="46bd0-153">Actions to take</span></span>

1. <span data-ttu-id="46bd0-154">`202 - Accepted`でPOST呼び出しに応答して、通知の受信を[確認](webhooks.md#notifications)します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-154">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="46bd0-155">通知の信頼性を[検証します](webhooks.md#notifications)。</span><span class="sxs-lookup"><span data-stu-id="46bd0-155">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="46bd0-156">次のステップに進むために、アプリに有効なアクセス トークンがあることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="46bd0-156">Ensure the app has a valid access token to take the next step.</span></span> 
> <span data-ttu-id="46bd0-157">\*\*注意:[認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) \*\* の1つを使用している場合、有効なキャッシュされたトークンを再利用するか、ユーザーに再度ログインするように要求するなど、新しいトークンを取得することでこれを処理します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-157">**Note:** If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to login again (e.g. with a new password).</span></span> <span data-ttu-id="46bd0-158">アクセスの状況が変化している可能性があり、呼び出し側がリソースデータへのアクセスを許可されなくなっている可能性があるため、新しいトークンの取得が失敗する可能性があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="46bd0-158">Note that obtaining a new token may fail, since the conditions of access may have changed, and the caller may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="46bd0-159">[ここ](webhooks.md#subscription-request-example)に記載されている標準プロセスを使用して、新しいサブスクリプションを作成します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-159">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

> <span data-ttu-id="46bd0-160">**注意:** システムによって実行される承認チェックによって、アプリまたはユーザーによるリソースへのアクセスが拒否される可能性があるため、このアクションは失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-160">**Note:** This action may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="46bd0-161">サブスクリプションを正常に再認証するには、アプリがユーザーから新しいアクセス トークンを取得する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-161">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="46bd0-162">アクセス条件に変化があった場合など、いつでもこれらのアクションを再試行できます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-162">You may retry these actions later, at any time, for example when the conditions of access have change.</span></span> <span data-ttu-id="46bd0-163">ライフサイクル通知が送信されてからアプリがサブスクリプションを正常に再作成するまでの間に発生したリソースの変更はすべて失われます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-163">Any resource changes in the time period from when the lifecycle notification was sent, to when the app re-creates the subscription successfully, will be lost.</span></span> <span data-ttu-id="46bd0-164">アプリは、独自にそれらの変更を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-164">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="46bd0-165">新しいサブスクリプションを作成した後、このリソースに関する通知を受け取った最後の既知の時間から不足しているリソースデータを同期します。 例えば：`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="46bd0-165">After creating the new subscription, sync any missing resource data from the last known time you received a notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="46bd0-166">不在通知に応答します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-166">Responding to missed notifications</span></span>

<span data-ttu-id="46bd0-167">これらのシグナルは、いくつかの通知が配信されなかった可能性があることを知らせます。</span><span class="sxs-lookup"><span data-stu-id="46bd0-167">These signals inform you that some notifications may have not been delivered.</span></span> <span data-ttu-id="46bd0-168">これらのシグナルを無視するか対処するかをあなたは決めなければなりません。</span><span class="sxs-lookup"><span data-stu-id="46bd0-168">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="46bd0-169">通知の例</span><span class="sxs-lookup"><span data-stu-id="46bd0-169">Notification example</span></span>

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

<span data-ttu-id="46bd0-170">このタイプの通知について注意することがいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-170">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="46bd0-171">この`"lifecycleEvent": "missed"`フィールドは、これを見逃し通知に関するシグナルとして指定します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-171">The `"lifecycleEvent": "missed"` field designates this as a signal about missed notifications.</span></span> <span data-ttu-id="46bd0-172">他の種類のライフサイクル通知も可能であり、新しいものが将来導入予定です。</span><span class="sxs-lookup"><span data-stu-id="46bd0-172">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="46bd0-173">通知には特定のリソースに関する情報は含まれていません。リソースの変更とは関係がなく、サブスクリプションの状態の変更のみに関するためです</span><span class="sxs-lookup"><span data-stu-id="46bd0-173">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change</span></span>
- <span data-ttu-id="46bd0-174">リソース通知と同様に、ライフサイクル通知はまとめてバッチ処理することができ(**value** 配列内で)、それぞれが異なる**lifecycleEvent**値を持つことがあります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-174">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="46bd0-175">それに応じてバッチ内の各通知を処理します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-175">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="46bd0-176">取るべきアクション</span><span class="sxs-lookup"><span data-stu-id="46bd0-176">Actions to take</span></span>

1. <span data-ttu-id="46bd0-177">`202 - Accepted`でPOST呼び出しに応答して、通知の受信を[確認](webhooks.md#notifications)します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-177">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
  - <span data-ttu-id="46bd0-178">無視するのであれば、他には何もしないでください。</span><span class="sxs-lookup"><span data-stu-id="46bd0-178">If you ignore these, signals, do nothing else.</span></span> <span data-ttu-id="46bd0-179">そうでない場合は:</span><span class="sxs-lookup"><span data-stu-id="46bd0-179">Otherwise,</span></span>
2. <span data-ttu-id="46bd0-180">通知の信頼性を[検証します](webhooks.md#notifications)。</span><span class="sxs-lookup"><span data-stu-id="46bd0-180">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="46bd0-181">通知として配信されなかった変更を識別するために、リソースの完全データ再同期を実行します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-181">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="46bd0-182">ライフ サイクルの通知を処理するコードを将来的にも有効にする</span><span class="sxs-lookup"><span data-stu-id="46bd0-182">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="46bd0-183">将来的には、Microsoft Graphはより多くの種類のサブスクリプションライフサイクル通知を追加する予定です。</span><span class="sxs-lookup"><span data-stu-id="46bd0-183">In the future Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="46bd0-184">それらは同じエンドポイント: **lifecycleNotificationUrl**にポストされますが、それらは**lifecycleEvent**下では異なる値を持ち、それらが発行されるシナリオに固有の、わずかに異なるスキーマとプロパティーを含むことがあります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-184">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and may contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="46bd0-185">Microsoft Graphが新しいタイプのライフサイクル通知を導入したときにコードが壊れないよう、将来を見込んだ方法で実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46bd0-185">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="46bd0-186">次のようなアプローチをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="46bd0-186">We recommend the following:</span></span>

1. <span data-ttu-id="46bd0-187">**lifecycleEvent**プロパティを使用して、サポートするイベントとして各通知を明示的に識別します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-187">Explicitly identify each notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="46bd0-188">たとえば、特定のイベントを識別するために`"lifecycleEvent": "subscriptionRemoved"` プロパティを探し、それを処理します。</span><span class="sxs-lookup"><span data-stu-id="46bd0-188">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="46bd0-189">将来、より多くの種類のライフサイクル通知ができる可能性があるので、新しいシナリオの通知の発表に注意してください。いえしょう。</span><span class="sxs-lookup"><span data-stu-id="46bd0-189">Watch for announcements of notifications for new scenarions, as there may be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="46bd0-190">アプリでは、アプリが認識しないすべてのライフ サイクル イベントは無視しますが、記録はとって意識していたほうがよいでしょう。</span><span class="sxs-lookup"><span data-stu-id="46bd0-190">In your app, ignore any lifecycle events that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="46bd0-191">あなたの判断で、新しいライフサイクル通知のための関連ドキュメントを調べて、それらのサポートを適切に実装してください。</span><span class="sxs-lookup"><span data-stu-id="46bd0-191">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="46bd0-192">関連項目</span><span class="sxs-lookup"><span data-stu-id="46bd0-192">See also</span></span>

- [<span data-ttu-id="46bd0-193">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="46bd0-193">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="46bd0-194">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="46bd0-194">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="46bd0-195">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="46bd0-195">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="46bd0-196">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="46bd0-196">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="46bd0-197">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="46bd0-197">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
