---
title: アプリケーション サービスから通知を作成し送信する
description: 'さまざまなクライアントにMicrosoft Graph を通じてユーザーを中心とした通知を送信するアプリケーション サービスを設定する。 '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: 1148c554b90fca5aeb56627e47a1d060f53f772e
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063350"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a>アプリケーション サービスから通知を作成し送信する

Microsoft Graph API を使用して、ユーザーに通知を作成して送信することができます。 通知は、アクティビティ フィードのストアに格納されて、ターゲット ユーザーがサインインしているすべてのデバイス上のすべてのアプリケーション クライアントに送信されます。認証方法、必要なアクセス許可の範囲、ヘッダーまたは本文の要求と予想される応答の詳細については、次を参照してください。

## <a name="authentication"></a>認証

Microsoft Graph 通知は、アプリケーション サービスがユーザーに通知を送信する On-Behalf-Of (OBO) フローを使用することを必要とします。 認証フローは、次のようにします。

1.  ユーザーが、Microsoft または職場や学校のアカウントを使用してアプリケーションにサインインします。 サインインするとき ID サービスにアクセス トークンが提供されます。

2.  アクセス トークンをアプリケーション サービスに送信します。

3.  アプリケーション サービスは ID サービスに対して認証を行い、Microsoft Graph 通知を行う OBO トークンを要求します。

4.  ID サービスには、OBO ベースのトークンと更新トークンが返されます。 アプリケーション サービスは、このアクセス トークンを使用して、このユーザーに通知を送信することができます。

OAuth 2.0 OBO フローについての詳細は、[委任ユーザー ID を使用するサービス間の呼び出し](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow)を参照してください。 Microsoft Graph 通知でこのフローが動作する方法についての詳細は、 [アプリケーション サービスのサンプル](https://aka.ms/gnsample-appservice)を参照してください。

> [!NOTE]
> Microsoft Graph 通知は、この認証をより簡略化し、アクセス トークンと更新トークンを維持する必要がない今後の計画とあわせて、OBO 認証フローを現在使用しています。

API アクセス許可と要求と応答ヘッダーの詳細については、API リファレンス セクションの [通知を作成して送信する](/graph/api/notifications-post)を参照してください。 
