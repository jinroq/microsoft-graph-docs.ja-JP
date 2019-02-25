---
title: ユーザー データの変更に関する通知の設定
description: Microsoft Graph の API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 545a2470e85d82ad3e56ab99943d7487f5df3ca3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168496"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="9d000-105">ユーザー データの変更に関する通知の設定</span><span class="sxs-lookup"><span data-stu-id="9d000-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="9d000-p102">Microsoft Graph の API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="9d000-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="9d000-109">Microsoft Graph はサブスクリプション要求を受け入れると、サブスクリプションで指定された URL に通知をプッシュします。</span><span class="sxs-lookup"><span data-stu-id="9d000-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="9d000-110">アプリはその後、そのビジネス ロジックに従ってアクションを実行します。</span><span class="sxs-lookup"><span data-stu-id="9d000-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="9d000-111">たとえば、詳細データのフェッチ、そのキャッシュやビューの更新などです。</span><span class="sxs-lookup"><span data-stu-id="9d000-111">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="9d000-112">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="9d000-112">Supported resources</span></span>

<span data-ttu-id="9d000-113">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="9d000-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="9d000-114">Outlook [メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="9d000-114">Outlook [message][]</span></span>
- <span data-ttu-id="9d000-115">Outlook [イベント][]</span><span class="sxs-lookup"><span data-stu-id="9d000-115">Outlook [event][]</span></span>
- <span data-ttu-id="9d000-116">Outlook 個人用[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="9d000-116">Outlook personal [contact][]</span></span>
- <span data-ttu-id="9d000-117">[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="9d000-117">[user][]</span></span>
- <span data-ttu-id="9d000-118">[グループ][]</span><span class="sxs-lookup"><span data-stu-id="9d000-118">[group][]</span></span>
- <span data-ttu-id="9d000-119">Office 365 グループ[会話][]</span><span class="sxs-lookup"><span data-stu-id="9d000-119">[Office 365 group notebooks][]</span></span>
- <span data-ttu-id="9d000-120">ユーザーの個人用 OneDrive 上の_任意のフォルダー_の [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="9d000-120">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="9d000-121">OneDrive for Business 上の_ルート フォルダー_の [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="9d000-121">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="9d000-122">セキュリティの[警告][]</span><span class="sxs-lookup"><span data-stu-id="9d000-122">Security [alert][]</span></span>

<span data-ttu-id="9d000-123">受信トレイなど特定の Outlook フォルダーに対してサブスクリプションを作成できます: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="9d000-123">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="9d000-124">あるいは、最上位レベルのリソース: `me/messages`、`me/contacts`、`me/events`、`users`、または `groups`</span><span class="sxs-lookup"><span data-stu-id="9d000-124">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="9d000-125">あるいは、特定のリソース インスタンス: `users/{id}`、`groups/{id}`、`groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="9d000-125">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="9d000-126">または、ユーザーの個人用 OneDrive 内の任意のフォルダー: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="9d000-126">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="9d000-127">あるいは、Sharepoint/OneDrive for Business ドライブのルート フォルダー: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="9d000-127">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="9d000-128">または、新しい[セキュリティ API](security-concept-overview.md) の警告: `/security/alerts?$filter=status eq ‘New’`、`/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="9d000-128">Or to a new [Security API alert](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="9d000-129">Azure AD リソースの制限</span><span class="sxs-lookup"><span data-stu-id="9d000-129">Azure AD resource limitations</span></span>

<span data-ttu-id="9d000-130">Azure AD ベースのリソース (ユーザー、グループ) には一定の制限が適用され、超過するとエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-130">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="9d000-131">最大サブスクリプションのクォータ:</span><span class="sxs-lookup"><span data-stu-id="9d000-131">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="9d000-132">アプリあたり: 合計 50,000 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="9d000-132">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="9d000-133">テナントあたり: すべてのアプリで合計 35 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="9d000-133">Per tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="9d000-134">アプリとテナントの組み合わせ: 合計 7 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="9d000-134">Per app and tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="9d000-135">Azure AD B2C テナントはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d000-135">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="9d000-136">ユーザー エンティティの通知は、個人用 Microsoft アカウントではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d000-136">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="9d000-137">サブスクリプション ライフタイム</span><span class="sxs-lookup"><span data-stu-id="9d000-137">Subscription lifetime</span></span>

<span data-ttu-id="9d000-138">サブスクリプションのライフタイムには制限があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-138">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="9d000-139">アプリは、有効期限が切れる前にサブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-139">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="9d000-140">そうしない場合、新しいサブスクリプションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-140">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="9d000-141">最長有効期限の一覧については、「[リソースの種類別のサブスクリプションの最大の長さ](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9d000-141">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="9d000-142">また、アプリはいつでも登録を解除して、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="9d000-142">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="9d000-143">サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="9d000-143">Managing subscriptions</span></span>

<span data-ttu-id="9d000-144">クライアントは、サブスクリプションを作成したり、サブスクリプションを更新したり、サブスクリプションを削除したりできます。</span><span class="sxs-lookup"><span data-stu-id="9d000-144">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="9d000-145">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="9d000-145">Creating a subscription</span></span>

<span data-ttu-id="9d000-p105">リソースの通知の受信を開始する最初の手順は、サブスクリプションの作成です。サブスクリプション プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="9d000-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="9d000-148">クライアントは、特定のリソースのサブスクリプション要求 (POST) を送信します。</span><span class="sxs-lookup"><span data-stu-id="9d000-148">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="9d000-149">Microsoft Graph が要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="9d000-149">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="9d000-150">要求が有効な場合、Microsoft Graph は検証トークンを通知 URL に送信します。</span><span class="sxs-lookup"><span data-stu-id="9d000-150">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="9d000-151">要求が無効である場合、Microsoft Graph は、エラー コードと詳細の付いたエラー応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="9d000-151">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="9d000-152">クライアントは、Microsoft Graph に検証トークンを返送します。</span><span class="sxs-lookup"><span data-stu-id="9d000-152">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="9d000-153">Microsoft Graph からクライアントに応答が送信されます。</span><span class="sxs-lookup"><span data-stu-id="9d000-153">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="9d000-154">クライアントは、サブスクリプションに通知を関連付けるために、サブスクリプション ID を格納する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-154">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="9d000-155">サブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="9d000-155">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

<span data-ttu-id="9d000-156">プロパティの `changeType`、`notificationUrl`、`resource`、および `expirationDateTime` は必須です。</span><span class="sxs-lookup"><span data-stu-id="9d000-156">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="9d000-157">プロパティの定義と値については、「[サブスクリプション リソースの種類](/graph/api/resources/subscription?view=graph-rest-1.0)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9d000-157">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="9d000-158">`resource` プロパティは、変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="9d000-158">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="9d000-159">たとえば、特定のメール フォルダーへサブスクリプションを作成できます: `me/mailFolders('inbox')/messages`または、管理者の同意を得たユーザーの代わりに作成できます: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`。</span><span class="sxs-lookup"><span data-stu-id="9d000-159">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="9d000-160">`clientState` は必須ではありませんが、推奨される通知の処理プロセスに準拠するには含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-160">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="9d000-161">このプロパティを設定すると、受け取る通知が Microsoft Graph サービスから来たものであることを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="9d000-161">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="9d000-162">その理由で、このプロパティの値は機密として保たなければならず、使用はアプリケーションと Microsoft Graph サービスのためにのみ限るようにしてください。</span><span class="sxs-lookup"><span data-stu-id="9d000-162">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="9d000-163">処理が正常に終了すると、Microsoft Graph は `201 Created` コードおよび本文内に [サブスクリプション](/graph/api/resources/subscription?view=graph-rest-1.0) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d000-163">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="9d000-164">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="9d000-164">Notification endpoint validation</span></span>

<span data-ttu-id="9d000-165">Microsoft Graph により、サブスクリプション作成の前にサブスクリプション要求の `notificationUrl` プロパティの中で提供される通知エンドポイントが検証されます。</span><span class="sxs-lookup"><span data-stu-id="9d000-165">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="9d000-166">検証プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="9d000-166">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="9d000-167">Microsoft Graph が通知 URL に POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="9d000-167">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="9d000-168">**重要:** `validationToken` はクエリ パラメーターであるため、クライアントが HTTP コーディング プラクティスに従って適切にデコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-168">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="9d000-169">クライアントがトークンをデコードせず、代わりに次の手順で示すエンコードされた値 (応答) を使用する場合、検証は失敗します。</span><span class="sxs-lookup"><span data-stu-id="9d000-169">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="9d000-170">また、トークンの形式は将来予告なしに変更される可能性があるため、クライアントはトークン値を曖昧なものとして処理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-170">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="9d000-171">クライアントは 10 秒以内に次の特性を持つ応答を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-171">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="9d000-172">200 (OK) 状態コード。</span><span class="sxs-lookup"><span data-stu-id="9d000-172">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="9d000-173">コンテンツ タイプは `text/plain` でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9d000-173">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="9d000-174">本文には Microsoft Graph が提供した検証トークンを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-174">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="9d000-175">クライアントは、応答を提供した後は検証トークンを破棄する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-175">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="9d000-176">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="9d000-176">Renewing a subscription</span></span>

<span data-ttu-id="9d000-177">クライアントは、要求時から最大 3 日間の特定の有効期限日を持つサブスクリプションを更新できます。</span><span class="sxs-lookup"><span data-stu-id="9d000-177">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="9d000-178">`expirationDateTime` プロパティは必須です。</span><span class="sxs-lookup"><span data-stu-id="9d000-178">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="9d000-179">サブスクリプションの更新の例</span><span class="sxs-lookup"><span data-stu-id="9d000-179">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="9d000-180">処理が正常に終了すると、Microsoft Graph は `200 OK` コードおよび本文内に [サブスクリプション](/graph/api/resources/subscription?view=graph-rest-1.0) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d000-180">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="9d000-181">サブスクリプション オブジェクトには、新しい `expirationDateTime` 値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9d000-181">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="9d000-182">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="9d000-182">Deleting a subscription</span></span>

<span data-ttu-id="9d000-183">クライアントは、その ID を使用してサブスクリプションを削除することにより、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="9d000-183">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="9d000-184">処理が正常に終了すると、Microsoft Graph は `204 No Content` コードを返します。</span><span class="sxs-lookup"><span data-stu-id="9d000-184">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="9d000-185">通知</span><span class="sxs-lookup"><span data-stu-id="9d000-185">Notifications</span></span>

<span data-ttu-id="9d000-186">クライアントはサブスクリプションを作成した後、通知の受信を開始します。</span><span class="sxs-lookup"><span data-stu-id="9d000-186">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="9d000-187">Microsoft Graph は、リソースに変更が発生すると通知 URL に POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="9d000-187">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="9d000-188">通知が送信されるのは、`created` など、サブスクリプションで指定されているタイプの変更についてのみです。</span><span class="sxs-lookup"><span data-stu-id="9d000-188">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="9d000-189">**注:** 同じリソース タイプを監視し、同じ通知 URL を使用する複数のサブスクリプションを使用している場合、サブスクリプション ID が異なる複数の通知が含まれる POST が送信されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d000-189">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="9d000-190">その POST に含まれるすべての通知が、単一のサブスクリプションに属しているという保証はありません。</span><span class="sxs-lookup"><span data-stu-id="9d000-190">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="9d000-191">通知のプロパティ</span><span class="sxs-lookup"><span data-stu-id="9d000-191">Notification properties</span></span>

<span data-ttu-id="9d000-192">通知オブジェクトには、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="9d000-192">The notification object has the following properties:</span></span>

| <span data-ttu-id="9d000-193">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d000-193">Property</span></span> | <span data-ttu-id="9d000-194">型</span><span class="sxs-lookup"><span data-stu-id="9d000-194">Type</span></span> | <span data-ttu-id="9d000-195">説明</span><span class="sxs-lookup"><span data-stu-id="9d000-195">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="9d000-196">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="9d000-196">subscriptionId</span></span> | <span data-ttu-id="9d000-197">string</span><span class="sxs-lookup"><span data-stu-id="9d000-197">string</span></span> | <span data-ttu-id="9d000-198">通知を生成したサブスクリプションの ID。</span><span class="sxs-lookup"><span data-stu-id="9d000-198">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="9d000-199">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9d000-199">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="9d000-200">dateTime</span><span class="sxs-lookup"><span data-stu-id="9d000-200">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="9d000-201">サブスクリプションの有効期限が切れるとき。</span><span class="sxs-lookup"><span data-stu-id="9d000-201">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="9d000-202">clientState</span><span class="sxs-lookup"><span data-stu-id="9d000-202">clientState</span></span> | <span data-ttu-id="9d000-203">string</span><span class="sxs-lookup"><span data-stu-id="9d000-203">string</span></span> | <span data-ttu-id="9d000-204">サブスクリプション要求で指定された `clientState` プロパティ (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="9d000-204">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="9d000-205">changeType</span><span class="sxs-lookup"><span data-stu-id="9d000-205">changeType</span></span> | <span data-ttu-id="9d000-206">string</span><span class="sxs-lookup"><span data-stu-id="9d000-206">string</span></span> | <span data-ttu-id="9d000-207">通知の原因となったイベントの種類。</span><span class="sxs-lookup"><span data-stu-id="9d000-207">The event type that caused the notification.</span></span> <span data-ttu-id="9d000-208">たとえば、メール受信時は `created`、または読んだメッセージをマークした場合は `updated`。</span><span class="sxs-lookup"><span data-stu-id="9d000-208">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="9d000-209">resource</span><span class="sxs-lookup"><span data-stu-id="9d000-209">resource</span></span> | <span data-ttu-id="9d000-210">string</span><span class="sxs-lookup"><span data-stu-id="9d000-210">string</span></span> | <span data-ttu-id="9d000-211">`https://graph.microsoft.com` に関連するリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="9d000-211">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="9d000-212">resourceData</span><span class="sxs-lookup"><span data-stu-id="9d000-212">resourceData</span></span> | <span data-ttu-id="9d000-213">object</span><span class="sxs-lookup"><span data-stu-id="9d000-213">object</span></span> | <span data-ttu-id="9d000-214">このプロパティの内容は、サブスクリプションの対象となるリソースの種類に応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="9d000-214">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="9d000-215">たとえば、Outlook リソースの場合、`resourceData` には次のフィールドが含まれています:</span><span class="sxs-lookup"><span data-stu-id="9d000-215">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="9d000-216">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d000-216">Property</span></span> | <span data-ttu-id="9d000-217">型</span><span class="sxs-lookup"><span data-stu-id="9d000-217">Type</span></span> | <span data-ttu-id="9d000-218">説明</span><span class="sxs-lookup"><span data-stu-id="9d000-218">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="9d000-219">@odata.type</span><span class="sxs-lookup"><span data-stu-id="9d000-219">@odata.type</span></span> | <span data-ttu-id="9d000-220">string</span><span class="sxs-lookup"><span data-stu-id="9d000-220">string</span></span> | <span data-ttu-id="9d000-221">表しているオブジェクトを記述する、Microsoft Graph の OData エンティティ タイプ。</span><span class="sxs-lookup"><span data-stu-id="9d000-221">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="9d000-222">@odata.id</span><span class="sxs-lookup"><span data-stu-id="9d000-222">@odata.id</span></span> | <span data-ttu-id="9d000-223">string</span><span class="sxs-lookup"><span data-stu-id="9d000-223">string</span></span> | <span data-ttu-id="9d000-224">オブジェクトの OData 識別子。</span><span class="sxs-lookup"><span data-stu-id="9d000-224">The OData identifier of the object.</span></span> |
| <span data-ttu-id="9d000-225">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="9d000-225">@odata.etag</span></span> | <span data-ttu-id="9d000-226">string</span><span class="sxs-lookup"><span data-stu-id="9d000-226">string</span></span> | <span data-ttu-id="9d000-227">オブジェクトのバージョンを表す HTTP エンティティ タグ。</span><span class="sxs-lookup"><span data-stu-id="9d000-227">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="9d000-228">ID</span><span class="sxs-lookup"><span data-stu-id="9d000-228">id</span></span> | <span data-ttu-id="9d000-229">string</span><span class="sxs-lookup"><span data-stu-id="9d000-229">string</span></span> | <span data-ttu-id="9d000-230">オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="9d000-230">The identifier of the object.</span></span> |

> <span data-ttu-id="9d000-231">**注:** `resourceData` で提供される `id` 値は、通知生成時に有効だったものです。</span><span class="sxs-lookup"><span data-stu-id="9d000-231">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="9d000-232">メッセージを別のフォルダーに移動するなど、アクションによっては、通知処理時に `id` が有効でなくなるという結果になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-232">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="9d000-233">通知の例</span><span class="sxs-lookup"><span data-stu-id="9d000-233">Notification example</span></span>

<span data-ttu-id="9d000-234">ユーザーが電子メールを受信すると、Microsoft Graph は次のように通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="9d000-234">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"<long_id_string>"
      }
    }
  ]
}
```

<span data-ttu-id="9d000-235">`value` フィールドはオブジェクトの配列であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="9d000-235">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="9d000-236">キューに多数の通知が入っている場合、Microsoft Graph から、単一の要求の中で複数の項目が送信されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d000-236">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="9d000-237">同じ通知要求の中に、異なる複数のサブスクリプションからの通知が含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d000-237">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="9d000-238">通知の処理</span><span class="sxs-lookup"><span data-stu-id="9d000-238">Processing the notification</span></span>

<span data-ttu-id="9d000-239">アプリの受け取る通知を、それぞれ処理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-239">Each notification received by your app should be processed.</span></span> <span data-ttu-id="9d000-240">アプリが通知を処理するために必要な最小限のタスクは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="9d000-240">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="9d000-241">`clientState` プロパティを検証します。</span><span class="sxs-lookup"><span data-stu-id="9d000-241">Validate the `clientState` property.</span></span> <span data-ttu-id="9d000-242">これは、サブスクリプション作成要求で当初送られた値に一致していなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9d000-242">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="9d000-243">**注:** そうでない場合、これを有効な通知と見なすことはできません。</span><span class="sxs-lookup"><span data-stu-id="9d000-243">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="9d000-244">通知が Microsoft Graph に由来するものでなく、悪意のある者が偽って送った可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-244">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="9d000-245">また、通知の送信元を調査し、適切なアクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-245">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="9d000-246">ビジネス ロジックに基づいて、アプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="9d000-246">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="9d000-247">Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。</span><span class="sxs-lookup"><span data-stu-id="9d000-247">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="9d000-248">Microsoft Graph が 2xx クラス コードを受信しない場合は、通知を何回でも再試行します。</span><span class="sxs-lookup"><span data-stu-id="9d000-248">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="9d000-249">**注:** `clientState`プロパティがサブスクリプション要求のものと一致しない場合でも、`202 - Accepted` ステータス コードを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d000-249">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="9d000-250">これは、偽通知が信頼されていないかもしれないという事実を悪意のある者が検出し、それを利用して `clientState` プロパティの値を類推するのを防ぐことになるため、優れた方法と言えます。</span><span class="sxs-lookup"><span data-stu-id="9d000-250">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="9d000-251">要求内の他の通知について、これらを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="9d000-251">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="9d000-252">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="9d000-252">Code samples</span></span>

<span data-ttu-id="9d000-253">GitHub では、次のコード サンプルを利用できます。</span><span class="sxs-lookup"><span data-stu-id="9d000-253">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="9d000-254">Node.js 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="9d000-254">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="9d000-255">ASP.NET 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="9d000-255">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="9d000-256">WebJobs SDK を使用した Microsoft Graph ユーザー Webhook のサンプル</span><span class="sxs-lookup"><span data-stu-id="9d000-256">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="9d000-257">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d000-257">See also</span></span>

- [<span data-ttu-id="9d000-258">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="9d000-258">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="9d000-259">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="9d000-259">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="9d000-260">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="9d000-260">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[連絡先]: /graph/api/resources/contact?view=graph-rest-1.0
[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[会話]: /graph/api/resources/conversation?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[イベント]: /graph/api/resources/event?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[グループ]: /graph/api/resources/group?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[メッセージ]: /graph/api/resources/message?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[ユーザー]: /graph/api/resources/user?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[警告]: /graph/api/resources/alert?view=graph-rest-1.0
[alert:]: /graph/api/resources/alert?view=graph-rest-1.0
