---
title: サブスクリプション リソースの種類
description: 'サブスクリプションは、Microsoft Graph 上のデータの変更に関する通知の受信をクライアント アプリに許可します。 サブスクリプションは現在、以下のリソースで有効です:'
localization_priority: Priority
author: piotrci
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 60219f50b78cf5c636fab1b24aa75922893002fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033970"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="f4b50-104">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4b50-104">subscription resource type</span></span>

<span data-ttu-id="f4b50-105">サブスクリプションは、Microsoft Graph 上のデータの変更に関する通知の受信をクライアント アプリに許可します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="f4b50-106">サブスクリプションは現在、以下のリソースで有効です:</span><span class="sxs-lookup"><span data-stu-id="f4b50-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="f4b50-107">Outlook の[メッセージ][]、[イベント][]、または[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="f4b50-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="f4b50-108">Office 365 グループの[会話][]</span><span class="sxs-lookup"><span data-stu-id="f4b50-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="f4b50-109">OneDrive for Business のルート フォルダー [driveItem][] の階層内にあるコンテンツ、またはユーザーの個人用 OneDrive のルート フォルダーまたはサブフォルダー [driveItem][] の階層内にあるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="f4b50-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="f4b50-110">Azure Active Directory 内の[ユーザー][]または[グループ][]</span><span class="sxs-lookup"><span data-stu-id="f4b50-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="f4b50-111">Microsoft Graph Security API の[警告][]</span><span class="sxs-lookup"><span data-stu-id="f4b50-111">An [alert][] from the Microsoft Graph Security API</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4b50-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4b50-112">JSON representation</span></span>

<span data-ttu-id="f4b50-113">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f4b50-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4b50-114">Properties</span></span>

| <span data-ttu-id="f4b50-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4b50-115">Property</span></span> | <span data-ttu-id="f4b50-116">型</span><span class="sxs-lookup"><span data-stu-id="f4b50-116">Type</span></span> | <span data-ttu-id="f4b50-117">説明</span><span class="sxs-lookup"><span data-stu-id="f4b50-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f4b50-118">changeType</span><span class="sxs-lookup"><span data-stu-id="f4b50-118">changeType</span></span> | <span data-ttu-id="f4b50-119">string</span><span class="sxs-lookup"><span data-stu-id="f4b50-119">string</span></span> | <span data-ttu-id="f4b50-120">必須です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-120">Required.</span></span> <span data-ttu-id="f4b50-121">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="f4b50-122">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="f4b50-123">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="f4b50-123">Multiple values can be combined using a comma-separated list.</span></span><br><br><span data-ttu-id="f4b50-124">注: ドライブ ルート項目の通知では `updated` changeType のみがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f4b50-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="f4b50-125">ユーザーとグループの通知では、`updated` と `deleted` changeType がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f4b50-125">User and group notifications support `updated` and `deleted` changeType.</span></span>|
| <span data-ttu-id="f4b50-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="f4b50-126">notificationUrl</span></span> | <span data-ttu-id="f4b50-127">string</span><span class="sxs-lookup"><span data-stu-id="f4b50-127">string</span></span> | <span data-ttu-id="f4b50-128">必須です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-128">Required.</span></span> <span data-ttu-id="f4b50-129">通知を受け取るエンドポイントの URL です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="f4b50-130">この URL は HTTPS プロトコルを利用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4b50-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="f4b50-131">リソース</span><span class="sxs-lookup"><span data-stu-id="f4b50-131">resource</span></span> | <span data-ttu-id="f4b50-132">string</span><span class="sxs-lookup"><span data-stu-id="f4b50-132">string</span></span> | <span data-ttu-id="f4b50-133">必須です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-133">Required.</span></span> <span data-ttu-id="f4b50-134">変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="f4b50-135">ベース URL (`https://graph.microsoft.com/v1.0/`) は含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f4b50-135">Do not include the base URL (`https://graph.microsoft.com/v1.0/`).</span></span> |
| <span data-ttu-id="f4b50-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f4b50-136">expirationDateTime</span></span> | [<span data-ttu-id="f4b50-137">dateTime</span><span class="sxs-lookup"><span data-stu-id="f4b50-137">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="f4b50-138">必須です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-138">Required.</span></span> <span data-ttu-id="f4b50-139">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="f4b50-140">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="f4b50-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="f4b50-141">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f4b50-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="f4b50-142">clientState</span><span class="sxs-lookup"><span data-stu-id="f4b50-142">clientState</span></span> | <span data-ttu-id="f4b50-143">string</span><span class="sxs-lookup"><span data-stu-id="f4b50-143">string</span></span> | <span data-ttu-id="f4b50-144">オプション。</span><span class="sxs-lookup"><span data-stu-id="f4b50-144">Optional.</span></span> <span data-ttu-id="f4b50-145">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="f4b50-146">最大の長さは 128 文字です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-146">The maximum length is 128 characters.</span></span> <span data-ttu-id="f4b50-147">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="f4b50-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="f4b50-148">id</span><span class="sxs-lookup"><span data-stu-id="f4b50-148">id</span></span> | <span data-ttu-id="f4b50-149">string</span><span class="sxs-lookup"><span data-stu-id="f4b50-149">string</span></span> | <span data-ttu-id="f4b50-p109">サブスクリプションの一意の識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f4b50-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="f4b50-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="f4b50-152">applicationId</span></span> | <span data-ttu-id="f4b50-153">string</span><span class="sxs-lookup"><span data-stu-id="f4b50-153">string</span></span> | <span data-ttu-id="f4b50-154">サブスクリプションを作成するときに使用するアプリケーションの識別子。</span><span class="sxs-lookup"><span data-stu-id="f4b50-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="f4b50-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-155">Read-only.</span></span> |
| <span data-ttu-id="f4b50-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="f4b50-156">creatorId</span></span> | <span data-ttu-id="f4b50-157">string</span><span class="sxs-lookup"><span data-stu-id="f4b50-157">string</span></span> | <span data-ttu-id="f4b50-158">サブスクリプションを作成したユーザーまたはサービス プリンシパルの識別子。</span><span class="sxs-lookup"><span data-stu-id="f4b50-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="f4b50-159">委任されたアクセス許可をアプリで使用してサブスクリプションを作成した場合、このフィールドには、アプリが代理で呼び出しを行っているサインインしているユーザーの ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4b50-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="f4b50-160">アプリがアプリケーション アクセス許可を使用した場合には、このフィールドには、アプリに対応するサービス プリンシパルの ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f4b50-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="f4b50-161">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f4b50-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="f4b50-162">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="f4b50-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="f4b50-163">リソース</span><span class="sxs-lookup"><span data-stu-id="f4b50-163">Resource</span></span>            | <span data-ttu-id="f4b50-164">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="f4b50-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="f4b50-165">ユーザー、グループ、その他のディレクトリ リソース</span><span class="sxs-lookup"><span data-stu-id="f4b50-165">User, group, other directory resources</span></span>   | <span data-ttu-id="f4b50-166">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="f4b50-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4b50-167">メール</span><span class="sxs-lookup"><span data-stu-id="f4b50-167">Mail</span></span>                | <span data-ttu-id="f4b50-168">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="f4b50-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4b50-169">カレンダー</span><span class="sxs-lookup"><span data-stu-id="f4b50-169">Calendar</span></span>            | <span data-ttu-id="f4b50-170">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="f4b50-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4b50-171">連絡先</span><span class="sxs-lookup"><span data-stu-id="f4b50-171">Contacts</span></span>            | <span data-ttu-id="f4b50-172">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="f4b50-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4b50-173">グループ会話</span><span class="sxs-lookup"><span data-stu-id="f4b50-173">Group conversations</span></span> | <span data-ttu-id="f4b50-174">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="f4b50-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4b50-175">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="f4b50-175">Drive root items</span></span>    | <span data-ttu-id="f4b50-176">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="f4b50-176">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="f4b50-177">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="f4b50-177">Security alerts</span></span>     | <span data-ttu-id="f4b50-178">43200 分 (30 日以内)</span><span class="sxs-lookup"><span data-stu-id="f4b50-178">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="f4b50-179">**注:** 既存のアプリケーションと新規アプリケーションのどちらもサポートされている値を超えてはなりません。</span><span class="sxs-lookup"><span data-stu-id="f4b50-179">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="f4b50-180">将来的には、最大値を超えるサブスクリプションを作成または更新する要求はすべて失敗します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-180">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="f4b50-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f4b50-181">Relationships</span></span>

<span data-ttu-id="f4b50-182">なし</span><span class="sxs-lookup"><span data-stu-id="f4b50-182">None</span></span>

## <a name="methods"></a><span data-ttu-id="f4b50-183">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4b50-183">Methods</span></span>

| <span data-ttu-id="f4b50-184">メソッド</span><span class="sxs-lookup"><span data-stu-id="f4b50-184">Method</span></span> | <span data-ttu-id="f4b50-185">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f4b50-185">Return Type</span></span> | <span data-ttu-id="f4b50-186">説明</span><span class="sxs-lookup"><span data-stu-id="f4b50-186">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="f4b50-187">Create subscription</span><span class="sxs-lookup"><span data-stu-id="f4b50-187">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="f4b50-188">subscription</span><span class="sxs-lookup"><span data-stu-id="f4b50-188">subscription</span></span>](subscription.md) | <span data-ttu-id="f4b50-189">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-189">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="f4b50-190">Update subscription</span><span class="sxs-lookup"><span data-stu-id="f4b50-190">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="f4b50-191">subscription</span><span class="sxs-lookup"><span data-stu-id="f4b50-191">subscription</span></span>](subscription.md) | <span data-ttu-id="f4b50-192">有効期限を更新することにより、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-192">Renews a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="f4b50-193">サブスクリプションのリスト作成</span><span class="sxs-lookup"><span data-stu-id="f4b50-193">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="f4b50-194">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="f4b50-194">subscription</span></span>](subscription.md) | <span data-ttu-id="f4b50-195">アクティブなサブスクリプションのリストを作成します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-195">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="f4b50-196">サブスクリプションの取得</span><span class="sxs-lookup"><span data-stu-id="f4b50-196">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="f4b50-197">subscription</span><span class="sxs-lookup"><span data-stu-id="f4b50-197">subscription</span></span>](subscription.md) | <span data-ttu-id="f4b50-198">サブスクリプション オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f4b50-198">Reads properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="f4b50-199">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="f4b50-199">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="f4b50-200">なし</span><span class="sxs-lookup"><span data-stu-id="f4b50-200">None</span></span> |<span data-ttu-id="f4b50-201">サブスクリプション オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="f4b50-201">Deletes a subscription object.</span></span> |

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
[alert]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
