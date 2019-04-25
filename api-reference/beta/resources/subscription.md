---
title: サブスクリプション リソースの種類
description: 'サブスクリプションは、Microsoft Graph 上のデータの変更に関する通知の受信をクライアント アプリに許可します。 サブスクリプションは現在、以下のリソースで有効です:'
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 78b81bb2e2689e17d3f65f35d4ddf9b534728de6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582132"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="b182c-104">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b182c-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b182c-105">サブスクリプションは、Microsoft Graph 上のデータの変更に関する通知の受信をクライアント アプリに許可します。</span><span class="sxs-lookup"><span data-stu-id="b182c-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="b182c-106">サブスクリプションは現在、以下のリソースで有効です:</span><span class="sxs-lookup"><span data-stu-id="b182c-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="b182c-107">Outlook の[メッセージ][]、[イベント][]、または[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="b182c-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="b182c-108">Office 365 グループの[会話][]</span><span class="sxs-lookup"><span data-stu-id="b182c-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="b182c-109">OneDrive for Business のルート フォルダー [driveItem][] の階層内にあるコンテンツ、またはユーザーの個人用 OneDrive のルート フォルダーまたはサブフォルダー [driveItem][] の階層内にあるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="b182c-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="b182c-110">Azure Active Directory 内の[ユーザー][]または[グループ][]</span><span class="sxs-lookup"><span data-stu-id="b182c-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="b182c-111">Microsoft Graph Security API の[警告][]</span><span class="sxs-lookup"><span data-stu-id="b182c-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="b182c-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b182c-112">JSON representation</span></span>

<span data-ttu-id="b182c-113">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b182c-113">Here is a JSON representation of the resource.</span></span>

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
  "lifecycleNotificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="b182c-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b182c-114">Properties</span></span>

| <span data-ttu-id="b182c-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b182c-115">Property</span></span> | <span data-ttu-id="b182c-116">型</span><span class="sxs-lookup"><span data-stu-id="b182c-116">Type</span></span> | <span data-ttu-id="b182c-117">説明</span><span class="sxs-lookup"><span data-stu-id="b182c-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="b182c-118">changeType</span><span class="sxs-lookup"><span data-stu-id="b182c-118">changeType</span></span> | <span data-ttu-id="b182c-119">string</span><span class="sxs-lookup"><span data-stu-id="b182c-119">string</span></span> | <span data-ttu-id="b182c-120">必須。</span><span class="sxs-lookup"><span data-stu-id="b182c-120">Required.</span></span> <span data-ttu-id="b182c-121">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="b182c-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="b182c-122">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="b182c-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="b182c-123">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="b182c-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="b182c-124">注: ドライブ ルート項目の通知では `updated` changeType のみがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="b182c-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="b182c-125">ユーザーとグループの通知では、`updated` と `deleted` changeType がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="b182c-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="b182c-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="b182c-126">notificationUrl</span></span> | <span data-ttu-id="b182c-127">string</span><span class="sxs-lookup"><span data-stu-id="b182c-127">string</span></span> | <span data-ttu-id="b182c-128">必須。</span><span class="sxs-lookup"><span data-stu-id="b182c-128">Required.</span></span> <span data-ttu-id="b182c-129">通知を受信するエンドポイントの URL。</span><span class="sxs-lookup"><span data-stu-id="b182c-129">The URL of the endpoint that receives the notifications.</span></span> <span data-ttu-id="b182c-130">この URL は HTTPS プロトコルを利用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b182c-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="b182c-131">lifecycleNotificationUrl</span><span class="sxs-lookup"><span data-stu-id="b182c-131">lifecycleNotificationUrl</span></span> | <span data-ttu-id="b182c-132">文字列</span><span class="sxs-lookup"><span data-stu-id="b182c-132">string</span></span> | <span data-ttu-id="b182c-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b182c-133">Optional.</span></span> <span data-ttu-id="b182c-134">ライフサイクル通知 (および`subscriptionRemoved` `missed`通知を含む) を受信するエンドポイントの URL。</span><span class="sxs-lookup"><span data-stu-id="b182c-134">The URL of the endpoint that receives lifecycle notifications, including `subscriptionRemoved` and `missed` notifications.</span></span> <span data-ttu-id="b182c-135">指定しない場合、これらの通知は**notificationurl**に配信されます。</span><span class="sxs-lookup"><span data-stu-id="b182c-135">If not provided, those notifications will be delivered to **notificationUrl**.</span></span> <span data-ttu-id="b182c-136">[「](/graph/webhooks-outlook-authz.md) Outlook リソースによるライフサイクル通知の使用方法」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b182c-136">[Read more](/graph/webhooks-outlook-authz.md) about how Outlook resources use lifecycle notifications.</span></span>  <span data-ttu-id="b182c-137">この URL は HTTPS プロトコルを利用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b182c-137">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="b182c-138">リソース</span><span class="sxs-lookup"><span data-stu-id="b182c-138">resource</span></span> | <span data-ttu-id="b182c-139">string</span><span class="sxs-lookup"><span data-stu-id="b182c-139">string</span></span> | <span data-ttu-id="b182c-140">必須。</span><span class="sxs-lookup"><span data-stu-id="b182c-140">Required.</span></span> <span data-ttu-id="b182c-141">変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="b182c-141">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="b182c-142">ベース URL (`https://graph.microsoft.com/beta/`) は含めないでください。</span><span class="sxs-lookup"><span data-stu-id="b182c-142">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="b182c-143">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b182c-143">expirationDateTime</span></span> | <span data-ttu-id="b182c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b182c-144">DateTimeOffset</span></span> | <span data-ttu-id="b182c-145">必須です。</span><span class="sxs-lookup"><span data-stu-id="b182c-145">Required.</span></span> <span data-ttu-id="b182c-146">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="b182c-146">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="b182c-147">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="b182c-147">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="b182c-148">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b182c-148">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="b182c-149">clientState</span><span class="sxs-lookup"><span data-stu-id="b182c-149">clientState</span></span> | <span data-ttu-id="b182c-150">文字列</span><span class="sxs-lookup"><span data-stu-id="b182c-150">string</span></span> | <span data-ttu-id="b182c-151">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b182c-151">Optional.</span></span> <span data-ttu-id="b182c-152">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b182c-152">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="b182c-153">最大の長さは 255 文字です。</span><span class="sxs-lookup"><span data-stu-id="b182c-153">The maximum length is 255 characters.</span></span> <span data-ttu-id="b182c-154">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティを比較することで、その通知がサービスから来たことを確認できます</span><span class="sxs-lookup"><span data-stu-id="b182c-154">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="b182c-155">id</span><span class="sxs-lookup"><span data-stu-id="b182c-155">id</span></span> | <span data-ttu-id="b182c-156">文字列</span><span class="sxs-lookup"><span data-stu-id="b182c-156">string</span></span> | <span data-ttu-id="b182c-p110">サブスクリプションの一意の識別子です。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b182c-p110">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="b182c-159">applicationId</span><span class="sxs-lookup"><span data-stu-id="b182c-159">applicationId</span></span> | <span data-ttu-id="b182c-160">string</span><span class="sxs-lookup"><span data-stu-id="b182c-160">string</span></span> | <span data-ttu-id="b182c-161">サブスクリプションを作成するときに使用するアプリケーションの識別子。</span><span class="sxs-lookup"><span data-stu-id="b182c-161">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="b182c-162">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b182c-162">Read-only.</span></span> |
| <span data-ttu-id="b182c-163">creatorId</span><span class="sxs-lookup"><span data-stu-id="b182c-163">creatorId</span></span> | <span data-ttu-id="b182c-164">string</span><span class="sxs-lookup"><span data-stu-id="b182c-164">string</span></span> | <span data-ttu-id="b182c-165">サブスクリプションを作成したユーザーまたはサービス プリンシパルの識別子。</span><span class="sxs-lookup"><span data-stu-id="b182c-165">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="b182c-166">委任されたアクセス許可をアプリで使用してサブスクリプションを作成した場合、このフィールドには、アプリが代理で呼び出しを行っているサインインしているユーザーの ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b182c-166">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="b182c-167">アプリがアプリケーション アクセス許可を使用した場合には、このフィールドには、アプリに対応するサービス プリンシパルの ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b182c-167">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="b182c-168">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b182c-168">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="b182c-169">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="b182c-169">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="b182c-170">リソース</span><span class="sxs-lookup"><span data-stu-id="b182c-170">Resource</span></span>            | <span data-ttu-id="b182c-171">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="b182c-171">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="b182c-172">メール</span><span class="sxs-lookup"><span data-stu-id="b182c-172">Mail</span></span>                | <span data-ttu-id="b182c-173">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="b182c-173">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b182c-174">カレンダー</span><span class="sxs-lookup"><span data-stu-id="b182c-174">Calendar</span></span>            | <span data-ttu-id="b182c-175">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="b182c-175">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b182c-176">連絡先</span><span class="sxs-lookup"><span data-stu-id="b182c-176">Contacts</span></span>            | <span data-ttu-id="b182c-177">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="b182c-177">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b182c-178">グループ会話</span><span class="sxs-lookup"><span data-stu-id="b182c-178">Group conversations</span></span> | <span data-ttu-id="b182c-179">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="b182c-179">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b182c-180">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="b182c-180">Drive root items</span></span>    | <span data-ttu-id="b182c-181">4230 分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="b182c-181">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="b182c-182">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="b182c-182">Security alerts</span></span>     | <span data-ttu-id="b182c-183">43200 分 (30 日以内)</span><span class="sxs-lookup"><span data-stu-id="b182c-183">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="b182c-184">**注:** 既存のアプリケーションと新規アプリケーションのどちらもサポートされている値を超えてはなりません。</span><span class="sxs-lookup"><span data-stu-id="b182c-184">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="b182c-185">将来的には、最大値を超えるサブスクリプションを作成または更新する要求はすべて失敗します。</span><span class="sxs-lookup"><span data-stu-id="b182c-185">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="b182c-186">関係</span><span class="sxs-lookup"><span data-stu-id="b182c-186">Relationships</span></span>

<span data-ttu-id="b182c-187">なし</span><span class="sxs-lookup"><span data-stu-id="b182c-187">None</span></span>

## <a name="methods"></a><span data-ttu-id="b182c-188">メソッド</span><span class="sxs-lookup"><span data-stu-id="b182c-188">Methods</span></span>

| <span data-ttu-id="b182c-189">メソッド</span><span class="sxs-lookup"><span data-stu-id="b182c-189">Method</span></span> | <span data-ttu-id="b182c-190">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b182c-190">Return Type</span></span> | <span data-ttu-id="b182c-191">説明</span><span class="sxs-lookup"><span data-stu-id="b182c-191">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="b182c-192">Create subscription</span><span class="sxs-lookup"><span data-stu-id="b182c-192">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="b182c-193">subscription</span><span class="sxs-lookup"><span data-stu-id="b182c-193">subscription</span></span>](subscription.md) | <span data-ttu-id="b182c-194">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="b182c-194">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="b182c-195">Update subscription</span><span class="sxs-lookup"><span data-stu-id="b182c-195">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="b182c-196">subscription</span><span class="sxs-lookup"><span data-stu-id="b182c-196">subscription</span></span>](subscription.md) | <span data-ttu-id="b182c-197">有効期限を更新して、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="b182c-197">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="b182c-198">サブスクリプションのリスト作成</span><span class="sxs-lookup"><span data-stu-id="b182c-198">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="b182c-199">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="b182c-199">subscription</span></span>](subscription.md) | <span data-ttu-id="b182c-200">アクティブなサブスクリプションのリストを作成します。</span><span class="sxs-lookup"><span data-stu-id="b182c-200">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="b182c-201">サブスクリプションの取得</span><span class="sxs-lookup"><span data-stu-id="b182c-201">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="b182c-202">subscription</span><span class="sxs-lookup"><span data-stu-id="b182c-202">subscription</span></span>](subscription.md) | <span data-ttu-id="b182c-203">subscription オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b182c-203">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="b182c-204">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="b182c-204">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="b182c-205">なし</span><span class="sxs-lookup"><span data-stu-id="b182c-205">None</span></span> | <span data-ttu-id="b182c-206">サブスクリプションオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="b182c-206">Delete a subscription object.</span></span> |

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
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
