---
title: 'Microsoft Graph の通知機能を統合する '
description: '通知は、アプリケーションのユーザーと再びやり取りするのに最も効果的な方法の 1 つです。 いくつかの簡単な手順で、アプリと Microsoft Graph の通知を統合することができます。  '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: 2f3a126ade92ff1615848f9f4db846aebb62d5f7
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063359"
---
# <a name="integrate-with-microsoft-graph-notifications"></a><span data-ttu-id="727fe-104">Microsoft Graph の通知機能を統合する</span><span class="sxs-lookup"><span data-stu-id="727fe-104">Integrate with Microsoft Graph notifications</span></span>

<span data-ttu-id="727fe-105">次の図に示されているように、いくつかの簡単な手順で、アプリと Microsoft Graph の通知を統合することができます。</span><span class="sxs-lookup"><span data-stu-id="727fe-105">You can integrate your apps with Microsoft Graph notifications with a few simple steps, as shown in the following diagram.</span></span>

![参加通知の手順を示す図: 登録、デバイス間のオンボーディング、サーバーの統合、およびクライアントの統合](images/notifications-integration-e2e-overview.png)

1.  <span data-ttu-id="727fe-107">アプリケーションを Microsoft Azure ポータルに[登録](notifications-integration-app-registration.md)します。</span><span class="sxs-lookup"><span data-stu-id="727fe-107"> Register a new application in the Azure portal</span></span>

2.  <span data-ttu-id="727fe-108">クロス プラットフォームのアプリケーション ID とプッシュ通知認証情報を取得するために、パートナー センター/Windows デベロッパー センターに[参加](notifications-integration-cross-device-experiences-onboarding.md)します。</span><span class="sxs-lookup"><span data-stu-id="727fe-108">[Onboard](notifications-integration-cross-device-experiences-onboarding.md) to Partner Center/Windows Dev Center for cross-platform application identity and push notification credentials.</span></span>

3.  <span data-ttu-id="727fe-109">Microsoft Graph を経由して通知を送信するように[アプリケーション サーバーを設定](notifications-integrating-app-server.md)します。</span><span class="sxs-lookup"><span data-stu-id="727fe-109">[Set up your app server](notifications-integrating-app-server.md) to send notifications via Microsoft Graph.</span></span>

4.  <span data-ttu-id="727fe-110">[Microsoft Graph 通知クライアント SDK](https://github.com/microsoft/project-rome) を Windows、Android、または iOS アプリに[統合](notifications-integrating-with-windows.md)して、通知を受信および管理します。</span><span class="sxs-lookup"><span data-stu-id="727fe-110">[Integrate](notifications-integrating-with-windows.md) the [Microsoft Graph notifications client SDK](https://github.com/microsoft/project-rome) into your Windows, Android, or iOS app clients to receive and manage notifications.</span></span>
