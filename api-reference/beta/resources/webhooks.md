---
title: Microsoft Graph API を使用して変更通知を取得する
description: Microsoft Graph REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。 クライアントは、通知を受信するために自身の URL を構成する Web サービスです。 クライアント アプリは通知を使用して、変更時に状態を更新します。 受信通知をサブスクライブおよび処理する方法などの詳細については、「ユーザーデータの変更の通知を設定する」を参照してください。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 8422328061ac1c2ad736435204b699544bffd2ed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341506"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="8fb87-106">Microsoft Graph API を使用して変更通知を取得する</span><span class="sxs-lookup"><span data-stu-id="8fb87-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fb87-107">Microsoft Graph REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。</span><span class="sxs-lookup"><span data-stu-id="8fb87-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="8fb87-108">クライアントは、通知を受信するために自身の URL を構成する Web サービスです。</span><span class="sxs-lookup"><span data-stu-id="8fb87-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="8fb87-109">クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="8fb87-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="8fb87-110">受信通知をサブスクライブおよび処理する方法などの詳細については、「[ユーザーデータの変更の通知を設定](/graph/webhooks)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fb87-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="8fb87-111">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="8fb87-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="8fb87-112">Outlook [メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-112">Outlook [message][]</span></span>
- <span data-ttu-id="8fb87-113">Outlook [イベント][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-113">Outlook [event][]</span></span>
- <span data-ttu-id="8fb87-114">Outlook 個人用[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="8fb87-115">[user][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-115">[user][]</span></span>
- <span data-ttu-id="8fb87-116">[group][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-116">[group][]</span></span>
- <span data-ttu-id="8fb87-117">Office 365 グループ[会話][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="8fb87-118">ユーザーの個人用 OneDrive 上の_任意のフォルダーの_ [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="8fb87-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="8fb87-119">OneDrive for Business 上の_ルート フォルダーの _ [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="8fb87-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="8fb87-120">セキュリティの[警告][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-120">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="8fb87-121">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8fb87-121">Permissions</span></span>

<span data-ttu-id="8fb87-122">一般に、サブスクリプション操作には、リソースに対する読み取りアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="8fb87-122">In general, subscription operations require read permission to the resource.</span></span> <span data-ttu-id="8fb87-123">たとえば、メッセージの通知を取得するには、アプリに`Mail.Read`アクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="8fb87-123">For example, to get notifications for messages, your app needs the `Mail.Read` permission.</span></span> <span data-ttu-id="8fb87-124">[サブスクリプションの作成](../api/subscription-post-subscriptions.md)の記事には、リソースの種類ごとに必要なアクセス許可が一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="8fb87-124">The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type.</span></span> <span data-ttu-id="8fb87-125">次の表に、特定のリソースの種類に対して webhook を使用するためにアプリが要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="8fb87-125">The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="8fb87-126">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8fb87-126">Permission type</span></span>                        | <span data-ttu-id="8fb87-127">サポートされるリソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fb87-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="8fb87-128">委任された職場または学校のアカウント</span><span class="sxs-lookup"><span data-stu-id="8fb87-128">Delegated - work or school account</span></span>     | <span data-ttu-id="8fb87-129">[通知][]、[連絡先][]、[会話][]、[ドライブアイテム][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="8fb87-130">委任-個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="8fb87-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="8fb87-131">[contact][]、 [drive item][]、 [event][]、 [message][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-131">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="8fb87-132">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8fb87-132">Application</span></span>                            | <span data-ttu-id="8fb87-133">[alert][]、 [contact][]、 [drive item][]、 [event][]、 [group][]、 [message][]、 [user][]</span><span class="sxs-lookup"><span data-stu-id="8fb87-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="8fb87-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="8fb87-134">See also</span></span>

- [<span data-ttu-id="8fb87-135">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="8fb87-135">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="8fb87-136">サブスクリプションのリスト作成</span><span class="sxs-lookup"><span data-stu-id="8fb87-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="8fb87-137">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="8fb87-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="8fb87-138">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="8fb87-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="8fb87-139">Update subscription</span><span class="sxs-lookup"><span data-stu-id="8fb87-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="8fb87-140">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="8fb87-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
