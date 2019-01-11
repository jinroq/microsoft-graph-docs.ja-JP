---
title: サブスクリプション リソースの種類
description: サブスクリプションは、Microsoft Graph でデータへの変更に関する通知を受信するクライアント アプリケーションを許可します。 現時点では、サブスクリプションが有効になって次のリソース。
localization_priority: Priority
ms.openlocfilehash: b70daca8eb0f7c303173945b3cacf2cf53af56ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867012"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="178fb-104">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="178fb-104">subscription resource type</span></span>

<span data-ttu-id="178fb-105">サブスクリプションは、Microsoft Graph でデータへの変更に関する通知を受信するクライアント アプリケーションを許可します。</span><span class="sxs-lookup"><span data-stu-id="178fb-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="178fb-106">現時点では、サブスクリプションが有効になって次のリソース。</span><span class="sxs-lookup"><span data-stu-id="178fb-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="178fb-107">メール、イベント、および Outlook の連絡先です。</span><span class="sxs-lookup"><span data-stu-id="178fb-107">Mail, events, and contacts from Outlook.</span></span>
- <span data-ttu-id="178fb-108">Office グループからの会話。</span><span class="sxs-lookup"><span data-stu-id="178fb-108">Conversations from Office Groups.</span></span>
- <span data-ttu-id="178fb-109">OneDrive からドライブのルート項目。</span><span class="sxs-lookup"><span data-stu-id="178fb-109">Drive root items from OneDrive.</span></span>
- <span data-ttu-id="178fb-110">ユーザーと Azure Active Directory のグループ。</span><span class="sxs-lookup"><span data-stu-id="178fb-110">Users and Groups from Azure Active Directory.</span></span>
- <span data-ttu-id="178fb-111">Graph セキュリティ API から通知されます。</span><span class="sxs-lookup"><span data-stu-id="178fb-111">Alerts from the Microsoft Graph Security API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="178fb-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="178fb-112">JSON representation</span></span>

<span data-ttu-id="178fb-113">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="178fb-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="178fb-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="178fb-114">Properties</span></span>

| <span data-ttu-id="178fb-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="178fb-115">Property</span></span> | <span data-ttu-id="178fb-116">種類</span><span class="sxs-lookup"><span data-stu-id="178fb-116">Type</span></span> | <span data-ttu-id="178fb-117">説明</span><span class="sxs-lookup"><span data-stu-id="178fb-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="178fb-118">changeType</span><span class="sxs-lookup"><span data-stu-id="178fb-118">changeType</span></span> | <span data-ttu-id="178fb-119">string</span><span class="sxs-lookup"><span data-stu-id="178fb-119">string</span></span> | <span data-ttu-id="178fb-120">必須。</span><span class="sxs-lookup"><span data-stu-id="178fb-120">Required.</span></span> <span data-ttu-id="178fb-121">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="178fb-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="178fb-122">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="178fb-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="178fb-123">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="178fb-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="178fb-124">メモ: ドライブのルート アイテムの通知だけをサポートして、 `updated` changeType です。</span><span class="sxs-lookup"><span data-stu-id="178fb-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="178fb-125">ユーザーとグループの通知をサポートして`updated`と`deleted`changeType です。</span><span class="sxs-lookup"><span data-stu-id="178fb-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="178fb-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="178fb-126">notificationUrl</span></span> | <span data-ttu-id="178fb-127">文字列</span><span class="sxs-lookup"><span data-stu-id="178fb-127">string</span></span> | <span data-ttu-id="178fb-128">必須。</span><span class="sxs-lookup"><span data-stu-id="178fb-128">Required.</span></span> <span data-ttu-id="178fb-129">通知を受信するエンドポイントの URL。</span><span class="sxs-lookup"><span data-stu-id="178fb-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="178fb-130">この URL が、HTTPS を使用する必要がありますプロトコルです。</span><span class="sxs-lookup"><span data-stu-id="178fb-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="178fb-131">resource</span><span class="sxs-lookup"><span data-stu-id="178fb-131">resource</span></span> | <span data-ttu-id="178fb-132">文字列</span><span class="sxs-lookup"><span data-stu-id="178fb-132">string</span></span> | <span data-ttu-id="178fb-133">必須。</span><span class="sxs-lookup"><span data-stu-id="178fb-133">Required.</span></span> <span data-ttu-id="178fb-134">変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="178fb-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="178fb-135">ベース URL が含まれていない (`https://graph.microsoft.com/v1.0/`)。</span><span class="sxs-lookup"><span data-stu-id="178fb-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="178fb-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="178fb-136">expirationDateTime</span></span> | [<span data-ttu-id="178fb-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="178fb-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="178fb-138">必須。</span><span class="sxs-lookup"><span data-stu-id="178fb-138">Required.</span></span> <span data-ttu-id="178fb-139">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="178fb-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="178fb-140">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="178fb-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="178fb-141">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="178fb-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="178fb-142">clientState</span><span class="sxs-lookup"><span data-stu-id="178fb-142">clientState</span></span> | <span data-ttu-id="178fb-143">string</span><span class="sxs-lookup"><span data-stu-id="178fb-143">string</span></span> | <span data-ttu-id="178fb-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="178fb-144">Optional.</span></span> <span data-ttu-id="178fb-145">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="178fb-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="178fb-146">最大の長さは 128 文字です。</span><span class="sxs-lookup"><span data-stu-id="178fb-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="178fb-147">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="178fb-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="178fb-148">ID</span><span class="sxs-lookup"><span data-stu-id="178fb-148">id</span></span> | <span data-ttu-id="178fb-149">文字列</span><span class="sxs-lookup"><span data-stu-id="178fb-149">string</span></span> | <span data-ttu-id="178fb-p109">サブスクリプションの一意の識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="178fb-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="178fb-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="178fb-152">applicationId</span></span> | <span data-ttu-id="178fb-153">文字列</span><span class="sxs-lookup"><span data-stu-id="178fb-153">string</span></span> | <span data-ttu-id="178fb-154">サブスクリプションを作成するために使用するアプリケーションの識別子です。</span><span class="sxs-lookup"><span data-stu-id="178fb-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="178fb-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="178fb-155">Read-only.</span></span> |
| <span data-ttu-id="178fb-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="178fb-156">creatorId</span></span> | <span data-ttu-id="178fb-157">文字列</span><span class="sxs-lookup"><span data-stu-id="178fb-157">string</span></span> | <span data-ttu-id="178fb-158">ユーザーまたはサブスクリプションを作成するサービス ・ プリンシパルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="178fb-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="178fb-159">使用するアプリケーションがサブスクリプションを作成するアクセス許可を委任する場合、このフィールドは、サインイン中のユーザーの代理で、アプリケーションが呼び出されるの id を含みます。</span><span class="sxs-lookup"><span data-stu-id="178fb-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="178fb-160">アプリケーションは、アプリケーションのアクセス許可を使用する場合、このフィールドには、アプリケーションに対応するサービス ・ プリンシパルの id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="178fb-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="178fb-161">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="178fb-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="178fb-162">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="178fb-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="178fb-163">リソース</span><span class="sxs-lookup"><span data-stu-id="178fb-163">Resource</span></span>            | <span data-ttu-id="178fb-164">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="178fb-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="178fb-165">メール</span><span class="sxs-lookup"><span data-stu-id="178fb-165">Mail</span></span>                | <span data-ttu-id="178fb-166">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="178fb-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="178fb-167">予定表</span><span class="sxs-lookup"><span data-stu-id="178fb-167">Calendar</span></span>            | <span data-ttu-id="178fb-168">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="178fb-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="178fb-169">連絡先</span><span class="sxs-lookup"><span data-stu-id="178fb-169">Contacts</span></span>            | <span data-ttu-id="178fb-170">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="178fb-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="178fb-171">グループ会話</span><span class="sxs-lookup"><span data-stu-id="178fb-171">Group conversations</span></span> | <span data-ttu-id="178fb-172">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="178fb-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="178fb-173">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="178fb-173">Drive root items</span></span>    | <span data-ttu-id="178fb-174">4230 分 (3 日間で)</span><span class="sxs-lookup"><span data-stu-id="178fb-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="178fb-175">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="178fb-175">Security alerts</span></span>     | <span data-ttu-id="178fb-176">43200 分 (30 日間で)</span><span class="sxs-lookup"><span data-stu-id="178fb-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="178fb-177">**注:** 既存のアプリケーションと新しいアプリケーションは、サポートされている値を超える必要があります。</span><span class="sxs-lookup"><span data-stu-id="178fb-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="178fb-178">将来、作成するか、最大値を超えるサブスクリプションを更新するすべての要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="178fb-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="178fb-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="178fb-179">Relationships</span></span>

<span data-ttu-id="178fb-180">なし</span><span class="sxs-lookup"><span data-stu-id="178fb-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="178fb-181">メソッド</span><span class="sxs-lookup"><span data-stu-id="178fb-181">Methods</span></span>

| <span data-ttu-id="178fb-182">メソッド</span><span class="sxs-lookup"><span data-stu-id="178fb-182">Method</span></span> | <span data-ttu-id="178fb-183">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="178fb-183">Return Type</span></span> | <span data-ttu-id="178fb-184">説明</span><span class="sxs-lookup"><span data-stu-id="178fb-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="178fb-185">Create subscription</span><span class="sxs-lookup"><span data-stu-id="178fb-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="178fb-186">subscription</span><span class="sxs-lookup"><span data-stu-id="178fb-186">subscription</span></span>](subscription.md) | <span data-ttu-id="178fb-187">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="178fb-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="178fb-188">Update subscription</span><span class="sxs-lookup"><span data-stu-id="178fb-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="178fb-189">subscription</span><span class="sxs-lookup"><span data-stu-id="178fb-189">subscription</span></span>](subscription.md) | <span data-ttu-id="178fb-190">有効期限を更新することにより、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="178fb-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="178fb-191">リストの購読</span><span class="sxs-lookup"><span data-stu-id="178fb-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="178fb-192">subscription</span><span class="sxs-lookup"><span data-stu-id="178fb-192">subscription</span></span>](subscription.md) | <span data-ttu-id="178fb-193">アクティブなサブスクリプションの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="178fb-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="178fb-194">Get subscription</span><span class="sxs-lookup"><span data-stu-id="178fb-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="178fb-195">subscription</span><span class="sxs-lookup"><span data-stu-id="178fb-195">subscription</span></span>](subscription.md) | <span data-ttu-id="178fb-196">サブスクリプション オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="178fb-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="178fb-197">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="178fb-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="178fb-198">なし</span><span class="sxs-lookup"><span data-stu-id="178fb-198">None</span></span> |<span data-ttu-id="178fb-199">サブスクリプション オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="178fb-199">Deletes a subscription object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
