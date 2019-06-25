---
title: ユーザー データの変更に関する通知の設定
description: Microsoft Graph の API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 43e4e4893cae46bb5d3bcecc1f0d7e96da4ccfed
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133783"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="659f3-105">ユーザー データの変更に関する通知の設定</span><span class="sxs-lookup"><span data-stu-id="659f3-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="659f3-p102">Microsoft Graph の API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="659f3-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="659f3-109">Microsoft Graph はサブスクリプション要求を受け入れると、サブスクリプションで指定された URL に通知をプッシュします。</span><span class="sxs-lookup"><span data-stu-id="659f3-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="659f3-110">アプリはその後、そのビジネス ロジックに従ってアクションを実行します。</span><span class="sxs-lookup"><span data-stu-id="659f3-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="659f3-111">たとえば、詳細データのフェッチ、そのキャッシュやビューの更新などです。</span><span class="sxs-lookup"><span data-stu-id="659f3-111">For example, it fetches more data, updates its cache and views, etc.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="659f3-112">.NET Core を使った Webhook アプリの作成</span><span class="sxs-lookup"><span data-stu-id="659f3-112">Build a webhook app with .NET Core</span></span>](/graph/tutorials/change-notifications)

## <a name="supported-resources"></a><span data-ttu-id="659f3-113">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="659f3-113">Supported resources</span></span>

<span data-ttu-id="659f3-114">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="659f3-114">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="659f3-115">Outlook [メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="659f3-115">Outlook [message][]</span></span>
- <span data-ttu-id="659f3-116">Outlook [イベント][]</span><span class="sxs-lookup"><span data-stu-id="659f3-116">Outlook [event][]</span></span>
- <span data-ttu-id="659f3-117">Outlook 個人用[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="659f3-117">Outlook personal [contact][]</span></span>
- <span data-ttu-id="659f3-118">[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="659f3-118">[user][]</span></span>
- <span data-ttu-id="659f3-119">[グループ][]</span><span class="sxs-lookup"><span data-stu-id="659f3-119">[group][]</span></span>
- <span data-ttu-id="659f3-120">Office 365 グループ[会話][]</span><span class="sxs-lookup"><span data-stu-id="659f3-120">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="659f3-121">ユーザーの個人用 OneDrive 上の_任意のフォルダーの_ [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="659f3-121">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="659f3-122">OneDrive for Business 上の_ルート フォルダーの _ [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="659f3-122">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="659f3-123">セキュリティの[警告][]</span><span class="sxs-lookup"><span data-stu-id="659f3-123">Security [alert][]</span></span>

<span data-ttu-id="659f3-124">受信トレイなど特定の Outlook フォルダーに対してサブスクリプションを作成できます: `me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="659f3-124">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="659f3-125">あるいは、最上位レベルのリソース: `me/messages`、`me/contacts`、`me/events`、`users`、または `groups`</span><span class="sxs-lookup"><span data-stu-id="659f3-125">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="659f3-126">あるいは、特定のリソース インスタンス: `users/{id}`、`groups/{id}`、`groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="659f3-126">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="659f3-127">または、ユーザーの個人用 OneDrive 内の任意のフォルダー: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="659f3-127">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="659f3-128">あるいは、Sharepoint/OneDrive for Business ドライブのルート フォルダー: `/drive/root`</span><span class="sxs-lookup"><span data-stu-id="659f3-128">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="659f3-129">または、新しい[セキュリティ API](security-concept-overview.md) の警告: `/security/alerts?$filter=status eq ‘New’`、`/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="659f3-129">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="659f3-130">Azure AD リソースの制限</span><span class="sxs-lookup"><span data-stu-id="659f3-130">Azure AD resource limitations</span></span>

<span data-ttu-id="659f3-131">Azure AD ベースのリソース (ユーザー、グループ) には一定の制限が適用され、超過するとエラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="659f3-131">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="659f3-132">**注:** これらの制限は、Azure AD 以外のサービスのリソースには適用されません。</span><span class="sxs-lookup"><span data-stu-id="659f3-132">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="659f3-133">たとえば、アプリは `message` または `event` リソースに対して、より多くのサブスクリプションを作成できます。これらは Microsoft Graph の一部として Exchange Online サービスでサポートされているものです。</span><span class="sxs-lookup"><span data-stu-id="659f3-133">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="659f3-134">最大サブスクリプションのクォータ:</span><span class="sxs-lookup"><span data-stu-id="659f3-134">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="659f3-135">アプリあたり: 合計 50,000 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="659f3-135">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="659f3-136">テナントあたり: すべてのアプリで合計 1000 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="659f3-136">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="659f3-137">アプリとテナントの組み合わせ: 合計 100 サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="659f3-137">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="659f3-138">制限を超えると、サブスクリプションを作成しようとして、[エラー応答](errors.md) - `403 Forbidden` が発生します。</span><span class="sxs-lookup"><span data-stu-id="659f3-138">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="659f3-139">`message` プロパティは、どの制限が超過しているかを説明します。</span><span class="sxs-lookup"><span data-stu-id="659f3-139">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="659f3-140">Azure AD B2C テナントはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="659f3-140">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="659f3-141">ユーザー エンティティの通知は、個人用 Microsoft アカウントではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="659f3-141">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="659f3-142">サブスクリプション ライフタイム</span><span class="sxs-lookup"><span data-stu-id="659f3-142">Subscription lifetime</span></span>

<span data-ttu-id="659f3-143">サブスクリプションのライフタイムには制限があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-143">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="659f3-144">アプリは、有効期限が切れる前にサブスクリプションを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-144">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="659f3-145">そうしない場合、新しいサブスクリプションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-145">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="659f3-146">最長有効期限の一覧については、「[リソースの種類別のサブスクリプションの最大の長さ](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="659f3-146">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="659f3-147">また、アプリはいつでも登録を解除して、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="659f3-147">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="659f3-148">サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="659f3-148">Managing subscriptions</span></span>

<span data-ttu-id="659f3-149">クライアントは、サブスクリプションを作成したり、サブスクリプションを更新したり、サブスクリプションを削除したりできます。</span><span class="sxs-lookup"><span data-stu-id="659f3-149">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="659f3-150">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="659f3-150">Creating a subscription</span></span>

<span data-ttu-id="659f3-p107">リソースの通知の受信を開始する最初の手順は、サブスクリプションの作成です。サブスクリプション プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="659f3-p107">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="659f3-153">クライアントは、特定のリソースのサブスクリプション要求 (POST) を送信します。</span><span class="sxs-lookup"><span data-stu-id="659f3-153">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="659f3-154">Microsoft Graph が要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="659f3-154">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="659f3-155">要求が有効な場合、Microsoft Graph は検証トークンを通知 URL に送信します。</span><span class="sxs-lookup"><span data-stu-id="659f3-155">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="659f3-156">要求が無効である場合、Microsoft Graph は、エラー コードと詳細の付いたエラー応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="659f3-156">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="659f3-157">クライアントは、Microsoft Graph に検証トークンを返送します。</span><span class="sxs-lookup"><span data-stu-id="659f3-157">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="659f3-158">Microsoft Graph からクライアントに応答が送信されます。</span><span class="sxs-lookup"><span data-stu-id="659f3-158">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="659f3-159">クライアントは、サブスクリプションに通知を関連付けるために、サブスクリプション ID を格納する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-159">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="659f3-160">サブスクリプション要求の例</span><span class="sxs-lookup"><span data-stu-id="659f3-160">Subscription request example</span></span>

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

<span data-ttu-id="659f3-161">プロパティの `changeType`、`notificationUrl`、`resource`、および `expirationDateTime` は必須です。</span><span class="sxs-lookup"><span data-stu-id="659f3-161">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="659f3-162">プロパティの定義と値については、「[サブスクリプション リソースの種類](/graph/api/resources/subscription?view=graph-rest-1.0)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="659f3-162">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="659f3-163">`resource` プロパティは、変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="659f3-163">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="659f3-164">たとえば、特定のメール フォルダーへサブスクリプションを作成できます: `me/mailFolders('inbox')/messages`または、管理者の同意を得たユーザーの代わりに作成できます: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`。</span><span class="sxs-lookup"><span data-stu-id="659f3-164">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="659f3-165">`clientState` は必須ではありませんが、推奨される通知の処理プロセスに準拠するには含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-165">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="659f3-166">このプロパティを設定すると、受け取る通知が Microsoft Graph サービスから来たものであることを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="659f3-166">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="659f3-167">その理由で、このプロパティの値は機密として保たなければならず、使用はアプリケーションと Microsoft Graph サービスのためにのみ限るようにしてください。</span><span class="sxs-lookup"><span data-stu-id="659f3-167">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="659f3-168">処理が正常に終了すると、Microsoft Graph は `201 Created` コードおよび本文内に [サブスクリプション](/graph/api/resources/subscription?view=graph-rest-1.0) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="659f3-168">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="659f3-169">通知エンドポイントの検証</span><span class="sxs-lookup"><span data-stu-id="659f3-169">Notification endpoint validation</span></span>

<span data-ttu-id="659f3-170">Microsoft Graph により、サブスクリプション作成の前にサブスクリプション要求の `notificationUrl` プロパティの中で提供される通知エンドポイントが検証されます。</span><span class="sxs-lookup"><span data-stu-id="659f3-170">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="659f3-171">検証プロセスは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="659f3-171">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="659f3-172">Microsoft Graph が通知 URL に POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="659f3-172">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="659f3-173">**重要:** `validationToken` はクエリ パラメーターであるため、クライアントが HTTP コーディング プラクティスに従って適切にデコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-173">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="659f3-174">クライアントがトークンをデコードせず、代わりに次の手順で示すエンコードされた値 (応答) を使用する場合、検証は失敗します。</span><span class="sxs-lookup"><span data-stu-id="659f3-174">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="659f3-175">また、トークンの形式は将来予告なしに変更される可能性があるため、クライアントはトークン値を曖昧なものとして処理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-175">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="659f3-176">クライアントは 10 秒以内に次の特性を持つ応答を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-176">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="659f3-177">200 (OK) 状態コード。</span><span class="sxs-lookup"><span data-stu-id="659f3-177">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="659f3-178">コンテンツ タイプは `text/plain` でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="659f3-178">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="659f3-179">本文には Microsoft Graph が提供した検証トークンを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-179">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="659f3-180">クライアントは、応答を提供した後は検証トークンを破棄する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-180">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="659f3-181">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="659f3-181">Renewing a subscription</span></span>

<span data-ttu-id="659f3-182">クライアントは、要求時から最大 3 日間の特定の有効期限日を持つサブスクリプションを更新できます。</span><span class="sxs-lookup"><span data-stu-id="659f3-182">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="659f3-183">`expirationDateTime` プロパティは必須です。</span><span class="sxs-lookup"><span data-stu-id="659f3-183">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="659f3-184">サブスクリプションの更新の例</span><span class="sxs-lookup"><span data-stu-id="659f3-184">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="659f3-185">処理が正常に終了すると、Microsoft Graph は `200 OK` コードおよび本文内に [サブスクリプション](/graph/api/resources/subscription?view=graph-rest-1.0) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="659f3-185">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="659f3-186">サブスクリプション オブジェクトには、新しい `expirationDateTime` 値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="659f3-186">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="659f3-187">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="659f3-187">Deleting a subscription</span></span>

<span data-ttu-id="659f3-188">クライアントは、その ID を使用してサブスクリプションを削除することにより、通知の受信を停止できます。</span><span class="sxs-lookup"><span data-stu-id="659f3-188">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="659f3-189">処理が正常に終了すると、Microsoft Graph は `204 No Content` コードを返します。</span><span class="sxs-lookup"><span data-stu-id="659f3-189">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="659f3-190">通知</span><span class="sxs-lookup"><span data-stu-id="659f3-190">Notifications</span></span>

<span data-ttu-id="659f3-191">クライアントはサブスクリプションを作成した後、通知の受信を開始します。</span><span class="sxs-lookup"><span data-stu-id="659f3-191">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="659f3-192">Microsoft Graph は、リソースに変更が発生すると通知 URL に POST 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="659f3-192">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="659f3-193">通知が送信されるのは、`created` など、サブスクリプションで指定されているタイプの変更についてのみです。</span><span class="sxs-lookup"><span data-stu-id="659f3-193">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="659f3-194">**注:** 同じリソース タイプを監視し、同じ通知 URL を使用する複数のサブスクリプションを使用している場合、サブスクリプション ID が異なる複数の通知が含まれる POST が送信されることがあります。</span><span class="sxs-lookup"><span data-stu-id="659f3-194">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="659f3-195">その POST に含まれるすべての通知が、単一のサブスクリプションに属しているという保証はありません。</span><span class="sxs-lookup"><span data-stu-id="659f3-195">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="659f3-196">通知のプロパティ</span><span class="sxs-lookup"><span data-stu-id="659f3-196">Notification properties</span></span>

<span data-ttu-id="659f3-197">通知オブジェクトには、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="659f3-197">The notification object has the following properties:</span></span>

| <span data-ttu-id="659f3-198">プロパティ</span><span class="sxs-lookup"><span data-stu-id="659f3-198">Property</span></span> | <span data-ttu-id="659f3-199">型</span><span class="sxs-lookup"><span data-stu-id="659f3-199">Type</span></span> | <span data-ttu-id="659f3-200">説明</span><span class="sxs-lookup"><span data-stu-id="659f3-200">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="659f3-201">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="659f3-201">subscriptionId</span></span> | <span data-ttu-id="659f3-202">string</span><span class="sxs-lookup"><span data-stu-id="659f3-202">string</span></span> | <span data-ttu-id="659f3-203">通知を生成したサブスクリプションの ID。</span><span class="sxs-lookup"><span data-stu-id="659f3-203">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="659f3-204">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="659f3-204">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="659f3-205">dateTime</span><span class="sxs-lookup"><span data-stu-id="659f3-205">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="659f3-206">サブスクリプションの有効期限が切れるとき。</span><span class="sxs-lookup"><span data-stu-id="659f3-206">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="659f3-207">clientState</span><span class="sxs-lookup"><span data-stu-id="659f3-207">clientState</span></span> | <span data-ttu-id="659f3-208">string</span><span class="sxs-lookup"><span data-stu-id="659f3-208">string</span></span> | <span data-ttu-id="659f3-209">サブスクリプション要求で指定された `clientState` プロパティ (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="659f3-209">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="659f3-210">changeType</span><span class="sxs-lookup"><span data-stu-id="659f3-210">changeType</span></span> | <span data-ttu-id="659f3-211">string</span><span class="sxs-lookup"><span data-stu-id="659f3-211">string</span></span> | <span data-ttu-id="659f3-212">通知の原因となったイベントの種類。</span><span class="sxs-lookup"><span data-stu-id="659f3-212">The event type that caused the notification.</span></span> <span data-ttu-id="659f3-213">たとえば、メール受信時は `created`、または読んだメッセージをマークした場合は `updated`。</span><span class="sxs-lookup"><span data-stu-id="659f3-213">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="659f3-214">resource</span><span class="sxs-lookup"><span data-stu-id="659f3-214">resource</span></span> | <span data-ttu-id="659f3-215">string</span><span class="sxs-lookup"><span data-stu-id="659f3-215">string</span></span> | <span data-ttu-id="659f3-216">`https://graph.microsoft.com` に関連するリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="659f3-216">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="659f3-217">resourceData</span><span class="sxs-lookup"><span data-stu-id="659f3-217">resourceData</span></span> | <span data-ttu-id="659f3-218">object</span><span class="sxs-lookup"><span data-stu-id="659f3-218">object</span></span> | <span data-ttu-id="659f3-219">このプロパティの内容は、サブスクリプションの対象となるリソースの種類に応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="659f3-219">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="659f3-220">たとえば、Outlook リソースの場合、`resourceData` には次のフィールドが含まれています:</span><span class="sxs-lookup"><span data-stu-id="659f3-220">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="659f3-221">プロパティ</span><span class="sxs-lookup"><span data-stu-id="659f3-221">Property</span></span> | <span data-ttu-id="659f3-222">型</span><span class="sxs-lookup"><span data-stu-id="659f3-222">Type</span></span> | <span data-ttu-id="659f3-223">説明</span><span class="sxs-lookup"><span data-stu-id="659f3-223">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="659f3-224">@odata.type</span><span class="sxs-lookup"><span data-stu-id="659f3-224">@odata.type</span></span> | <span data-ttu-id="659f3-225">string</span><span class="sxs-lookup"><span data-stu-id="659f3-225">string</span></span> | <span data-ttu-id="659f3-226">表しているオブジェクトを記述する、Microsoft Graph の OData エンティティ タイプ。</span><span class="sxs-lookup"><span data-stu-id="659f3-226">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="659f3-227">@odata.id</span><span class="sxs-lookup"><span data-stu-id="659f3-227">@odata.id</span></span> | <span data-ttu-id="659f3-228">string</span><span class="sxs-lookup"><span data-stu-id="659f3-228">string</span></span> | <span data-ttu-id="659f3-229">オブジェクトの OData 識別子。</span><span class="sxs-lookup"><span data-stu-id="659f3-229">The OData identifier of the object.</span></span> |
| <span data-ttu-id="659f3-230">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="659f3-230">@odata.etag</span></span> | <span data-ttu-id="659f3-231">string</span><span class="sxs-lookup"><span data-stu-id="659f3-231">string</span></span> | <span data-ttu-id="659f3-232">オブジェクトのバージョンを表す HTTP エンティティ タグ。</span><span class="sxs-lookup"><span data-stu-id="659f3-232">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="659f3-233">ID</span><span class="sxs-lookup"><span data-stu-id="659f3-233">id</span></span> | <span data-ttu-id="659f3-234">string</span><span class="sxs-lookup"><span data-stu-id="659f3-234">string</span></span> | <span data-ttu-id="659f3-235">オブジェクトの識別子。</span><span class="sxs-lookup"><span data-stu-id="659f3-235">The identifier of the object.</span></span> |

> <span data-ttu-id="659f3-236">**注:** `resourceData` で提供される `id` 値は、通知生成時に有効だったものです。</span><span class="sxs-lookup"><span data-stu-id="659f3-236">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="659f3-237">メッセージを別のフォルダーに移動するなど、アクションによっては、通知処理時に `id` が有効でなくなるという結果になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-237">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="659f3-238">通知の例</span><span class="sxs-lookup"><span data-stu-id="659f3-238">Notification example</span></span>

<span data-ttu-id="659f3-239">ユーザーが電子メールを受信すると、Microsoft Graph は次のように通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="659f3-239">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

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

<span data-ttu-id="659f3-240">`value` フィールドはオブジェクトの配列であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="659f3-240">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="659f3-241">キューに多数の通知が入っている場合、Microsoft Graph から、単一の要求の中で複数の項目が送信されることがあります。</span><span class="sxs-lookup"><span data-stu-id="659f3-241">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="659f3-242">同じ通知要求の中に、異なる複数のサブスクリプションからの通知が含まれることがあります。</span><span class="sxs-lookup"><span data-stu-id="659f3-242">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="659f3-243">通知の処理</span><span class="sxs-lookup"><span data-stu-id="659f3-243">Processing the notification</span></span>

<span data-ttu-id="659f3-244">アプリの受け取る通知を、それぞれ処理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-244">Each notification received by your app should be processed.</span></span> <span data-ttu-id="659f3-245">アプリが通知を処理するために必要な最小限のタスクは、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="659f3-245">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="659f3-246">`clientState` プロパティを検証します。</span><span class="sxs-lookup"><span data-stu-id="659f3-246">Validate the `clientState` property.</span></span> <span data-ttu-id="659f3-247">これは、サブスクリプション作成要求で当初送られた値に一致していなければなりません。</span><span class="sxs-lookup"><span data-stu-id="659f3-247">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="659f3-248">**注:** そうでない場合、これを有効な通知と見なすことはできません。</span><span class="sxs-lookup"><span data-stu-id="659f3-248">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="659f3-249">通知が Microsoft Graph に由来するものでなく、悪意のある者が偽って送った可能性があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-249">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="659f3-250">また、通知の送信元を調査し、適切なアクションを実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-250">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="659f3-251">ビジネス ロジックに基づいて、アプリケーションを更新します。</span><span class="sxs-lookup"><span data-stu-id="659f3-251">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="659f3-252">Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。</span><span class="sxs-lookup"><span data-stu-id="659f3-252">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="659f3-253">Microsoft Graph が 2xx クラス コードを受信しない場合は、通知を何回でも再試行します。</span><span class="sxs-lookup"><span data-stu-id="659f3-253">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="659f3-254">**注:** `clientState`プロパティがサブスクリプション要求のものと一致しない場合でも、`202 - Accepted` ステータス コードを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="659f3-254">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="659f3-255">これは、偽通知が信頼されていないかもしれないという事実を悪意のある者が検出し、それを利用して `clientState` プロパティの値を類推するのを防ぐことになるため、優れた方法と言えます。</span><span class="sxs-lookup"><span data-stu-id="659f3-255">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="659f3-256">要求内の他の通知について、これらを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="659f3-256">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="659f3-257">コード サンプル</span><span class="sxs-lookup"><span data-stu-id="659f3-257">Code samples</span></span>

<span data-ttu-id="659f3-258">GitHub では、次のコード サンプルを利用できます。</span><span class="sxs-lookup"><span data-stu-id="659f3-258">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="659f3-259">Microsoft Graph トレーニング モジュール - Microsoft Graph で変更通知と変更履歴を使用する</span><span class="sxs-lookup"><span data-stu-id="659f3-259">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="659f3-260">Node.js 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="659f3-260">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="659f3-261">ASP.NET 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="659f3-261">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="659f3-262">WebJobs SDK を使用した Microsoft Graph ユーザー Webhook のサンプル</span><span class="sxs-lookup"><span data-stu-id="659f3-262">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="659f3-263">関連項目</span><span class="sxs-lookup"><span data-stu-id="659f3-263">See also</span></span>

- [<span data-ttu-id="659f3-264">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="659f3-264">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="659f3-265">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="659f3-265">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="659f3-266">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="659f3-266">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="659f3-267">変更通知チュートリアル</span><span class="sxs-lookup"><span data-stu-id="659f3-267">Change notifications tutorial</span></span>](/graph/tutorials/change-notifications)

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
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
