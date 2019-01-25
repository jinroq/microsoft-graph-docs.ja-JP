---
title: 変更通知を使用して Microsoft グラフ API を取得するには
description: Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。 クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。 クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。 購読して、着信の通知を処理する方法を含め、詳細については、セットを参照してくださいユーザー データの変更の通知を設定します。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 02ab18d3fa8980211a4937433ad1616b0629bf8c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526215"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="a1c6d-106">変更通知を使用して Microsoft グラフ API を取得するには</span><span class="sxs-lookup"><span data-stu-id="a1c6d-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1c6d-107">Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。</span><span class="sxs-lookup"><span data-stu-id="a1c6d-107">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="a1c6d-108">クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。</span><span class="sxs-lookup"><span data-stu-id="a1c6d-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="a1c6d-109">クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。</span><span class="sxs-lookup"><span data-stu-id="a1c6d-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="a1c6d-110">詳細についてなどを購読、受信通知を処理し、[ユーザー データの変更の通知を設定する](/graph/webhooks)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1c6d-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="a1c6d-111">Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。</span><span class="sxs-lookup"><span data-stu-id="a1c6d-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="a1c6d-112">メッセージ</span><span class="sxs-lookup"><span data-stu-id="a1c6d-112">Messages</span></span>
- <span data-ttu-id="a1c6d-113">イベント</span><span class="sxs-lookup"><span data-stu-id="a1c6d-113">Events</span></span>
- <span data-ttu-id="a1c6d-114">連絡先</span><span class="sxs-lookup"><span data-stu-id="a1c6d-114">Contacts</span></span>
- <span data-ttu-id="a1c6d-115">ユーザー</span><span class="sxs-lookup"><span data-stu-id="a1c6d-115">Users</span></span>
- <span data-ttu-id="a1c6d-116">グループ</span><span class="sxs-lookup"><span data-stu-id="a1c6d-116">Groups</span></span>
- <span data-ttu-id="a1c6d-117">グループ会話</span><span class="sxs-lookup"><span data-stu-id="a1c6d-117">Group conversations</span></span>
- <span data-ttu-id="a1c6d-118">SharePoint サイトに関連付けられたドライブを含む、OneDrive で共有されるコンテンツ</span><span class="sxs-lookup"><span data-stu-id="a1c6d-118">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="a1c6d-119">ユーザーの個人用 OneDrive フォルダー</span><span class="sxs-lookup"><span data-stu-id="a1c6d-119">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="a1c6d-120">セキュリティの警告</span><span class="sxs-lookup"><span data-stu-id="a1c6d-120">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="a1c6d-121">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1c6d-121">Permissions</span></span>

<span data-ttu-id="a1c6d-p103">一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription-post-subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="a1c6d-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="a1c6d-126">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1c6d-126">Permission type</span></span>                        | <span data-ttu-id="a1c6d-127">サポートされているリソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1c6d-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="a1c6d-128">委任 - 職場または学校アカウント</span><span class="sxs-lookup"><span data-stu-id="a1c6d-128">Delegated - work or school account</span></span>     | <span data-ttu-id="a1c6d-129">[連絡先][]、[会話][]、[ドライブ][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]は、[警告][]</span><span class="sxs-lookup"><span data-stu-id="a1c6d-129">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="a1c6d-130">委任 - 個人用の Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="a1c6d-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="a1c6d-131">[問い合わせて][]、[ドライブ][]、[イベント][]、[メッセージ][]</span><span class="sxs-lookup"><span data-stu-id="a1c6d-131">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="a1c6d-132">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1c6d-132">Application</span></span>                            | <span data-ttu-id="a1c6d-133">[連絡先][]、[会話][]、[ドライブ][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]は、[警告][]</span><span class="sxs-lookup"><span data-stu-id="a1c6d-133">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="a1c6d-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="a1c6d-134">See also</span></span>

- [<span data-ttu-id="a1c6d-135">Subscription リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="a1c6d-135">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="a1c6d-136">リストの購読</span><span class="sxs-lookup"><span data-stu-id="a1c6d-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="a1c6d-137">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="a1c6d-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="a1c6d-138">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="a1c6d-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="a1c6d-139">Update subscription</span><span class="sxs-lookup"><span data-stu-id="a1c6d-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="a1c6d-140">サブスクリプションの削除</span><span class="sxs-lookup"><span data-stu-id="a1c6d-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
<span data-ttu-id="a1c6d-148"> 警告 : </span><span class="sxs-lookup"><span data-stu-id="a1c6d-148">[alert]: ./alert.md</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
