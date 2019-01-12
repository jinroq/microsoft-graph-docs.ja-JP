---
title: サブスクリプション リソースの種類
description: サブスクリプションは、Microsoft Graph でデータへの変更に関する通知を受信するクライアント アプリケーションを許可します。 現時点では、サブスクリプションが有効になって次のリソース。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 0f6baa3ca36b91c8a4dd38086a7fc0eebdcf46e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982464"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="1095c-104">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1095c-104">subscription resource type</span></span>

> <span data-ttu-id="1095c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1095c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1095c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1095c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1095c-107">サブスクリプションは、Microsoft Graph でデータへの変更に関する通知を受信するクライアント アプリケーションを許可します。</span><span class="sxs-lookup"><span data-stu-id="1095c-107">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="1095c-108">現時点では、サブスクリプションが有効になって次のリソース。</span><span class="sxs-lookup"><span data-stu-id="1095c-108">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="1095c-109">メール、イベント、および Outlook の連絡先です。</span><span class="sxs-lookup"><span data-stu-id="1095c-109">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="1095c-110">Office グループからの会話。</span><span class="sxs-lookup"><span data-stu-id="1095c-110">Conversations from Office Groups.</span></span>
- <span data-ttu-id="1095c-111">OneDrive からドライブのルート項目。</span><span class="sxs-lookup"><span data-stu-id="1095c-111">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="1095c-112">ユーザーと Azure Active Directory のグループ。</span><span class="sxs-lookup"><span data-stu-id="1095c-112">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="1095c-113">Graph セキュリティ API から通知されます。</span><span class="sxs-lookup"><span data-stu-id="1095c-113">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1095c-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1095c-114">JSON representation</span></span>

<span data-ttu-id="1095c-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1095c-115">Here is a JSON representation of the resource.</span></span>

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
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="1095c-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1095c-116">Properties</span></span>

| <span data-ttu-id="1095c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1095c-117">Property</span></span> | <span data-ttu-id="1095c-118">種類</span><span class="sxs-lookup"><span data-stu-id="1095c-118">Type</span></span> | <span data-ttu-id="1095c-119">説明</span><span class="sxs-lookup"><span data-stu-id="1095c-119">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="1095c-120">changeType</span><span class="sxs-lookup"><span data-stu-id="1095c-120">changeType</span></span> | <span data-ttu-id="1095c-121">string</span><span class="sxs-lookup"><span data-stu-id="1095c-121">string</span></span> | <span data-ttu-id="1095c-122">必須。</span><span class="sxs-lookup"><span data-stu-id="1095c-122">Required.</span></span> <span data-ttu-id="1095c-123">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="1095c-123">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="1095c-124">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="1095c-124">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="1095c-125">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="1095c-125">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="1095c-126">メモ: ドライブのルート アイテムの通知だけをサポートして、 `updated` changeType です。</span><span class="sxs-lookup"><span data-stu-id="1095c-126">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="1095c-127">ユーザーとグループの通知をサポートして`updated`と`deleted`changeType です。</span><span class="sxs-lookup"><span data-stu-id="1095c-127">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="1095c-128">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="1095c-128">notificationUrl</span></span> | <span data-ttu-id="1095c-129">文字列</span><span class="sxs-lookup"><span data-stu-id="1095c-129">string</span></span> | <span data-ttu-id="1095c-130">必須。</span><span class="sxs-lookup"><span data-stu-id="1095c-130">Required.</span></span> <span data-ttu-id="1095c-131">通知を受信するエンドポイントの URL。</span><span class="sxs-lookup"><span data-stu-id="1095c-131">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="1095c-132">この URL が、HTTPS を使用する必要がありますプロトコルです。</span><span class="sxs-lookup"><span data-stu-id="1095c-132">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="1095c-133">resource</span><span class="sxs-lookup"><span data-stu-id="1095c-133">resource</span></span> | <span data-ttu-id="1095c-134">文字列</span><span class="sxs-lookup"><span data-stu-id="1095c-134">string</span></span> | <span data-ttu-id="1095c-135">必須。</span><span class="sxs-lookup"><span data-stu-id="1095c-135">Required.</span></span> <span data-ttu-id="1095c-136">変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="1095c-136">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="1095c-137">ベース URL が含まれていない (`https://graph.microsoft.com/beta/`)。</span><span class="sxs-lookup"><span data-stu-id="1095c-137">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="1095c-138">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1095c-138">expirationDateTime</span></span> | <span data-ttu-id="1095c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1095c-139">DateTimeOffset</span></span> | <span data-ttu-id="1095c-140">必須。</span><span class="sxs-lookup"><span data-stu-id="1095c-140">Required.</span></span> <span data-ttu-id="1095c-141">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="1095c-141">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="1095c-142">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="1095c-142">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="1095c-143">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1095c-143">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="1095c-144">clientState</span><span class="sxs-lookup"><span data-stu-id="1095c-144">clientState</span></span> | <span data-ttu-id="1095c-145">string</span><span class="sxs-lookup"><span data-stu-id="1095c-145">string</span></span> | <span data-ttu-id="1095c-146">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1095c-146">Optional.</span></span> <span data-ttu-id="1095c-147">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="1095c-147">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="1095c-148">最大の長さは、255 文字です。</span><span class="sxs-lookup"><span data-stu-id="1095c-148">The maximum length is 255 characters.</span></span> <span data-ttu-id="1095c-149">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="1095c-149">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="1095c-150">ID</span><span class="sxs-lookup"><span data-stu-id="1095c-150">id</span></span> | <span data-ttu-id="1095c-151">文字列</span><span class="sxs-lookup"><span data-stu-id="1095c-151">string</span></span> | <span data-ttu-id="1095c-p110">サブスクリプションの一意の識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1095c-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="1095c-154">applicationId</span><span class="sxs-lookup"><span data-stu-id="1095c-154">applicationId</span></span> | <span data-ttu-id="1095c-155">文字列</span><span class="sxs-lookup"><span data-stu-id="1095c-155">string</span></span> | <span data-ttu-id="1095c-156">サブスクリプションを作成するために使用するアプリケーションの識別子です。</span><span class="sxs-lookup"><span data-stu-id="1095c-156">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="1095c-157">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1095c-157">Read-only.</span></span> |
| <span data-ttu-id="1095c-158">creatorId</span><span class="sxs-lookup"><span data-stu-id="1095c-158">creatorId</span></span> | <span data-ttu-id="1095c-159">文字列</span><span class="sxs-lookup"><span data-stu-id="1095c-159">string</span></span> | <span data-ttu-id="1095c-160">ユーザーまたはサブスクリプションを作成するサービス ・ プリンシパルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="1095c-160">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="1095c-161">使用するアプリケーションがサブスクリプションを作成するアクセス許可を委任する場合、このフィールドは、サインイン中のユーザーの代理で、アプリケーションが呼び出されるの id を含みます。</span><span class="sxs-lookup"><span data-stu-id="1095c-161">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="1095c-162">アプリケーションは、アプリケーションのアクセス許可を使用する場合、このフィールドには、アプリケーションに対応するサービス ・ プリンシパルの id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1095c-162">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="1095c-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1095c-163">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="1095c-164">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="1095c-164">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="1095c-165">リソース</span><span class="sxs-lookup"><span data-stu-id="1095c-165">Resource</span></span>            | <span data-ttu-id="1095c-166">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="1095c-166">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="1095c-167">メール</span><span class="sxs-lookup"><span data-stu-id="1095c-167">Mail</span></span>                | <span data-ttu-id="1095c-168">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="1095c-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1095c-169">予定表</span><span class="sxs-lookup"><span data-stu-id="1095c-169">Calendar</span></span>            | <span data-ttu-id="1095c-170">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="1095c-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1095c-171">連絡先</span><span class="sxs-lookup"><span data-stu-id="1095c-171">Contacts</span></span>            | <span data-ttu-id="1095c-172">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="1095c-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1095c-173">グループ会話</span><span class="sxs-lookup"><span data-stu-id="1095c-173">Group conversations</span></span> | <span data-ttu-id="1095c-174">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="1095c-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1095c-175">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="1095c-175">Drive root items</span></span>    | <span data-ttu-id="1095c-176">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="1095c-176">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="1095c-177">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="1095c-177">Security alerts</span></span>     | <span data-ttu-id="1095c-178">43200 分 (30 日間で)</span><span class="sxs-lookup"><span data-stu-id="1095c-178">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="1095c-179">**注:** 既存のアプリケーションと新しいアプリケーションは、サポートされている値を超える必要があります。</span><span class="sxs-lookup"><span data-stu-id="1095c-179">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="1095c-180">将来、作成するか、最大値を超えるサブスクリプションを更新するすべての要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="1095c-180">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="1095c-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1095c-181">Relationships</span></span>

<span data-ttu-id="1095c-182">なし</span><span class="sxs-lookup"><span data-stu-id="1095c-182">None</span></span>

## <a name="methods"></a><span data-ttu-id="1095c-183">メソッド</span><span class="sxs-lookup"><span data-stu-id="1095c-183">Methods</span></span>

| <span data-ttu-id="1095c-184">メソッド</span><span class="sxs-lookup"><span data-stu-id="1095c-184">Method</span></span> | <span data-ttu-id="1095c-185">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1095c-185">Return Type</span></span> | <span data-ttu-id="1095c-186">説明</span><span class="sxs-lookup"><span data-stu-id="1095c-186">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="1095c-187">Create subscription</span><span class="sxs-lookup"><span data-stu-id="1095c-187">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="1095c-188">subscription</span><span class="sxs-lookup"><span data-stu-id="1095c-188">subscription</span></span>](subscription.md) | <span data-ttu-id="1095c-189">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="1095c-189">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="1095c-190">Update subscription</span><span class="sxs-lookup"><span data-stu-id="1095c-190">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="1095c-191">subscription</span><span class="sxs-lookup"><span data-stu-id="1095c-191">subscription</span></span>](subscription.md) | <span data-ttu-id="1095c-192">有効期限を更新することにより、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="1095c-192">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="1095c-193">リストの購読</span><span class="sxs-lookup"><span data-stu-id="1095c-193">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="1095c-194">subscription</span><span class="sxs-lookup"><span data-stu-id="1095c-194">subscription</span></span>](subscription.md) | <span data-ttu-id="1095c-195">アクティブなサブスクリプションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="1095c-195">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="1095c-196">Get subscription</span><span class="sxs-lookup"><span data-stu-id="1095c-196">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="1095c-197">subscription</span><span class="sxs-lookup"><span data-stu-id="1095c-197">subscription</span></span>](subscription.md) | <span data-ttu-id="1095c-198">Subscription オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1095c-198">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="1095c-199">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="1095c-199">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="1095c-200">なし</span><span class="sxs-lookup"><span data-stu-id="1095c-200">None</span></span> | <span data-ttu-id="1095c-201">サブスクリプション オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="1095c-201">Delete a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
