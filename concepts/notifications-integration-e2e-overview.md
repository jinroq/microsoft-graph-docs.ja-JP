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
# <a name="integrate-with-microsoft-graph-notifications"></a>Microsoft Graph の通知機能を統合する

次の図に示されているように、いくつかの簡単な手順で、アプリと Microsoft Graph の通知を統合することができます。

![参加通知の手順を示す図: 登録、デバイス間のオンボーディング、サーバーの統合、およびクライアントの統合](images/notifications-integration-e2e-overview.png)

1.  アプリケーションを Microsoft Azure ポータルに[登録](notifications-integration-app-registration.md)します。

2.  クロス プラットフォームのアプリケーション ID とプッシュ通知認証情報を取得するために、パートナー センター/Windows デベロッパー センターに[参加](notifications-integration-cross-device-experiences-onboarding.md)します。

3.  Microsoft Graph を経由して通知を送信するように[アプリケーション サーバーを設定](notifications-integrating-app-server.md)します。

4.  [Microsoft Graph 通知クライアント SDK](https://github.com/microsoft/project-rome) を Windows、Android、または iOS アプリに[統合](notifications-integrating-with-windows.md)して、通知を受信および管理します。
