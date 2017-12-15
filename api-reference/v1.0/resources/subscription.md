# <a name="subscription-resource-type"></a><span data-ttu-id="f5b96-101">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="f5b96-101">Subscription Resource Type</span></span>
<span data-ttu-id="f5b96-102">サブスクリプションは、Microsoft Graph 上のデータに関する通知の受信をクライアントのアプリケーションに許可します。</span><span class="sxs-lookup"><span data-stu-id="f5b96-102">A subscription allows a client app to receive notifications about data on the Microsoft Graph. Currently subscriptions are enabled for the following datasets:</span></span> <span data-ttu-id="f5b96-103">サブスクリプションは現在、以下のデータセットで有効です:</span><span class="sxs-lookup"><span data-stu-id="f5b96-103">Currently, subscriptions are enabled for the following datasets:</span></span>

1. <span data-ttu-id="f5b96-104">Outlook からのメール、イベント、および連絡先</span><span class="sxs-lookup"><span data-stu-id="f5b96-104">Mail, events, and contacts from Outlook</span></span>
1. <span data-ttu-id="f5b96-105">Office グループからの会話。</span><span class="sxs-lookup"><span data-stu-id="f5b96-105">Conversations from Office Groups.</span></span>
1. <span data-ttu-id="f5b96-106">OneDrive からドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="f5b96-106">Drive root items from OneDrive</span></span> 


## <a name="json-representation"></a><span data-ttu-id="f5b96-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5b96-107">JSON representation</span></span>

<span data-ttu-id="f5b96-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5b96-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a><span data-ttu-id="f5b96-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5b96-109">Properties</span></span>
| <span data-ttu-id="f5b96-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5b96-110">Property</span></span>     | <span data-ttu-id="f5b96-111">型</span><span class="sxs-lookup"><span data-stu-id="f5b96-111">Type</span></span>   |<span data-ttu-id="f5b96-112">説明</span><span class="sxs-lookup"><span data-stu-id="f5b96-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5b96-113">changeType</span><span class="sxs-lookup"><span data-stu-id="f5b96-113">changeType</span></span>|<span data-ttu-id="f5b96-114">string</span><span class="sxs-lookup"><span data-stu-id="f5b96-114">string</span></span>|<span data-ttu-id="f5b96-115">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="f5b96-115">Indicates the type of change in the subscribed resource that will raise a notification. The supported values are: , , . Multiple values can be combined using a comma-separated list.</span></span> <span data-ttu-id="f5b96-116">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="f5b96-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="f5b96-117">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="f5b96-117">Multiple values can be combined using a comma-separated list.</span></span>|
|<span data-ttu-id="f5b96-118">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="f5b96-118">notificationUrl</span></span>|<span data-ttu-id="f5b96-119">string</span><span class="sxs-lookup"><span data-stu-id="f5b96-119">string</span></span>|<span data-ttu-id="f5b96-p103">通知を受け取るエンドポイントの URL です。この URL は HTTPS プロトコルを利用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f5b96-p103">The URL of the endpoint that will receive the notifications. This URL has to make use of the HTTPS protocol.</span></span>|
|<span data-ttu-id="f5b96-122">リソース</span><span class="sxs-lookup"><span data-stu-id="f5b96-122">resource</span></span>|<span data-ttu-id="f5b96-123">string</span><span class="sxs-lookup"><span data-stu-id="f5b96-123">string</span></span>|<span data-ttu-id="f5b96-p104">変更の監視対象となるリソースを指定します。ベース URL ("https://graph.microsoft.com/v1.0/") は含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f5b96-p104">Specifies the resource that will be monitored for changes. Do not include the base URL ("https://graph.microsoft.com/v1.0/").</span></span>|
|<span data-ttu-id="f5b96-126">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f5b96-126">expirationDateTime</span></span>|[<span data-ttu-id="f5b96-127">dateTime</span><span class="sxs-lookup"><span data-stu-id="f5b96-127">dateTime</span></span>](http://tools.ietf.org/html/rfc3339)|<span data-ttu-id="f5b96-128">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5b96-128">Specifies the date and time when the notification subscription expires. The time is in UTC.</span></span> <span data-ttu-id="f5b96-129">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="f5b96-129">Specifies the date and time when the webhook subscription expires. The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.  See the table below for maximum values.</span></span>  <span data-ttu-id="f5b96-130">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f5b96-130">See the table below for maximum supported subscription length of time.</span></span> |
|<span data-ttu-id="f5b96-131">clientState</span><span class="sxs-lookup"><span data-stu-id="f5b96-131">clientState</span></span>|<span data-ttu-id="f5b96-132">string</span><span class="sxs-lookup"><span data-stu-id="f5b96-132">string</span></span>|<span data-ttu-id="f5b96-133">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5b96-133">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="f5b96-134">最大の長さは 128 文字です。</span><span class="sxs-lookup"><span data-stu-id="f5b96-134">The maximum length is 255 characters.</span></span> <span data-ttu-id="f5b96-135">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="f5b96-135">Specifies the value of the  property sent by the service in each notification. The maximum length is 128 characters. The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span>|
|<span data-ttu-id="f5b96-136">id</span><span class="sxs-lookup"><span data-stu-id="f5b96-136">id</span></span>|<span data-ttu-id="f5b96-137">string</span><span class="sxs-lookup"><span data-stu-id="f5b96-137">string</span></span>|<span data-ttu-id="f5b96-p107">サブスクリプションの一意の識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f5b96-p107">Unique identifier for the subscription. Read-only.</span></span>|

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="f5b96-140">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="f5b96-140">Maximum length of subscription per resource type</span></span>
| <span data-ttu-id="f5b96-141">リソース</span><span class="sxs-lookup"><span data-stu-id="f5b96-141">Resource</span></span> | <span data-ttu-id="f5b96-142">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="f5b96-142">Maximum Expiration Time</span></span> |
|:---------------------|:--------------------|
|<span data-ttu-id="f5b96-143">メール</span><span class="sxs-lookup"><span data-stu-id="f5b96-143">Mail</span></span>| <span data-ttu-id="f5b96-144">4230 分。</span><span class="sxs-lookup"><span data-stu-id="f5b96-144">4230 minutes.</span></span>|
|<span data-ttu-id="f5b96-145">予定表</span><span class="sxs-lookup"><span data-stu-id="f5b96-145">Calendar</span></span>| <span data-ttu-id="f5b96-146">4230 分。</span><span class="sxs-lookup"><span data-stu-id="f5b96-146">4230 minutes.</span></span>|
|<span data-ttu-id="f5b96-147">連絡先</span><span class="sxs-lookup"><span data-stu-id="f5b96-147">Contacts</span></span>| <span data-ttu-id="f5b96-148">4230 分。</span><span class="sxs-lookup"><span data-stu-id="f5b96-148">4230 minutes.</span></span>|
|<span data-ttu-id="f5b96-149">グループ会話</span><span class="sxs-lookup"><span data-stu-id="f5b96-149">Group conversations</span></span>| <span data-ttu-id="f5b96-150">4230 分。</span><span class="sxs-lookup"><span data-stu-id="f5b96-150">4230 minutes.</span></span>|
|<span data-ttu-id="f5b96-151">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="f5b96-151">Drive root items</span></span>| <span data-ttu-id="f5b96-152">43200 分。</span><span class="sxs-lookup"><span data-stu-id="f5b96-152">43200 minutes.</span></span> <span data-ttu-id="f5b96-153">既存のアプリケーションと新規アプリケーションのどちらもサポートされている値を超えてはなりません。</span><span class="sxs-lookup"><span data-stu-id="f5b96-153">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="f5b96-154">今後のリリースでは、これより高い値は設定できません。</span><span class="sxs-lookup"><span data-stu-id="f5b96-154">Higher values won't be permitted in upcoming releases.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f5b96-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f5b96-155">Relationships</span></span>
<span data-ttu-id="f5b96-156">なし</span><span class="sxs-lookup"><span data-stu-id="f5b96-156">None</span></span>


## <a name="methods"></a><span data-ttu-id="f5b96-157">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5b96-157">Methods</span></span>

| <span data-ttu-id="f5b96-158">メソッド</span><span class="sxs-lookup"><span data-stu-id="f5b96-158">Method</span></span>           | <span data-ttu-id="f5b96-159">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f5b96-159">Return Type</span></span>    |<span data-ttu-id="f5b96-160">説明</span><span class="sxs-lookup"><span data-stu-id="f5b96-160">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5b96-161">Create subscription</span><span class="sxs-lookup"><span data-stu-id="f5b96-161">Create subscription</span></span>](../api/subscription_post_subscriptions.md) | [<span data-ttu-id="f5b96-162">subscription</span><span class="sxs-lookup"><span data-stu-id="f5b96-162">subscription</span></span>](subscription.md) |<span data-ttu-id="f5b96-163">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="f5b96-163">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span>|
|[<span data-ttu-id="f5b96-164">Update subscription</span><span class="sxs-lookup"><span data-stu-id="f5b96-164">Update subscription</span></span>](../api/subscription_update.md) | [<span data-ttu-id="f5b96-165">subscription</span><span class="sxs-lookup"><span data-stu-id="f5b96-165">subscription</span></span>](subscription.md) |<span data-ttu-id="f5b96-166">有効期限を更新することにより、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="f5b96-166">Renews a subscription by updating its expiration time.</span></span>|
|[<span data-ttu-id="f5b96-167">Get subscription</span><span class="sxs-lookup"><span data-stu-id="f5b96-167">Get subscription</span></span>](../api/subscription_get.md) | [<span data-ttu-id="f5b96-168">subscription</span><span class="sxs-lookup"><span data-stu-id="f5b96-168">subscription</span></span>](subscription.md) |<span data-ttu-id="f5b96-169">サブスクリプション オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f5b96-169">Reads properties and relationships of subscription object.</span></span>|
|[<span data-ttu-id="f5b96-170">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="f5b96-170">Delete subscription</span></span>](../api/subscription_delete.md) | <span data-ttu-id="f5b96-171">なし</span><span class="sxs-lookup"><span data-stu-id="f5b96-171">None</span></span> |<span data-ttu-id="f5b96-172">サブスクリプション オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="f5b96-172">Deletes a subscription object.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
