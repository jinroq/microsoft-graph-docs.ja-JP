---
title: 変更通知を使用して Microsoft グラフ API を取得するには
description: Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。 クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。 クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。 購読して、着信の通知を処理する方法を含め、詳細については、セットを参照してくださいユーザー データの変更の通知を設定します。
localization_priority: Priority
ms.openlocfilehash: e846e31870e2d14a1e7822cbb9f42682c8b2ac1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860866"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="abbce-106">変更通知を使用して Microsoft グラフ API を取得するには</span><span class="sxs-lookup"><span data-stu-id="abbce-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="abbce-107">Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。</span><span class="sxs-lookup"><span data-stu-id="abbce-107">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="abbce-108">クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。</span><span class="sxs-lookup"><span data-stu-id="abbce-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="abbce-109">クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="abbce-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="abbce-110">詳細についてなどを購読、受信通知を処理し、[ユーザー データの変更の通知を設定する](/graph/webhooks)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abbce-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="abbce-111">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="abbce-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="abbce-112">メッセージ</span><span class="sxs-lookup"><span data-stu-id="abbce-112">Messages</span></span>
- <span data-ttu-id="abbce-113">イベント</span><span class="sxs-lookup"><span data-stu-id="abbce-113">Events</span></span>
- <span data-ttu-id="abbce-114">連絡先</span><span class="sxs-lookup"><span data-stu-id="abbce-114">Contacts</span></span>
- <span data-ttu-id="abbce-115">ユーザー</span><span class="sxs-lookup"><span data-stu-id="abbce-115">Users</span></span>
- <span data-ttu-id="abbce-116">グループ</span><span class="sxs-lookup"><span data-stu-id="abbce-116">Groups</span></span>
- <span data-ttu-id="abbce-117">グループ会話</span><span class="sxs-lookup"><span data-stu-id="abbce-117">Group conversations</span></span>
- <span data-ttu-id="abbce-118">SharePoint サイトに関連付けられているドライブを含む、OneDrive で共有されているコンテンツ</span><span class="sxs-lookup"><span data-stu-id="abbce-118">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="abbce-119">ユーザーの個人用の OneDrive フォルダー</span><span class="sxs-lookup"><span data-stu-id="abbce-119">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="abbce-120">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="abbce-120">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="abbce-121">Permissions</span><span class="sxs-lookup"><span data-stu-id="abbce-121">Permissions</span></span>

<span data-ttu-id="abbce-p103">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription-post-subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="abbce-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="abbce-126">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abbce-126">Permission type</span></span>                        | <span data-ttu-id="abbce-127">サポートされているリソースの種類</span><span class="sxs-lookup"><span data-stu-id="abbce-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="abbce-128">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="abbce-128">Delegated - work or school account</span></span>     | <span data-ttu-id="abbce-129">[連絡先][]、[会話][]、[ドライブ][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]は、[警告][]</span><span class="sxs-lookup"><span data-stu-id="abbce-129">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="abbce-130">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="abbce-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="abbce-131">[問い合わせて][]、[ドライブ][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="abbce-131">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="abbce-132">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abbce-132">Application</span></span>                            | <span data-ttu-id="abbce-133">[連絡先][]、[会話][]、[ドライブ][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]は、[警告][]</span><span class="sxs-lookup"><span data-stu-id="abbce-133">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="abbce-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="abbce-134">See also</span></span>

- [<span data-ttu-id="abbce-135">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="abbce-135">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="abbce-136">リストの購読</span><span class="sxs-lookup"><span data-stu-id="abbce-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="abbce-137">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="abbce-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="abbce-138">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="abbce-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="abbce-139">Update subscription</span><span class="sxs-lookup"><span data-stu-id="abbce-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="abbce-140">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="abbce-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
