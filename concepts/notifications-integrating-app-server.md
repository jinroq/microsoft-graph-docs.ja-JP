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
# <a name="create-and-send-a-notification-from-your-app-service"></a><span data-ttu-id="e5bae-103">アプリケーション サービスから通知を作成し送信する</span><span class="sxs-lookup"><span data-stu-id="e5bae-103">Create and send a notification from your app service</span></span>

<span data-ttu-id="e5bae-104">Microsoft Graph API を使用して、ユーザーに通知を作成して送信することができます。</span><span class="sxs-lookup"><span data-stu-id="e5bae-104">You can create and send a notification to a user by using Microsoft Graph APIs.</span></span> <span data-ttu-id="e5bae-105">通知は、アクティビティ フィードのストアに格納されて、ターゲット ユーザーがサインインしているすべてのデバイス上のすべてのアプリケーション クライアントに送信されます。認証方法、必要なアクセス許可の範囲、ヘッダーまたは本文の要求と予想される応答の詳細については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5bae-105">The notification is stored in the activity feed store and is sent to all app clients on all devices that the target user is signed in on.See below to learn how to authenticate, required permission scopes, request header/body and expected response.</span></span>

## <a name="authentication"></a><span data-ttu-id="e5bae-106">認証</span><span class="sxs-lookup"><span data-stu-id="e5bae-106">Authentication</span></span>

<span data-ttu-id="e5bae-107">Microsoft Graph 通知は、アプリケーション サービスがユーザーに通知を送信する On-Behalf-Of (OBO) フローを使用することを必要とします。</span><span class="sxs-lookup"><span data-stu-id="e5bae-107">Microsoft Graph notifications requires that your application service uses the On-Behalf-Of (OBO) flow to post a notification to a user.</span></span> <span data-ttu-id="e5bae-108">認証フローは、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="e5bae-108">The following is a simple and typical authentication flow:</span></span>

1.  <span data-ttu-id="e5bae-109">ユーザーが、Microsoft または職場や学校のアカウントを使用してアプリケーションにサインインします。</span><span class="sxs-lookup"><span data-stu-id="e5bae-109">The user signs in to your application with their Microsoft or their work or school account.</span></span> <span data-ttu-id="e5bae-110">サインインするとき ID サービスにアクセス トークンが提供されます。</span><span class="sxs-lookup"><span data-stu-id="e5bae-110">When they sign in, the identity service gives you an access token.</span></span>

2.  <span data-ttu-id="e5bae-111">アクセス トークンをアプリケーション サービスに送信します。</span><span class="sxs-lookup"><span data-stu-id="e5bae-111">You send the access token to your app service.</span></span>

3.  <span data-ttu-id="e5bae-112">アプリケーション サービスは ID サービスに対して認証を行い、Microsoft Graph 通知を行う OBO トークンを要求します。</span><span class="sxs-lookup"><span data-stu-id="e5bae-112">You app service authenticates against the identity service and requests an OBO token for Microsoft Graph notifications.</span></span>

4.  <span data-ttu-id="e5bae-113">ID サービスには、OBO ベースのトークンと更新トークンが返されます。</span><span class="sxs-lookup"><span data-stu-id="e5bae-113">The identity service returns an OBO-based token and a refresh token.</span></span> <span data-ttu-id="e5bae-114">アプリケーション サービスは、このアクセス トークンを使用して、このユーザーに通知を送信することができます。</span><span class="sxs-lookup"><span data-stu-id="e5bae-114">Your app service can use this access token to post notifications to this user.</span></span>

<span data-ttu-id="e5bae-115">OAuth 2.0 OBO フローについての詳細は、[委任ユーザー ID を使用するサービス間の呼び出し](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5bae-115">To learn more about OAuth 2.0 OBO flow, see [Service-to-service calls that use delegated user identity in the On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow).</span></span> <span data-ttu-id="e5bae-116">Microsoft Graph 通知でこのフローが動作する方法についての詳細は、 [アプリケーション サービスのサンプル](https://aka.ms/gnsample-appservice)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5bae-116">For details about how this flow works with Microsoft Graph notifications, see the [App Service sample](https://aka.ms/gnsample-appservice).</span></span>

> [!NOTE]
> <span data-ttu-id="e5bae-117">Microsoft Graph 通知は、この認証をより簡略化し、アクセス トークンと更新トークンを維持する必要がない今後の計画とあわせて、OBO 認証フローを現在使用しています。</span><span class="sxs-lookup"><span data-stu-id="e5bae-117">Microsoft Graph notifications currently uses OBO authentication flow with future plans to simplify this authentication further and eliminate the need to maintain access tokens and refresh tokens.</span></span>

<span data-ttu-id="e5bae-118">API アクセス許可と要求と応答ヘッダーの詳細については、API リファレンス セクションの [通知を作成して送信する](/graph/api/notifications-post)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5bae-118">For more details on the API permissions and on the request and response headers, please see [Create and send a notification](/graph/api/notifications-post) in API reference section.</span></span> 
