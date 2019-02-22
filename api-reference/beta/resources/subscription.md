---
title: subscription リソースの種類
description: サブスクリプションを使用すると、クライアントアプリは Microsoft Graph のデータに対する変更に関する通知を受け取ることができます。 現時点では、以下のリソースのサブスクリプションが有効になっています。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 9de48cc6a3e5dde459673117d9ee00a34477faf6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163939"
---
# <a name="subscription-resource-type"></a><span data-ttu-id="6c71b-104">subscription リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c71b-104">subscription resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c71b-105">サブスクリプションを使用すると、クライアントアプリは Microsoft Graph のデータに対する変更に関する通知を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="6c71b-105">A subscription allows a client app to receive notifications about changes to data in Microsoft Graph.</span></span> <span data-ttu-id="6c71b-106">現時点では、以下のリソースのサブスクリプションが有効になっています。</span><span class="sxs-lookup"><span data-stu-id="6c71b-106">Currently, subscriptions are enabled for the following resources:</span></span>

- <span data-ttu-id="6c71b-107">Outlook の[メッセージ][]、[イベント][]、または[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="6c71b-107">A [message][], [event][], or [contact][] in Outlook</span></span>
- <span data-ttu-id="6c71b-108">Office 365 グループの[会話][]</span><span class="sxs-lookup"><span data-stu-id="6c71b-108">A [conversation][] of an Office 365 group</span></span>
- <span data-ttu-id="6c71b-109">onedrive for business のルートフォルダーのファイル[][]の階層内のコンテンツ、またはユーザーの個人用 OneDrive のルートフォルダーまたはサブフォルダの[ドライブ項目][]。</span><span class="sxs-lookup"><span data-stu-id="6c71b-109">Content in the hierarchy of a root folder [driveItem][] in OneDrive for Business, or of a root folder or subfolder [driveItem][] in a user's personal OneDrive</span></span>
- <span data-ttu-id="6c71b-110">Azure Active Directory の[ユーザー][]または[グループ][]</span><span class="sxs-lookup"><span data-stu-id="6c71b-110">A [user][] or [group][] in Azure Active Directory</span></span>
- <span data-ttu-id="6c71b-111">Microsoft Graph セキュリティ API からの[警告][]</span><span class="sxs-lookup"><span data-stu-id="6c71b-111">An [alert][] from the Microsoft Graph Security API</span></span>


## <a name="json-representation"></a><span data-ttu-id="6c71b-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c71b-112">JSON representation</span></span>

<span data-ttu-id="6c71b-113">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c71b-113">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6c71b-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c71b-114">Properties</span></span>

| <span data-ttu-id="6c71b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c71b-115">Property</span></span> | <span data-ttu-id="6c71b-116">型</span><span class="sxs-lookup"><span data-stu-id="6c71b-116">Type</span></span> | <span data-ttu-id="6c71b-117">説明</span><span class="sxs-lookup"><span data-stu-id="6c71b-117">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="6c71b-118">changeType</span><span class="sxs-lookup"><span data-stu-id="6c71b-118">changeType</span></span> | <span data-ttu-id="6c71b-119">string</span><span class="sxs-lookup"><span data-stu-id="6c71b-119">string</span></span> | <span data-ttu-id="6c71b-120">必須。</span><span class="sxs-lookup"><span data-stu-id="6c71b-120">Required.</span></span> <span data-ttu-id="6c71b-121">登録しているリソース内の、通知を上げる変更の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-121">Indicates the type of change in the subscribed resource that will raise a notification.</span></span> <span data-ttu-id="6c71b-122">サポートされている値は `created`、`updated`、`deleted` です。</span><span class="sxs-lookup"><span data-stu-id="6c71b-122">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="6c71b-123">コンマ区切りのリストを使用して複数値を結合できます。</span><span class="sxs-lookup"><span data-stu-id="6c71b-123">Multiple values can be combined using a comma-separated list.</span></span> <br><br><span data-ttu-id="6c71b-124">注: ドライブのルートアイテムの通知で`updated`は、changeType のみがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="6c71b-124">Note: Drive root item notifications support only the `updated` changeType.</span></span> <span data-ttu-id="6c71b-125">ユーザーおよびグループの通知`updated`の`deleted`サポートと changeType。</span><span class="sxs-lookup"><span data-stu-id="6c71b-125">User and group notifications support `updated` and `deleted` changeType.</span></span> |
| <span data-ttu-id="6c71b-126">notificationUrl</span><span class="sxs-lookup"><span data-stu-id="6c71b-126">notificationUrl</span></span> | <span data-ttu-id="6c71b-127">string</span><span class="sxs-lookup"><span data-stu-id="6c71b-127">string</span></span> | <span data-ttu-id="6c71b-128">必須。</span><span class="sxs-lookup"><span data-stu-id="6c71b-128">Required.</span></span> <span data-ttu-id="6c71b-129">通知を受信するエンドポイントの URL。</span><span class="sxs-lookup"><span data-stu-id="6c71b-129">The URL of the endpoint that will receive the notifications.</span></span> <span data-ttu-id="6c71b-130">この URL には、HTTPS プロトコルを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c71b-130">This URL must make use of the HTTPS protocol.</span></span> |
| <span data-ttu-id="6c71b-131">リソース</span><span class="sxs-lookup"><span data-stu-id="6c71b-131">resource</span></span> | <span data-ttu-id="6c71b-132">文字列</span><span class="sxs-lookup"><span data-stu-id="6c71b-132">string</span></span> | <span data-ttu-id="6c71b-133">必須。</span><span class="sxs-lookup"><span data-stu-id="6c71b-133">Required.</span></span> <span data-ttu-id="6c71b-134">変更の監視対象となるリソースを指定します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-134">Specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="6c71b-135">ベース URL (`https://graph.microsoft.com/beta/`) は含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6c71b-135">Do not include the base URL (`https://graph.microsoft.com/beta/`).</span></span> |
| <span data-ttu-id="6c71b-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6c71b-136">expirationDateTime</span></span> | <span data-ttu-id="6c71b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c71b-137">DateTimeOffset</span></span> | <span data-ttu-id="6c71b-138">必須です。</span><span class="sxs-lookup"><span data-stu-id="6c71b-138">Required.</span></span> <span data-ttu-id="6c71b-139">webhook サブスクリプションの有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-139">Specifies the date and time when the webhook subscription expires.</span></span> <span data-ttu-id="6c71b-140">時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。</span><span class="sxs-lookup"><span data-stu-id="6c71b-140">The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to.</span></span>  <span data-ttu-id="6c71b-141">サポートされているサブスクリプションの最長時間については、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6c71b-141">See the table below for maximum supported subscription length of time.</span></span> |
| <span data-ttu-id="6c71b-142">clientState</span><span class="sxs-lookup"><span data-stu-id="6c71b-142">clientState</span></span> | <span data-ttu-id="6c71b-143">string</span><span class="sxs-lookup"><span data-stu-id="6c71b-143">string</span></span> | <span data-ttu-id="6c71b-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6c71b-144">Optional.</span></span> <span data-ttu-id="6c71b-145">各通知内のサービスによって送信される `clientState` プロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-145">Specifies the value of the `clientState` property sent by the service in each notification.</span></span> <span data-ttu-id="6c71b-146">最大の長さは、255 文字です。</span><span class="sxs-lookup"><span data-stu-id="6c71b-146">The maximum length is 255 characters.</span></span> <span data-ttu-id="6c71b-147">クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="6c71b-147">The client can check that the notification came from the service by comparing the value of the `clientState` property sent with the subscription with the value of the `clientState` property received with each notification.</span></span> |
| <span data-ttu-id="6c71b-148">id</span><span class="sxs-lookup"><span data-stu-id="6c71b-148">id</span></span> | <span data-ttu-id="6c71b-149">string</span><span class="sxs-lookup"><span data-stu-id="6c71b-149">string</span></span> | <span data-ttu-id="6c71b-p109">サブスクリプションの一意の識別子です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6c71b-p109">Unique identifier for the subscription. Read-only.</span></span> |
| <span data-ttu-id="6c71b-152">applicationId</span><span class="sxs-lookup"><span data-stu-id="6c71b-152">applicationId</span></span> | <span data-ttu-id="6c71b-153">string</span><span class="sxs-lookup"><span data-stu-id="6c71b-153">string</span></span> | <span data-ttu-id="6c71b-154">サブスクリプションの作成に使用されたアプリケーションの識別子。</span><span class="sxs-lookup"><span data-stu-id="6c71b-154">Identifier of the application used to create the subscription.</span></span> <span data-ttu-id="6c71b-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6c71b-155">Read-only.</span></span> |
| <span data-ttu-id="6c71b-156">creatorId</span><span class="sxs-lookup"><span data-stu-id="6c71b-156">creatorId</span></span> | <span data-ttu-id="6c71b-157">string</span><span class="sxs-lookup"><span data-stu-id="6c71b-157">string</span></span> | <span data-ttu-id="6c71b-158">サブスクリプションを作成したユーザーまたはサービスプリンシパルの識別子。</span><span class="sxs-lookup"><span data-stu-id="6c71b-158">Identifier of the user or service principal that created the subscription.</span></span> <span data-ttu-id="6c71b-159">アプリがサブスクリプションを作成するために委任されたアクセス許可を使用している場合、このフィールドには、アプリが代理で呼び出した、サインインしているユーザーの id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c71b-159">If the app used delegated permissions to create the subscription, this field contains the id of the signed-in user the app called on behalf of.</span></span> <span data-ttu-id="6c71b-160">アプリがアプリケーションのアクセス許可を使用している場合、このフィールドには、アプリに対応するサービスプリンシパルの id が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6c71b-160">If the app used application permissions, this field contains the id of the service principal corresponding to the app.</span></span> <span data-ttu-id="6c71b-161">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6c71b-161">Read-only.</span></span> |

## <a name="maximum-length-of-subscription-per-resource-type"></a><span data-ttu-id="6c71b-162">リソースの種類別のサブスクリプションの最大の長さ</span><span class="sxs-lookup"><span data-stu-id="6c71b-162">Maximum length of subscription per resource type</span></span>

| <span data-ttu-id="6c71b-163">リソース</span><span class="sxs-lookup"><span data-stu-id="6c71b-163">Resource</span></span>            | <span data-ttu-id="6c71b-164">最大有効期限</span><span class="sxs-lookup"><span data-stu-id="6c71b-164">Maximum Expiration Time</span></span>  |
|:--------------------|:-------------------------|
| <span data-ttu-id="6c71b-165">メール</span><span class="sxs-lookup"><span data-stu-id="6c71b-165">Mail</span></span>                | <span data-ttu-id="6c71b-166">4230分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="6c71b-166">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="6c71b-167">カレンダー</span><span class="sxs-lookup"><span data-stu-id="6c71b-167">Calendar</span></span>            | <span data-ttu-id="6c71b-168">4230分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="6c71b-168">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="6c71b-169">連絡先</span><span class="sxs-lookup"><span data-stu-id="6c71b-169">Contacts</span></span>            | <span data-ttu-id="6c71b-170">4230分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="6c71b-170">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="6c71b-171">グループ会話</span><span class="sxs-lookup"><span data-stu-id="6c71b-171">Group conversations</span></span> | <span data-ttu-id="6c71b-172">4230分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="6c71b-172">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="6c71b-173">ドライブ ルート項目</span><span class="sxs-lookup"><span data-stu-id="6c71b-173">Drive root items</span></span>    | <span data-ttu-id="6c71b-174">4230分 (3 日以内)</span><span class="sxs-lookup"><span data-stu-id="6c71b-174">4230 minutes (under 3 days)</span></span>    |
| <span data-ttu-id="6c71b-175">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="6c71b-175">Security alerts</span></span>     | <span data-ttu-id="6c71b-176">43200分 (30 日以内)</span><span class="sxs-lookup"><span data-stu-id="6c71b-176">43200 minutes (under 30 days)</span></span>  |

> <span data-ttu-id="6c71b-177">**注:** 既存のアプリケーションと新しいアプリケーションは、サポートされている値を超えないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c71b-177">**Note:** Existing applications and new applications should not exceed the supported value.</span></span> <span data-ttu-id="6c71b-178">その後、最大値を超えるサブスクリプションを作成または更新する要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-178">In the future, any requests to create or renew a subscription beyond the maximum value will fail.</span></span>

## <a name="relationships"></a><span data-ttu-id="6c71b-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c71b-179">Relationships</span></span>

<span data-ttu-id="6c71b-180">なし</span><span class="sxs-lookup"><span data-stu-id="6c71b-180">None</span></span>

## <a name="methods"></a><span data-ttu-id="6c71b-181">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c71b-181">Methods</span></span>

| <span data-ttu-id="6c71b-182">メソッド</span><span class="sxs-lookup"><span data-stu-id="6c71b-182">Method</span></span> | <span data-ttu-id="6c71b-183">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6c71b-183">Return Type</span></span> | <span data-ttu-id="6c71b-184">説明</span><span class="sxs-lookup"><span data-stu-id="6c71b-184">Description</span></span> |
|:-------|:------------|:------------|
| [<span data-ttu-id="6c71b-185">Create subscription</span><span class="sxs-lookup"><span data-stu-id="6c71b-185">Create subscription</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="6c71b-186">subscription</span><span class="sxs-lookup"><span data-stu-id="6c71b-186">subscription</span></span>](subscription.md) | <span data-ttu-id="6c71b-187">Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-187">Subscribes a listener application to receive notifications when Microsoft Graph data changes.</span></span> |
| [<span data-ttu-id="6c71b-188">Update subscription</span><span class="sxs-lookup"><span data-stu-id="6c71b-188">Update subscription</span></span>](../api/subscription-update.md) | [<span data-ttu-id="6c71b-189">subscription</span><span class="sxs-lookup"><span data-stu-id="6c71b-189">subscription</span></span>](subscription.md) | <span data-ttu-id="6c71b-190">有効期限を更新して、サブスクリプションを更新します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-190">Renew a subscription by updating its expiration time.</span></span> |
| [<span data-ttu-id="6c71b-191">サブスクリプションの一覧表示</span><span class="sxs-lookup"><span data-stu-id="6c71b-191">List subscriptions</span></span>](../api/subscription-list.md) | [<span data-ttu-id="6c71b-192">subscription</span><span class="sxs-lookup"><span data-stu-id="6c71b-192">subscription</span></span>](subscription.md) | <span data-ttu-id="6c71b-193">アクティブなサブスクリプションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-193">Lists active subscriptions.</span></span> |
| [<span data-ttu-id="6c71b-194">Get subscription</span><span class="sxs-lookup"><span data-stu-id="6c71b-194">Get subscription</span></span>](../api/subscription-get.md) | [<span data-ttu-id="6c71b-195">subscription</span><span class="sxs-lookup"><span data-stu-id="6c71b-195">subscription</span></span>](subscription.md) | <span data-ttu-id="6c71b-196">subscription オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6c71b-196">Read properties and relationships of subscription object.</span></span> |
| [<span data-ttu-id="6c71b-197">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="6c71b-197">Delete subscription</span></span>](../api/subscription-delete.md) | <span data-ttu-id="6c71b-198">なし</span><span class="sxs-lookup"><span data-stu-id="6c71b-198">None</span></span> | <span data-ttu-id="6c71b-199">サブスクリプションオブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="6c71b-199">Delete a subscription object.</span></span> |

[連絡先]: ./contact.md
[contact]: ./contact.md
[会話]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[通知]: ./alert.md
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
