# <a name="subscription-resource-type"></a><span data-ttu-id="8a1b3-101">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8a1b3-101">subscription resource type</span></span>

<span data-ttu-id="8a1b3-102">サブスクリプションは、Microsoft Graph でデータへの変更に関する通知を受信するクライアント アプリケーションを許可します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-102">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="8a1b3-103">現時点では、サブスクリプションが有効になって次のリソース。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-103">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="8a1b3-104">メール、イベント、および Outlook の連絡先です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-104">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="8a1b3-105">Office グループからの会話。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-105">Conversations from Office Groups.</span></span>
- <span data-ttu-id="8a1b3-106">OneDrive からドライブのルート項目。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-106">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="8a1b3-107">ユーザーと Azure Active Directory のグループ。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-107">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="8a1b3-108">Graph セキュリティ API から通知されます。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-108">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a1b3-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a1b3-109">JSON representation</span></span>

<span data-ttu-id="8a1b3-110">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8a1b3-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a1b3-111">Properties</span></span>

| <span data-ttu-id="8a1b3-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a1b3-112">Property</span></span> | <span data-ttu-id="8a1b3-113">型</span><span class="sxs-lookup"><span data-stu-id="8a1b3-113">Type</span></span> | <span data-ttu-id="8a1b3-114">説明</span><span class="sxs-lookup"><span data-stu-id="8a1b3-114">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8a1b3-115">changeType</span><span class="sxs-lookup"><span data-stu-id="8a1b3-115">changeType</span></span> | <span data-ttu-id="8a1b3-116">string</span><span class="sxs-lookup"><span data-stu-id="8a1b3-116">string</span></span> | <span data-ttu-id="8a1b3-117">必須。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-117">Required.</span></span> <span data-ttu-id="8a1b3-118">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-118">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="8a1b3-119">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-119">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="8a1b3-120">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-120">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="8a1b3-121">メモ: ドライブのルート アイテムの通知だけをサポートして、 `updated` changeType です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-121">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="8a1b3-122">ユーザーとグループの通知をサポートして`updated`と`deleted`changeType です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-122">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="8a1b3-123">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="8a1b3-123">notificationUrl</span></span> | <span data-ttu-id="8a1b3-124">文字列</span><span class="sxs-lookup"><span data-stu-id="8a1b3-124">string</span></span> | <span data-ttu-id="8a1b3-125">必須。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-125">Required.</span></span> <span data-ttu-id="8a1b3-126">通知を受信するエンドポイントの URL。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-126">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="8a1b3-127">この URL が、HTTPS を使用する必要がありますプロトコルです。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-127">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="8a1b3-128">resource</span><span class="sxs-lookup"><span data-stu-id="8a1b3-128">resource</span></span> | <span data-ttu-id="8a1b3-129">文字列</span><span class="sxs-lookup"><span data-stu-id="8a1b3-129">string</span></span> | <span data-ttu-id="8a1b3-130">必須。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-130">Required.</span></span> <span data-ttu-id="8a1b3-131">変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-131">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="8a1b3-132">ベース URL が含まれていない (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-132">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="8a1b3-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8a1b3-133">expirationDateTime</span></span> | [<span data-ttu-id="8a1b3-134">dateTime</span><span class="sxs-lookup"><span data-stu-id="8a1b3-134">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="8a1b3-135">必須。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-135">Required.</span></span> <span data-ttu-id="8a1b3-136">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-136">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="8a1b3-137">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-137">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="8a1b3-138">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-138">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="8a1b3-139">clientState</span><span class="sxs-lookup"><span data-stu-id="8a1b3-139">clientState</span></span> | <span data-ttu-id="8a1b3-140">string</span><span class="sxs-lookup"><span data-stu-id="8a1b3-140">string</span></span> | <span data-ttu-id="8a1b3-141">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-141">Optional.</span></span> <span data-ttu-id="8a1b3-142">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-142">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="8a1b3-143">最大の長さは 128 文字です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-143">The maximum length is 128 characters.</span></span> <span data-ttu-id="8a1b3-144">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-144">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="8a1b3-145">ID</span><span class="sxs-lookup"><span data-stu-id="8a1b3-145">id</span></span> | <span data-ttu-id="8a1b3-146">文字列</span><span class="sxs-lookup"><span data-stu-id="8a1b3-146">string</span></span> | <span data-ttu-id="8a1b3-p108">サブスクリプションの一意の識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-p108">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="8a1b3-149">applicationId</span><span class="sxs-lookup"><span data-stu-id="8a1b3-149">applicationId</span></span> | <span data-ttu-id="8a1b3-150">文字列</span><span class="sxs-lookup"><span data-stu-id="8a1b3-150">string</span></span> | <span data-ttu-id="8a1b3-151">サブスクリプションを作成するために使用するアプリケーションの識別子です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-151">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="8a1b3-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-152">Read-only.</span></span> |
| <span data-ttu-id="8a1b3-153">creatorId</span><span class="sxs-lookup"><span data-stu-id="8a1b3-153">creatorId</span></span> | <span data-ttu-id="8a1b3-154">文字列</span><span class="sxs-lookup"><span data-stu-id="8a1b3-154">string</span></span> | <span data-ttu-id="8a1b3-155">ユーザーまたはサブスクリプションを作成するサービス ・ プリンシパルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-155">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="8a1b3-156">使用するアプリケーションがサブスクリプションを作成するアクセス許可を委任する場合、このフィールドは、サインイン中のユーザーの代理で、アプリケーションが呼び出されるの id を含みます。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-156">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="8a1b3-157">アプリケーションは、アプリケーションのアクセス許可を使用する場合、このフィールドには、アプリケーションに対応するサービス ・ プリンシパルの id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-157">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="8a1b3-158">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-158">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="8a1b3-159">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="8a1b3-159">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="8a1b3-160">リソース</span><span class="sxs-lookup"><span data-stu-id="8a1b3-160">Resource</span></span>            | <span data-ttu-id="8a1b3-161">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="8a1b3-161">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="8a1b3-162">メール</span><span class="sxs-lookup"><span data-stu-id="8a1b3-162">Mail</span></span>                | <span data-ttu-id="8a1b3-163">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="8a1b3-163">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8a1b3-164">予定表</span><span class="sxs-lookup"><span data-stu-id="8a1b3-164">Calendar</span></span>            | <span data-ttu-id="8a1b3-165">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="8a1b3-165">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8a1b3-166">連絡先</span><span class="sxs-lookup"><span data-stu-id="8a1b3-166">Contacts</span></span>            | <span data-ttu-id="8a1b3-167">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="8a1b3-167">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8a1b3-168">グループ会話</span><span class="sxs-lookup"><span data-stu-id="8a1b3-168">Group conversations</span></span> | <span data-ttu-id="8a1b3-169">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="8a1b3-169">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8a1b3-170">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="8a1b3-170">Drive root items</span></span>    | <span data-ttu-id="8a1b3-171">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="8a1b3-171">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="8a1b3-172">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="8a1b3-172">Security alerts</span></span>     | <span data-ttu-id="8a1b3-173">43200 分 (30 日間で)</span><span class="sxs-lookup"><span data-stu-id="8a1b3-173">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="8a1b3-174">**注:** 既存のアプリケーションと新しいアプリケーションは、サポートされている値を超える必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-174">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="8a1b3-175">将来、作成するか、最大値を超えるサブスクリプションを更新するすべての要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-175">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="8a1b3-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a1b3-176">Relationships</span></span>

<span data-ttu-id="8a1b3-177">なし</span><span class="sxs-lookup"><span data-stu-id="8a1b3-177">None</span></span>

## <a name="methods"></a><span data-ttu-id="8a1b3-178">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a1b3-178">Methods</span></span>

| <span data-ttu-id="8a1b3-179">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a1b3-179">Method</span></span> | <span data-ttu-id="8a1b3-180">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8a1b3-180">Return Type</span></span> | <span data-ttu-id="8a1b3-181">説明</span><span class="sxs-lookup"><span data-stu-id="8a1b3-181">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="8a1b3-182">Create subscription</span><span class="sxs-lookup"><span data-stu-id="8a1b3-182">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="8a1b3-183">subscription</span><span class="sxs-lookup"><span data-stu-id="8a1b3-183">subscription</span></span>](subscription.md) | <span data-ttu-id="8a1b3-184">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-184">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="8a1b3-185">Update subscription</span><span class="sxs-lookup"><span data-stu-id="8a1b3-185">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="8a1b3-186">subscription</span><span class="sxs-lookup"><span data-stu-id="8a1b3-186">subscription</span></span>](subscription.md) | <span data-ttu-id="8a1b3-187">有効期限を更新することにより、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-187">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="8a1b3-188">リストの購読</span><span class="sxs-lookup"><span data-stu-id="8a1b3-188">List subscriptions</span></span>](../api/subscription_list.md) | [<span data-ttu-id="8a1b3-189">subscription</span><span class="sxs-lookup"><span data-stu-id="8a1b3-189">subscription</span></span>](subscription.md) | <span data-ttu-id="8a1b3-190">アクティブなサブスクリプションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-190">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="8a1b3-191">Get subscription</span><span class="sxs-lookup"><span data-stu-id="8a1b3-191">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="8a1b3-192">subscription</span><span class="sxs-lookup"><span data-stu-id="8a1b3-192">subscription</span></span>](subscription.md) | <span data-ttu-id="8a1b3-193">サブスクリプション オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-193">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="8a1b3-194">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="8a1b3-194">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="8a1b3-195">なし</span><span class="sxs-lookup"><span data-stu-id="8a1b3-195">None</span></span> |<span data-ttu-id="8a1b3-196">サブスクリプション オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="8a1b3-196">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
