---
title: アプリケーション サービスから通知を作成し送信する
description: 'さまざまなクライアントにMicrosoft Graph を通じてユーザーを中心とした通知を送信するアプリケーション サービスを設定する。 '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: cf40087aff3956a88f79197482db8126bbe8d96c
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683511"
---
# <a name="create-and-send-a-notification-from-your-app-service"></a><span data-ttu-id="235dd-103">アプリケーション サービスから通知を作成し送信する</span><span class="sxs-lookup"><span data-stu-id="235dd-103">Create and send a notification from your app service</span></span>

<span data-ttu-id="235dd-104">Microsoft Graph API を使用して、ユーザーに通知を作成して送信することができます。</span><span class="sxs-lookup"><span data-stu-id="235dd-104">You can create and send a notification to a user by using Microsoft Graph APIs.</span></span> <span data-ttu-id="235dd-105">通知はアクティビティ フィード ストアに格納され、ターゲット ユーザーがサインインしているすべてのデバイスのすべてのアプリ クライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="235dd-105">The notification is stored in the activity feed store and is sent to all app clients on all devices that the target user is signed in on.</span></span> 

## <a name="authentication"></a><span data-ttu-id="235dd-106">認証</span><span class="sxs-lookup"><span data-stu-id="235dd-106">Authentication</span></span>

<span data-ttu-id="235dd-107">Microsoft Graph 通知は、アプリケーション サービスがユーザーに通知を送信する On-Behalf-Of (OBO) フローを使用することを必要とします。</span><span class="sxs-lookup"><span data-stu-id="235dd-107">Microsoft Graph notifications requires that your application service uses the On-Behalf-Of (OBO) flow to post a notification to a user.</span></span> <span data-ttu-id="235dd-108">認証フローは、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="235dd-108">The following is a simple and typical authentication flow:</span></span>

1.  <span data-ttu-id="235dd-109">ユーザーが、Microsoft または職場や学校のアカウントを使用してアプリケーションにサインインします。</span><span class="sxs-lookup"><span data-stu-id="235dd-109">The user signs in to your application with their Microsoft or their work or school account.</span></span> <span data-ttu-id="235dd-110">サインインするとき ID サービスにアクセス トークンが提供されます。</span><span class="sxs-lookup"><span data-stu-id="235dd-110">When they sign in, the identity service gives you an access token.</span></span>

2.  <span data-ttu-id="235dd-111">アクセス トークンをアプリケーション サービスに送信します。</span><span class="sxs-lookup"><span data-stu-id="235dd-111">You send the access token to your app service.</span></span>

3.  <span data-ttu-id="235dd-112">アプリケーション サービスは ID サービスに対して認証を行い、Microsoft Graph 通知を行う OBO トークンを要求します。</span><span class="sxs-lookup"><span data-stu-id="235dd-112">You app service authenticates against the identity service and requests an OBO token for Microsoft Graph notifications.</span></span>

4.  <span data-ttu-id="235dd-113">ID サービスには、OBO ベースのトークンと更新トークンが返されます。</span><span class="sxs-lookup"><span data-stu-id="235dd-113">The identity service returns an OBO-based token and a refresh token.</span></span> <span data-ttu-id="235dd-114">アプリケーション サービスは、このアクセス トークンを使用して、このユーザーに通知を送信することができます。</span><span class="sxs-lookup"><span data-stu-id="235dd-114">Your app service can use this access token to post notifications to this user.</span></span>

<span data-ttu-id="235dd-115">OAuth 2.0 OBO フローについての詳細は、[委任ユーザー ID を使用するサービス間の呼び出し](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="235dd-115">To learn more about OAuth 2.0 OBO flow, see [Service-to-service calls that use delegated user identity in the On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-oauth2-on-behalf-of-flow).</span></span> <span data-ttu-id="235dd-116">Microsoft Graph 通知でこのフローが動作する方法についての詳細は、 [アプリケーション サービスのサンプル](https://aka.ms/gnsample-appservice)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="235dd-116">For details about how this flow works with Microsoft Graph notifications, see the [App Service sample](https://aka.ms/gnsample-appservice).</span></span>

> [!NOTE]
> <span data-ttu-id="235dd-117">Microsoft Graph 通知は、この認証をより簡略化し、アクセス トークンと更新トークンを維持する必要がない今後の計画とあわせて、OBO 認証フローを現在使用しています。</span><span class="sxs-lookup"><span data-stu-id="235dd-117">Microsoft Graph notifications currently uses OBO authentication flow with future plans to simplify this authentication further and eliminate the need to maintain access tokens and refresh tokens.</span></span>

<span data-ttu-id="235dd-118">API アクセス許可と要求と応答ヘッダーの詳細については、API リファレンス セクションの [通知を作成して送信する](/graph/api/notifications-post)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="235dd-118">For more details on the API permissions and on the request and response headers, please see [Create and send a notification](/graph/api/notifications-post) in the API reference section.</span></span> 
