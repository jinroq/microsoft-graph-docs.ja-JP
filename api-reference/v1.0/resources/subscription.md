# <a name="subscription-resource-type"></a><span data-ttu-id="95edf-101">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95edf-101">Subscription resource type</span></span>

<span data-ttu-id="95edf-102">サブスクリプションは、Microsoft Graph 上のデータに対する変更についての通知の受信をクライアント アプリケーションに許可します。</span><span class="sxs-lookup"><span data-stu-id="95edf-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph.</span></span> <span data-ttu-id="95edf-103">現時点では、サブスクリプションは次のリソースで有効です。</span><span class="sxs-lookup"><span data-stu-id="95edf-103">Currently, subscriptions are enabled for the following datasets:</span></span>

- <span data-ttu-id="95edf-104">Outlook からのメール、イベント、および連絡先</span><span class="sxs-lookup"><span data-stu-id="95edf-104">Mail, events, and contacts from Outlook</span></span>
- <span data-ttu-id="95edf-105">Office グループからの会話。</span><span class="sxs-lookup"><span data-stu-id="95edf-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="95edf-106">OneDrive からドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="95edf-106">Drive root items from OneDrive</span></span>
- <span data-ttu-id="95edf-107">Azure Active Directory からのユーザーおよびグループ</span><span class="sxs-lookup"><span data-stu-id="95edf-107">Users and Groups from Azure Active Directory</span></span>

## <a name="json-representation"></a><span data-ttu-id="95edf-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95edf-108">JSON representation</span></span>

<span data-ttu-id="95edf-109">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95edf-109">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="95edf-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95edf-110">Properties</span></span>

| <span data-ttu-id="95edf-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95edf-111">Property</span></span> | <span data-ttu-id="95edf-112">タイプ</span><span class="sxs-lookup"><span data-stu-id="95edf-112">Type</span></span> | <span data-ttu-id="95edf-113">説明</span><span class="sxs-lookup"><span data-stu-id="95edf-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="95edf-114">changeType</span><span class="sxs-lookup"><span data-stu-id="95edf-114">changeType</span></span> | <span data-ttu-id="95edf-115">文字列</span><span class="sxs-lookup"><span data-stu-id="95edf-115">string</span></span> | <span data-ttu-id="95edf-116">必須。</span><span class="sxs-lookup"><span data-stu-id="95edf-116">Required.</span></span> <span data-ttu-id="95edf-117">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="95edf-117">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="95edf-118">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="95edf-118">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="95edf-119">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="95edf-119">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="95edf-120">メモ: ドライブ ルート項目の通知は `updated` changeType のみに対応しています。</span><span class="sxs-lookup"><span data-stu-id="95edf-120">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="95edf-121">ユーザーとグループの通知は`updated` と `deleted` changeType に対応しています。</span><span class="sxs-lookup"><span data-stu-id="95edf-121">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="95edf-122">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="95edf-122">notificationUrl</span></span> | <span data-ttu-id="95edf-123">文字列</span><span class="sxs-lookup"><span data-stu-id="95edf-123">string</span></span> | <span data-ttu-id="95edf-124">必須。</span><span class="sxs-lookup"><span data-stu-id="95edf-124">Required.</span></span> <span data-ttu-id="95edf-125">通知を受信するエンドポイントの URL。</span><span class="sxs-lookup"><span data-stu-id="95edf-125">The URL of the application that will receive the push notifications.</span></span> <span data-ttu-id="95edf-126">この URL は必ず HTTPS プロトコルを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="95edf-126">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="95edf-127">リソース</span><span class="sxs-lookup"><span data-stu-id="95edf-127">resource</span></span> | <span data-ttu-id="95edf-128">文字列</span><span class="sxs-lookup"><span data-stu-id="95edf-128">string</span></span> | <span data-ttu-id="95edf-129">必須。</span><span class="sxs-lookup"><span data-stu-id="95edf-129">Required.</span></span> <span data-ttu-id="95edf-130">変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="95edf-130">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="95edf-131">ベース URL (`https://graph.microsoft.com/v1.0/`) は含めないでください。</span><span class="sxs-lookup"><span data-stu-id="95edf-131">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="95edf-132">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="95edf-132">expirationDateTime</span></span> | [<span data-ttu-id="95edf-133">dateTime</span><span class="sxs-lookup"><span data-stu-id="95edf-133">dateTime</span></span>](http://tools.ietf.org/html/rfc3339) | <span data-ttu-id="95edf-134">必須。</span><span class="sxs-lookup"><span data-stu-id="95edf-134">Required.</span></span> <span data-ttu-id="95edf-135">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="95edf-135">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="95edf-136">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="95edf-136">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="95edf-137">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="95edf-137">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="95edf-138">clientState</span><span class="sxs-lookup"><span data-stu-id="95edf-138">clientState</span></span> | <span data-ttu-id="95edf-139">文字列</span><span class="sxs-lookup"><span data-stu-id="95edf-139">string</span></span> | <span data-ttu-id="95edf-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="95edf-140">Optional.</span></span> <span data-ttu-id="95edf-141">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="95edf-141">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="95edf-142">最大の長さは 128 文字です。</span><span class="sxs-lookup"><span data-stu-id="95edf-142">The maximum length is 128 characters.</span></span> <span data-ttu-id="95edf-143">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="95edf-143">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="95edf-144">ID</span><span class="sxs-lookup"><span data-stu-id="95edf-144">id</span></span> | <span data-ttu-id="95edf-145">文字列</span><span class="sxs-lookup"><span data-stu-id="95edf-145">string</span></span> | <span data-ttu-id="95edf-p108">サブスクリプションの一意の識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95edf-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="95edf-148">applicationId</span><span class="sxs-lookup"><span data-stu-id="95edf-148">applicationId</span></span> | <span data-ttu-id="95edf-149">文字列</span><span class="sxs-lookup"><span data-stu-id="95edf-149">string</span></span> | <span data-ttu-id="95edf-150">サブスクリプションを作成するために使用するアプリケーションの識別子です。</span><span class="sxs-lookup"><span data-stu-id="95edf-150">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="95edf-151">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="95edf-151">Read-only.</span></span> |
| <span data-ttu-id="95edf-152">creatorId</span><span class="sxs-lookup"><span data-stu-id="95edf-152">creatorId</span></span> | <span data-ttu-id="95edf-153">文字列</span><span class="sxs-lookup"><span data-stu-id="95edf-153">string</span></span> | <span data-ttu-id="95edf-154">サブスクリプションを作成したユーザーまたはサービス プリンシパルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="95edf-154">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="95edf-155">アプリケーションがサブスクリプションを作成するのに委任されたアクセス許可を使用した場合、このフィールドには、代理でアプリケーションが呼び出したサインイン中のユーザーの ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="95edf-155">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="95edf-156">アプリケーションは、アプリケーションのアクセス許可を使用した場合、このフィールドには、そのアプリケーションに対応するサービス プリンシパルの ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="95edf-156">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="95edf-157">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="95edf-157">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="95edf-158">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="95edf-158">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="95edf-159">リソース</span><span class="sxs-lookup"><span data-stu-id="95edf-159">Resource</span></span>            | <span data-ttu-id="95edf-160">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="95edf-160">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="95edf-161">メール</span><span class="sxs-lookup"><span data-stu-id="95edf-161">Mail</span></span>                | <span data-ttu-id="95edf-162">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="95edf-162">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="95edf-163">カレンダー</span><span class="sxs-lookup"><span data-stu-id="95edf-163">Calendar</span></span>            | <span data-ttu-id="95edf-164">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="95edf-164">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="95edf-165">連絡先</span><span class="sxs-lookup"><span data-stu-id="95edf-165">Contacts</span></span>            | <span data-ttu-id="95edf-166">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="95edf-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="95edf-167">グループ会話</span><span class="sxs-lookup"><span data-stu-id="95edf-167">Group conversations</span></span> | <span data-ttu-id="95edf-168">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="95edf-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="95edf-169">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="95edf-169">Drive root items</span></span>    | <span data-ttu-id="95edf-170">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="95edf-170">4230 minutes (under 3 days)</span></span>    |

> <span data-ttu-id="95edf-171">**注意:** 既存のアプリケーションと新規アプリケーションのどちらもサポートされている値を超えてはなりません。</span><span class="sxs-lookup"><span data-stu-id="95edf-171">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="95edf-172">後になされる最大値を超えるサブスクリプションの作成や更新の要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="95edf-172">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="95edf-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95edf-173">Relationships</span></span>

<span data-ttu-id="95edf-174">なし</span><span class="sxs-lookup"><span data-stu-id="95edf-174">None</span></span>

## <a name="methods"></a><span data-ttu-id="95edf-175">メソッド</span><span class="sxs-lookup"><span data-stu-id="95edf-175">Methods</span></span>

| <span data-ttu-id="95edf-176">メソッド</span><span class="sxs-lookup"><span data-stu-id="95edf-176">Method</span></span> | <span data-ttu-id="95edf-177">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="95edf-177">Return Type</span></span> | <span data-ttu-id="95edf-178">説明</span><span class="sxs-lookup"><span data-stu-id="95edf-178">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="95edf-179">サブスクリプションを作成</span><span class="sxs-lookup"><span data-stu-id="95edf-179">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="95edf-180">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="95edf-180">subscription</span></span>](subscription.md) | <span data-ttu-id="95edf-181">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="95edf-181">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="95edf-182">サブスクリプションを更新</span><span class="sxs-lookup"><span data-stu-id="95edf-182">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="95edf-183">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="95edf-183">subscription</span></span>](subscription.md) | <span data-ttu-id="95edf-184">有効期限を更新することにより、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="95edf-184">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="95edf-185">サブスクリプションをリスト</span><span class="sxs-lookup"><span data-stu-id="95edf-185">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="95edf-186">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="95edf-186">subscription</span></span>](subscription.md) | <span data-ttu-id="95edf-187">アクティブなサブスクリプションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="95edf-187">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="95edf-188">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="95edf-188">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="95edf-189">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="95edf-189">subscription</span></span>](subscription.md) | <span data-ttu-id="95edf-190">サブスクリプション オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="95edf-190">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="95edf-191">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="95edf-191">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="95edf-192">なし</span><span class="sxs-lookup"><span data-stu-id="95edf-192">None</span></span> |<span data-ttu-id="95edf-193">サブスクリプション オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="95edf-193">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
