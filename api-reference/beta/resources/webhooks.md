---
title: 変更通知を使用して Microsoft グラフ API を取得するには
description: Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。 クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。 クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。 購読して、着信の通知を処理する方法を含め、詳細については、セットを参照してくださいユーザー データの変更の通知を設定します。
localization_priority: Normal
ms.openlocfilehash: 9b1907d37115e21b41a9e957de9b7ae0a32fd311
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816472"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="ebfaf-106">変更通知を使用して Microsoft グラフ API を取得するには</span><span class="sxs-lookup"><span data-stu-id="ebfaf-106">Use the Microsoft Graph API to get change notifications</span></span>

> <span data-ttu-id="ebfaf-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ebfaf-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebfaf-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebfaf-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebfaf-109">Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。</span><span class="sxs-lookup"><span data-stu-id="ebfaf-109">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="ebfaf-110">クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。</span><span class="sxs-lookup"><span data-stu-id="ebfaf-110">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="ebfaf-111">クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="ebfaf-111">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="ebfaf-112">詳細についてなどを購読、受信通知を処理し、[ユーザー データの変更の通知を設定する](/graph/webhooks)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebfaf-112">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="ebfaf-113">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="ebfaf-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="ebfaf-114">メッセージ</span><span class="sxs-lookup"><span data-stu-id="ebfaf-114">Messages</span></span>
- <span data-ttu-id="ebfaf-115">イベント</span><span class="sxs-lookup"><span data-stu-id="ebfaf-115">Events</span></span>
- <span data-ttu-id="ebfaf-116">連絡先</span><span class="sxs-lookup"><span data-stu-id="ebfaf-116">Contacts</span></span>
- <span data-ttu-id="ebfaf-117">ユーザー</span><span class="sxs-lookup"><span data-stu-id="ebfaf-117">Users</span></span>
- <span data-ttu-id="ebfaf-118">グループ</span><span class="sxs-lookup"><span data-stu-id="ebfaf-118">Groups</span></span>
- <span data-ttu-id="ebfaf-119">グループ会話</span><span class="sxs-lookup"><span data-stu-id="ebfaf-119">Group conversations</span></span>
- <span data-ttu-id="ebfaf-120">SharePoint サイトに関連付けられているドライブを含む、OneDrive で共有されているコンテンツ</span><span class="sxs-lookup"><span data-stu-id="ebfaf-120">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="ebfaf-121">ユーザーの個人用の OneDrive フォルダー</span><span class="sxs-lookup"><span data-stu-id="ebfaf-121">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="ebfaf-122">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="ebfaf-122">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="ebfaf-123">Permissions</span><span class="sxs-lookup"><span data-stu-id="ebfaf-123">Permissions</span></span>

<span data-ttu-id="ebfaf-p104">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription-post-subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ebfaf-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="ebfaf-128">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebfaf-128">Permission type</span></span>                        | <span data-ttu-id="ebfaf-129">サポートされているリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ebfaf-129">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="ebfaf-130">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="ebfaf-130">Delegated - work or school account</span></span>     | <span data-ttu-id="ebfaf-131">[連絡先][]、[会話][]、[ドライブ][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]は、[警告][]</span><span class="sxs-lookup"><span data-stu-id="ebfaf-131">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="ebfaf-132">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="ebfaf-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="ebfaf-133">[問い合わせて][]、[ドライブ][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="ebfaf-133">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="ebfaf-134">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebfaf-134">Application</span></span>                            | <span data-ttu-id="ebfaf-135">[連絡先][]、[会話][]、[ドライブ][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]は、[警告][]</span><span class="sxs-lookup"><span data-stu-id="ebfaf-135">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="ebfaf-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="ebfaf-136">See also</span></span>

- [<span data-ttu-id="ebfaf-137">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="ebfaf-137">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="ebfaf-138">リストの購読</span><span class="sxs-lookup"><span data-stu-id="ebfaf-138">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="ebfaf-139">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="ebfaf-139">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="ebfaf-140">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="ebfaf-140">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="ebfaf-141">Update subscription</span><span class="sxs-lookup"><span data-stu-id="ebfaf-141">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="ebfaf-142">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="ebfaf-142">Delete subscription</span></span>](../api/subscription-delete.md)

[連絡先]: ./contact.md
[contact]: ./contact.md
[会話]: ./conversation.md
[conversation]: ./conversation.md
[ドライブ]: ./drive.md
[drive]: ./drive.md
[イベント]: ./event.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[アラート]: ./alert.md
[alert]: ./alert.md
