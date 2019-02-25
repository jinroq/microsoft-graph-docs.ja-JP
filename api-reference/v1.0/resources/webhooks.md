---
title: Microsoft Graph API を使用して変更通知を取得する
description: Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。 クライアントは、通知を受信するために自身の URL を構成する Web サービスです。 クライアント アプリは通知を使用して、変更時に状態を更新します。 着信通知のサブスクライブ方法や処理方法などの詳細については、「ユーザー データの変更に関する通知の設定」をご覧ください。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: 60def6f31ac13ad5417ad3d00e48e700550f6efe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159375"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="b61f1-106">Microsoft Graph API を使用して変更通知を取得する</span><span class="sxs-lookup"><span data-stu-id="b61f1-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="b61f1-107">Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。</span><span class="sxs-lookup"><span data-stu-id="b61f1-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="b61f1-108">クライアントは、通知を受信するために自身の URL を構成する Web サービスです。</span><span class="sxs-lookup"><span data-stu-id="b61f1-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="b61f1-109">クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="b61f1-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="b61f1-110">着信通知のサブスクライブ方法や処理方法などの詳細については、「[ユーザー データの変更に関する通知の設定](/graph/webhooks)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b61f1-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="b61f1-111">Microsoft Graph の API を使用すると、アプリは次のリソースの変更にサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="b61f1-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="b61f1-112">Outlook [メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-112">Outlook [message][]</span></span>
- <span data-ttu-id="b61f1-113">Outlook [イベント][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-113">Outlook [event][]</span></span>
- <span data-ttu-id="b61f1-114">Outlook 個人用[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="b61f1-115">[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-115">[user][]</span></span>
- <span data-ttu-id="b61f1-116">[グループ][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-116">[group][]</span></span>
- <span data-ttu-id="b61f1-117">Office 365 グループ[会話][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-117">[Office 365 group notebooks][]</span></span>
- <span data-ttu-id="b61f1-118">ユーザーの個人用 OneDrive 上の_任意のフォルダーの_ [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="b61f1-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="b61f1-119">OneDrive for Business 上の_ルート フォルダーの _ [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="b61f1-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="b61f1-120">セキュリティの[警告][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-120">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="b61f1-121">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b61f1-121">Permissions</span></span>

<span data-ttu-id="b61f1-p103">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription-post-subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="b61f1-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="b61f1-126">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b61f1-126">Permission type</span></span>                        | <span data-ttu-id="b61f1-127">サポートされているリソースの種類</span><span class="sxs-lookup"><span data-stu-id="b61f1-127">Supported resource types in v1.0</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="b61f1-128">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="b61f1-128">Delegated - work or school account</span></span>     | <span data-ttu-id="b61f1-129">[警告][]、[連絡先][]、[会話][]、[driveItem][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="b61f1-130">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="b61f1-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="b61f1-131">[連絡先][]、[driveItem][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-131">[contact][], [conversation][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="b61f1-132">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b61f1-132">Application</span></span>                            | <span data-ttu-id="b61f1-133">[警告][]、[連絡先][]、[driveItem][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="b61f1-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|


## <a name="see-also"></a><span data-ttu-id="b61f1-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b61f1-134">See also</span></span>

- [<span data-ttu-id="b61f1-135">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b61f1-135">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="b61f1-136">サブスクリプションのリスト作成</span><span class="sxs-lookup"><span data-stu-id="b61f1-136">List current subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="b61f1-137">サブスクリプションの取得</span><span class="sxs-lookup"><span data-stu-id="b61f1-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="b61f1-138">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="b61f1-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="b61f1-139">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="b61f1-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="b61f1-140">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="b61f1-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
