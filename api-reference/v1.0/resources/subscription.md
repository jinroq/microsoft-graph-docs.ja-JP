---
title: サブスクリプション リソースの種類
description: 'サブスクリプションは、Microsoft Graph 上のデータの変更に関する通知の受信をクライアント アプリに許可します。 サブスクリプションは現在、以下のリソースで有効です:'
localization_priority: Priority
author: piotrci
ms.openlocfilehash: db3a536395f327115af69f769f37c823013ec7fa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155763"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="4e57c-104">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e57c-104">Subscription resource type</span></span>

<span data-ttu-id="4e57c-105">サブスクリプションは、Microsoft Graph 上のデータの変更に関する通知の受信をクライアント アプリに許可します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-105">A subscription allows a client app to receive notifications about data on the Microsoft Graph.</span></span> <span data-ttu-id="4e57c-106">サブスクリプションは現在、以下のリソースで有効です:</span><span class="sxs-lookup"><span data-stu-id="4e57c-106">Currently, subscriptions are enabled for the following datasets:</span></span>

- <span data-ttu-id="4e57c-107">Outlook の[メッセージ][]、[イベント][]、または[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="4e57c-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="4e57c-108">Office 365 グループの[会話][]</span><span class="sxs-lookup"><span data-stu-id="4e57c-108">[post][] of an Office 365 group</span></span>
- <span data-ttu-id="4e57c-109">OneDrive for Business のルート フォルダー [driveItem][] の階層内にあるコンテンツ、またはユーザーの個人用 OneDrive のルート フォルダーまたはサブフォルダー [driveItem][] の階層内にあるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="4e57c-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="4e57c-110">Azure Active Directory 内の[ユーザー][]または[グループ][]</span><span class="sxs-lookup"><span data-stu-id="4e57c-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="4e57c-111">Microsoft Graph Security API の[警告][]</span><span class="sxs-lookup"><span data-stu-id="4e57c-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e57c-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e57c-112">JSON representation</span></span>

<span data-ttu-id="4e57c-113">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4e57c-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e57c-114">Properties</span></span>

| <span data-ttu-id="4e57c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e57c-115">Property</span></span> | <span data-ttu-id="4e57c-116">型</span><span class="sxs-lookup"><span data-stu-id="4e57c-116">Type</span></span> | <span data-ttu-id="4e57c-117">説明</span><span class="sxs-lookup"><span data-stu-id="4e57c-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="4e57c-118">changeType</span><span class="sxs-lookup"><span data-stu-id="4e57c-118">changeType</span></span> | <span data-ttu-id="4e57c-119">string</span><span class="sxs-lookup"><span data-stu-id="4e57c-119">string</span></span> | <span data-ttu-id="4e57c-120">必須です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-120">Required.</span></span> <span data-ttu-id="4e57c-121">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="4e57c-122">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="4e57c-123">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="4e57c-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="4e57c-124">注: ドライブ ルート項目の通知では `updated` changeType のみがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="4e57c-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="4e57c-125">ユーザーとグループの通知では、`updated` と `deleted` changeType がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="4e57c-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="4e57c-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="4e57c-126">notificationUrl</span></span> | <span data-ttu-id="4e57c-127">string</span><span class="sxs-lookup"><span data-stu-id="4e57c-127">string</span></span> | <span data-ttu-id="4e57c-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-128">Required.</span></span> <span data-ttu-id="4e57c-129">通知を受け取るエンドポイントの URL です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-129">The URL of the application that will receive the push notifications.</span></span> <span data-ttu-id="4e57c-130">この URL は HTTPS プロトコルを利用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e57c-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="4e57c-131">リソース</span><span class="sxs-lookup"><span data-stu-id="4e57c-131">resource</span></span> | <span data-ttu-id="4e57c-132">string</span><span class="sxs-lookup"><span data-stu-id="4e57c-132">string</span></span> | <span data-ttu-id="4e57c-133">必須です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-133">Required.</span></span> <span data-ttu-id="4e57c-134">変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="4e57c-135">ベース URL (`https://graph.microsoft.com/v1.0/`) は含めないでください。</span><span class="sxs-lookup"><span data-stu-id="4e57c-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="4e57c-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4e57c-136">expirationDateTime</span></span> | [<span data-ttu-id="4e57c-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="4e57c-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="4e57c-138">必須です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-138">Required.</span></span> <span data-ttu-id="4e57c-139">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="4e57c-140">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="4e57c-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="4e57c-141">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4e57c-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="4e57c-142">clientState</span><span class="sxs-lookup"><span data-stu-id="4e57c-142">clientState</span></span> | <span data-ttu-id="4e57c-143">string</span><span class="sxs-lookup"><span data-stu-id="4e57c-143">string</span></span> | <span data-ttu-id="4e57c-144">オプション。</span><span class="sxs-lookup"><span data-stu-id="4e57c-144">Optional.</span></span> <span data-ttu-id="4e57c-145">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="4e57c-146">最大の長さは 128 文字です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="4e57c-147">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="4e57c-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="4e57c-148">id</span><span class="sxs-lookup"><span data-stu-id="4e57c-148">id</span></span> | <span data-ttu-id="4e57c-149">string</span><span class="sxs-lookup"><span data-stu-id="4e57c-149">string</span></span> | <span data-ttu-id="4e57c-p109">サブスクリプションの一意の識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4e57c-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="4e57c-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="4e57c-152">applicationId</span></span> | <span data-ttu-id="4e57c-153">string</span><span class="sxs-lookup"><span data-stu-id="4e57c-153">string</span></span> | <span data-ttu-id="4e57c-154">サブスクリプションを作成するときに使用するアプリケーションの識別子。</span><span class="sxs-lookup"><span data-stu-id="4e57c-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="4e57c-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-155">Read-only.</span></span> |
| <span data-ttu-id="4e57c-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="4e57c-156">creatorId</span></span> | <span data-ttu-id="4e57c-157">string</span><span class="sxs-lookup"><span data-stu-id="4e57c-157">string</span></span> | <span data-ttu-id="4e57c-158">サブスクリプションを作成したユーザーまたはサービス プリンシパルの識別子。</span><span class="sxs-lookup"><span data-stu-id="4e57c-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="4e57c-159">委任されたアクセス許可をアプリで使用してサブスクリプションを作成した場合、このフィールドには、アプリが代理で呼び出しを行っているサインインしているユーザーの ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="4e57c-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="4e57c-160">アプリがアプリケーション アクセス許可を使用した場合には、このフィールドには、アプリに対応するサービス プリンシパルの ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="4e57c-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="4e57c-161">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4e57c-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="4e57c-162">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="4e57c-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="4e57c-163">リソース</span><span class="sxs-lookup"><span data-stu-id="4e57c-163">Resource</span></span>            | <span data-ttu-id="4e57c-164">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="4e57c-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="4e57c-165">メール</span><span class="sxs-lookup"><span data-stu-id="4e57c-165">Mail</span></span>                | <span data-ttu-id="4e57c-166">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="4e57c-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4e57c-167">カレンダー</span><span class="sxs-lookup"><span data-stu-id="4e57c-167">Calendar</span></span>            | <span data-ttu-id="4e57c-168">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="4e57c-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4e57c-169">連絡先</span><span class="sxs-lookup"><span data-stu-id="4e57c-169">Contacts</span></span>            | <span data-ttu-id="4e57c-170">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="4e57c-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4e57c-171">グループ会話</span><span class="sxs-lookup"><span data-stu-id="4e57c-171">Group conversations</span></span> | <span data-ttu-id="4e57c-172">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="4e57c-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4e57c-173">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="4e57c-173">Drive root items</span></span>    | <span data-ttu-id="4e57c-174">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="4e57c-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="4e57c-175">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="4e57c-175">Security Alerts</span></span>     | <span data-ttu-id="4e57c-176">43200 分 (30 日以内)</span><span class="sxs-lookup"><span data-stu-id="4e57c-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="4e57c-177">**注:** 既存のアプリケーションと新規アプリケーションのどちらもサポートされている値を超えてはなりません。</span><span class="sxs-lookup"><span data-stu-id="4e57c-177">Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="4e57c-178">将来的には、最大値を超えるサブスクリプションを作成または更新する要求はすべて失敗します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="4e57c-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4e57c-179">Relationships</span></span>

<span data-ttu-id="4e57c-180">なし</span><span class="sxs-lookup"><span data-stu-id="4e57c-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="4e57c-181">メソッド</span><span class="sxs-lookup"><span data-stu-id="4e57c-181">Methods</span></span>

| <span data-ttu-id="4e57c-182">メソッド</span><span class="sxs-lookup"><span data-stu-id="4e57c-182">Method</span></span> | <span data-ttu-id="4e57c-183">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4e57c-183">Return Type</span></span> | <span data-ttu-id="4e57c-184">説明</span><span class="sxs-lookup"><span data-stu-id="4e57c-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="4e57c-185">Create subscription</span><span class="sxs-lookup"><span data-stu-id="4e57c-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="4e57c-186">subscription</span><span class="sxs-lookup"><span data-stu-id="4e57c-186">subscription</span></span>](subscription.md) | <span data-ttu-id="4e57c-187">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="4e57c-188">Update subscription</span><span class="sxs-lookup"><span data-stu-id="4e57c-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="4e57c-189">subscription</span><span class="sxs-lookup"><span data-stu-id="4e57c-189">subscription</span></span>](subscription.md) | <span data-ttu-id="4e57c-190">有効期限を更新することにより、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-190">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="4e57c-191">サブスクリプションのリスト作成</span><span class="sxs-lookup"><span data-stu-id="4e57c-191">List current subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="4e57c-192">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="4e57c-192">subscription</span></span>](subscription.md) | <span data-ttu-id="4e57c-193">アクティブなサブスクリプションのリストを作成します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="4e57c-194">サブスクリプションの取得</span><span class="sxs-lookup"><span data-stu-id="4e57c-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="4e57c-195">subscription</span><span class="sxs-lookup"><span data-stu-id="4e57c-195">subscription</span></span>](subscription.md) | <span data-ttu-id="4e57c-196">サブスクリプション オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4e57c-196">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="4e57c-197">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="4e57c-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="4e57c-198">なし</span><span class="sxs-lookup"><span data-stu-id="4e57c-198">None</span></span> |<span data-ttu-id="4e57c-199">サブスクリプション オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="4e57c-199">Deletes a subscription object.</span></span> |

[連絡先]: ./contact.md
[contact]: ./contact.md
[会話]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[イベント]: ./event.md
[event]: ./event.md
[グループ]: ./group.md
[group]: ./group.md
[メッセージ]: ./message.md
[message]: ./message.md
[ユーザー]: ./user.md
[user]: ./user.md
[警告]: ./alert.md
[alert:]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
