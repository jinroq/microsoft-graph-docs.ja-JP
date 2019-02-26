---
title: Microsoft Graph API を使用して変更通知を取得する
description: Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。 クライアントは、通知を受信するために自身の URL を構成する Web サービスです。 クライアント アプリは通知を使用して、変更時に状態を更新します。 着信通知のサブスクライブ方法や処理方法などの詳細については、「ユーザー データの変更に関する通知の設定」をご覧ください。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1d7a3d868ffc640f7659623942ac102575fb94fc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151493"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="54271-106">Microsoft Graph API を使用して変更通知を取得する</span><span class="sxs-lookup"><span data-stu-id="54271-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54271-107">Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。</span><span class="sxs-lookup"><span data-stu-id="54271-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="54271-108">クライアントは、通知を受信するために自身の URL を構成する Web サービスです。</span><span class="sxs-lookup"><span data-stu-id="54271-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="54271-109">クライアント アプリは通知を使用して、変更時に状態を更新します。</span><span class="sxs-lookup"><span data-stu-id="54271-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="54271-110">着信通知のサブスクライブ方法や処理方法などの詳細については、「[ユーザー データの変更に関する通知の設定](/graph/webhooks)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="54271-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="54271-111">Microsoft Graph の API を使用すると、アプリは次のリソースの変更にサブスクライブできます。</span><span class="sxs-lookup"><span data-stu-id="54271-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="54271-112">Outlook [メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="54271-112">Outlook [message][]</span></span>
- <span data-ttu-id="54271-113">Outlook [イベント][]</span><span class="sxs-lookup"><span data-stu-id="54271-113">Outlook [event][]</span></span>
- <span data-ttu-id="54271-114">Outlook 個人用[連絡先][]</span><span class="sxs-lookup"><span data-stu-id="54271-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="54271-115">[user][]</span><span class="sxs-lookup"><span data-stu-id="54271-115">[user][]</span></span>
- <span data-ttu-id="54271-116">[group][]</span><span class="sxs-lookup"><span data-stu-id="54271-116">[group][]</span></span>
- <span data-ttu-id="54271-117">Office 365 グループ[会話][]</span><span class="sxs-lookup"><span data-stu-id="54271-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="54271-118">ユーザーの個人用 OneDrive 上の_任意のフォルダー_の [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="54271-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="54271-119">OneDrive for Business 上の_ルート フォルダー_の [driveItem][] 階層内のコンテンツ</span><span class="sxs-lookup"><span data-stu-id="54271-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="54271-120">セキュリティの[警告][]</span><span class="sxs-lookup"><span data-stu-id="54271-120">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="54271-121">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="54271-121">Permissions</span></span>

<span data-ttu-id="54271-p103">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription-post-subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="54271-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="54271-126">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54271-126">Permission type</span></span>                        | <span data-ttu-id="54271-127">サポートされているリソースの種類</span><span class="sxs-lookup"><span data-stu-id="54271-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="54271-128">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="54271-128">Delegated - work or school account</span></span>     | <span data-ttu-id="54271-129">[警告][]、[連絡先][]、[会話][]、[driveItem][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="54271-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="54271-130">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="54271-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="54271-131">[連絡先][]、[driveItem][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="54271-131">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="54271-132">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54271-132">Application</span></span>                            | <span data-ttu-id="54271-133">[警告][]、[連絡先][]、[driveItem][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]</span><span class="sxs-lookup"><span data-stu-id="54271-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="54271-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="54271-134">See also</span></span>

- [<span data-ttu-id="54271-135">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54271-135">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="54271-136">サブスクリプションのリスト作成</span><span class="sxs-lookup"><span data-stu-id="54271-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="54271-137">サブスクリプションの取得</span><span class="sxs-lookup"><span data-stu-id="54271-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="54271-138">サブスクリプションの作成</span><span class="sxs-lookup"><span data-stu-id="54271-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="54271-139">サブスクリプションの更新</span><span class="sxs-lookup"><span data-stu-id="54271-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="54271-140">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="54271-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
