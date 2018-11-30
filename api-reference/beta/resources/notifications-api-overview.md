---
title: 通知の REST API を使用して、Microsoft Graph で
description: Graph API の通知を使用すると、ユーザーにプッシュ通知を送信します。 単に、通知を送信するユーザー アカウントをターゲットし、デバイスのすべてのエンドポイントへの通知の配布には、プラットフォームです。 API の通知の要求が実行アクセス許可を委任し、[通知のアクセス許可]( /graph/permissions_reference)を使用してユーザーの代理としていずれかの Microsoft アカウントを使用できるか、職場、学校のアカウントです。
ms.openlocfilehash: 07b59fb7d7eae2e626b58325e82999bbd36c5489
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069859"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="1c5d9-105">通知の REST API を使用して、Microsoft Graph で</span><span class="sxs-lookup"><span data-stu-id="1c5d9-105">Use the notifications REST API in Microsoft Graph</span></span>

> <span data-ttu-id="1c5d9-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c5d9-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c5d9-108">Graph API の通知を使用すると、ユーザーにプッシュ通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-108">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="1c5d9-109">単に、通知を送信するユーザー アカウントをターゲットし、デバイスのすべてのエンドポイントへの通知の配布には、プラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-109">Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints.</span></span> <span data-ttu-id="1c5d9-110">API の通知の要求が実行[アクセス許可を委任して](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions)、[通知のアクセス許可]( /graph/permissions_reference)を使用してユーザーの代理としていずれかの Microsoft アカウントを使用できるか、職場、学校のアカウントです。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-110">Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.</span></span>
<span data-ttu-id="1c5d9-111">このユーザーを中心とした通知の種類は、[通知](../resources/projectrome-notification.md)リソースで表されますされ、Microsoft Graph で格納されます。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-111">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="1c5d9-112">アクセスおよび管理できる[プロジェクト ローマ SDK Api](https://github.com/Microsoft/project-rome)を通じて公開アプリケーションでします。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-112">It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="next-steps"></a><span data-ttu-id="1c5d9-113">次の手順</span><span class="sxs-lookup"><span data-stu-id="1c5d9-113">Next steps</span></span>
- <span data-ttu-id="1c5d9-114">[通知リソース](../resources/projectrome-notification.md)を参照してくださいし、やり取りを行い、ユーザーへの通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-114">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="1c5d9-115">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試す。</span><span class="sxs-lookup"><span data-stu-id="1c5d9-115">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
