---
title: Microsoft Graph の REST API 通知を使用する
description: プッシュ通知をユーザーに送信するには、Microsoft Graph の API 通知を使用できます。 ターゲットのユーザー アカウントに通知を送信し、プラットフォームはすべてのデバイスのエンドポイントに通知を配布します。 API 通知の要求は、ユーザーの代理アクセス権と [アクセス権許可の通知]( /graph/permissions_reference)を経由して、Microsoft アカウント、または職場 / 学校のアカウントのどちらでも使用することができます。
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 243f412162ed1427c766272d02d58c57ba47cf42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342101"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a><span data-ttu-id="c753d-105">Microsoft Graph の REST API 通知を使用する</span><span class="sxs-lookup"><span data-stu-id="c753d-105">Use the notifications REST API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c753d-106">プッシュ通知をユーザーに送信するには、Microsoft Graph の API 通知を使用できます。</span><span class="sxs-lookup"><span data-stu-id="c753d-106">You can use the notifications API in Microsoft Graph to send push notifications to a user.</span></span> <span data-ttu-id="c753d-107">ターゲットのユーザー アカウントに通知を送信し、プラットフォームはすべてのデバイスのエンドポイントに通知を配布します。</span><span class="sxs-lookup"><span data-stu-id="c753d-107">Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints.</span></span> <span data-ttu-id="c753d-108">API 通知の要求は、ユーザーの[代理アクセス権](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) と[アクセス権許可の通知]( /graph/permissions_reference)を経由して、Microsoft アカウント、または職場 / 学校のアカウントのどちらでも使用することができます。</span><span class="sxs-lookup"><span data-stu-id="c753d-108">Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.</span></span>
<span data-ttu-id="c753d-109">このユーザー中心の通知は[通知](../resources/projectrome-notification.md)リソースによって表示され、 Microsoft Graph で保存されています。</span><span class="sxs-lookup"><span data-stu-id="c753d-109">This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph.</span></span> <span data-ttu-id="c753d-110">[Project Rome SDK APIs](https://github.com/Microsoft/project-rome)を経由する発行アプリケーションによってアクセスし管理することができます。</span><span class="sxs-lookup"><span data-stu-id="c753d-110">It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c753d-111">次の手順</span><span class="sxs-lookup"><span data-stu-id="c753d-111">Next steps</span></span>
- <span data-ttu-id="c753d-112">[通知リソース](../resources/projectrome-notification.md) を参照し、ユーザーに通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="c753d-112">See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users.</span></span> 
- <span data-ttu-id="c753d-113">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。</span><span class="sxs-lookup"><span data-stu-id="c753d-113">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
