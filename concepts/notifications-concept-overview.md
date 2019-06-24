---
title: 'Microsoft Graph 通知を使用して、人中心の通知エクスペリエンスを有効にする '
description: '通知は、アプリケーションのユーザーと再びやり取りするのに最も効果的な方法の 1 つです。 優れた通知エクスペリエンスによってほぼリアルタイムにアプリケーション ユーザーとのコミュニケーション チャンネルを開くことができます。これにより、適切なタイミングでアプリケーションの使用が促進され、ユーザーの生産性が向上し、重要なイベントや必要な場合タイムリー アクションが通知されます。 '
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: b83e91be74de44dbd72315331964379992b811de
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133566"
---
# <a name="enabling-human-centric-notification-experiences-using-microsoft-graph-notifications"></a><span data-ttu-id="b6e52-104">Microsoft Graph 通知を使用して、人中心の通知エクスペリエンスを有効にする</span><span class="sxs-lookup"><span data-stu-id="b6e52-104">Enabling human-centric notification experiences using Microsoft Graph notifications</span></span>

<span data-ttu-id="b6e52-105">通知は、アプリケーション ユーザーと再びやり取りするのに最も効果的な方法の 1 つです。</span><span class="sxs-lookup"><span data-stu-id="b6e52-105">Notifications are one of the most effective and direct ways to communicate to and engage with your users.</span></span> <span data-ttu-id="b6e52-106">優れた通知エクスペリエンスによってほぼリアルタイムにアプリケーション ユーザーとのコミュニケーション チャンネルを開くことができます。これにより、適切なタイミングでアプリケーションの使用が促進され、ユーザーの生産性が向上し、重要なイベントや必要なアクションが通知されます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-106">A great notification experience can help open a near real-time communication channel between you and your users, and that in turn can increase app engagement at the right time, make users more productive, and alert them to important events or required actions.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/cmpPFhrS8ZA]

<span data-ttu-id="b6e52-107">今日、ユーザーはさまざまなプラットフォームやフォーム ファクターを経由してアプリケーションやサービスにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-107">Today, users can access your applications and services via a wide variety of platforms and form factors.</span></span> <span data-ttu-id="b6e52-108">このようなデバイスの組み合わせでは、マルチプラットフォームの通知システムを理解してサポートし、ユーザーをエンドポイントにマッピングし、デバイス間で通知状態を維持する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6e52-108">This mix of devices requires that you understand and support multiplatform notification systems, map users to endpoints, and maintain notification state across devices.</span></span> 

<span data-ttu-id="b6e52-109">他のほとんどの通知システムでは、プラットフォーム固有のプッシュ通知システムを理解してターゲットにする必要はありませんが、それでも各デバイスをターゲットにするように設計されています。</span><span class="sxs-lookup"><span data-stu-id="b6e52-109">Most other notification systems eliminate the need to understand and target platform-specific push notification systems, but are still  designed to target each device.</span></span> <span data-ttu-id="b6e52-110">Microsoft Graph 通知は人中心のアプローチを提供します。これにより、あらゆるデバイス エンドポイントでユーザーをターゲットにすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-110">Microsoft Graph notifications provide a human-centric approach that gives you the ability to target your  users across any and all device endpoints.</span></span>

![複数のエンドポイントに通知を送信するために Microsoft Graph と通信するアプリ サービスを示す画像](images/notifications-flow-overview.png)

## <a name="why-integrate-with-microsoft-graph-notifications"></a><span data-ttu-id="b6e52-112">Microsoft Graph の通知機能を統合する理由</span><span class="sxs-lookup"><span data-stu-id="b6e52-112">Why integrate with Microsoft Graph notifications?</span></span>

<span data-ttu-id="b6e52-113">Microsoft Graph の通知は、アプリケーションに 4 つの主要な利点をもたらすユーザー中心の通知プラットフォームを提供します。</span><span class="sxs-lookup"><span data-stu-id="b6e52-113">Microsoft Graph notifications provide a user-centric notification platform that brings four key benefits to your applications.</span></span>

### <a name="effortlessly-target-your-user-for-notification-delivery-across-different-endpoints"></a><span data-ttu-id="b6e52-114">さまざまなエンドポイント間で通知配信ができるように、簡単にユーザーをターゲットとして設定する</span><span class="sxs-lookup"><span data-stu-id="b6e52-114">Effortlessly target your user for notification delivery across different endpoints</span></span>

<span data-ttu-id="b6e52-115">通知 API を使用して、個人の Microsoft アカウント、職場または学校の Azure Active Directory (Azure AD) アカウントをターゲットとして通知を配信できます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-115">You can use the notifications API to target a personal Microsoft account or a work or school Azure Active Directory (Azure AD) account to deliver notifications.</span></span> <span data-ttu-id="b6e52-116">この通知はプラットフォームにより、Windows UWP、Android、iOS を含む、アプリケーションまたはサービスを実行しているすべてのユーザーのエンドポイントに配信されます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-116">The platform distributes this notification to all user endpoints running your application or service, including Windows UWP, Android, and iOS.</span></span> <span data-ttu-id="b6e52-117">この機能は、適切な通知がどこにいても確実に到達できるようにすることで、アウトリーチを最大化します。</span><span class="sxs-lookup"><span data-stu-id="b6e52-117">This capability helps maximize outreach by ensuring appropriate notifications can reach your target, wherever they are.</span></span>

### <a name="easily-manage-notifications-across-endpoints"></a><span data-ttu-id="b6e52-118">エンドポイント全体にわたって通知を簡単に管理する</span><span class="sxs-lookup"><span data-stu-id="b6e52-118">Easily manage notifications across endpoints</span></span>

<span data-ttu-id="b6e52-119">クライアント アプリケーションで [Microsoft Graph 通知クライアント SDK](https://github.com/microsoft/project-rome) を使用すると、通知の状態を更新し、更新後の状態をすべてのエンドポイントで同期できます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-119">Using the [Microsoft Graph notifications client SDK](https://github.com/microsoft/project-rome) within your client application, you can update the state of a notification and sync that state across all endpoints.</span></span> <span data-ttu-id="b6e52-120">たとえば、ユーザーがあるデバイスで通知に対して操作 (開封済みまたは破棄済みとしてマークするなど) を行った場合、この状態変更が他のすべてのエンドポイントに伝播されます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-120">For example, when a user acts on a notification on one device, you can update the state of this notification (such as marking it as read or dismissed), and the same state change will be distributed to all other endpoints.</span></span> <span data-ttu-id="b6e52-121">Microsoft Graph の通知 API は、一元管理された方法でユーザーの通知の状態を追跡します。したがって簡単かつ確実に、1 回処理された通知をすべての場所で非表示にできます。これにより、冗長性を最小限に抑え、優れたカスタマー エクスペリエンスを確保します。</span><span class="sxs-lookup"><span data-stu-id="b6e52-121">The Microsoft Graph notifications API tracks the state of your users' notifications in a centralized way, making it easy for you to ensure that your notifications are handled once, and dismissed everywhere.</span></span>

### <a name="retrieve-notification-state-and-history"></a><span data-ttu-id="b6e52-122">通知状態と履歴を取得する</span><span class="sxs-lookup"><span data-stu-id="b6e52-122">Retrieve notification state and history</span></span>

<span data-ttu-id="b6e52-123">通知 API を使用して、ユーザー定義の期間 (最大 30 日間) に基づく通知履歴を取得できます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-123">You can use the notifications API to retrieve notification history based on an expiration time you define (up to 30 days).</span></span> <span data-ttu-id="b6e52-124">開封済みまたは破棄済みとしてマークされた通知でも、履歴から取得してアプリ内の通知履歴で表示でき、また分析情報とインテリジェンスを組み合わせることもできます。</span><span class="sxs-lookup"><span data-stu-id="b6e52-124">Notifications that are marked as read or dismissed are still retrievable from the history, enabling in-app views of notification history as well as enabling you to build on insights and intelligence.</span></span>

### <a name="privacy-and-compliance"></a><span data-ttu-id="b6e52-125">プライバシーとコンプライアンス</span><span class="sxs-lookup"><span data-stu-id="b6e52-125">Privacy, security, and compliance in MyAnalytics</span></span>

<span data-ttu-id="b6e52-126">Microsoft Graph 通知は、ISO 27001、ISO 27018、EUMC、HIPAA、SOC 1、SOC 2、そして GDPR など、ほとんどの企業のコンプライアンス要件を満たします。</span><span class="sxs-lookup"><span data-stu-id="b6e52-126">Microsoft Graph notifications meet most enterprise compliance requirements, including ISO 27001, ISO 27018, EUMC, HIPAA, SOC 1, SOC 2, and of course GDPR.</span></span>

## <a name="how-do-i-get-started"></a><span data-ttu-id="b6e52-127">開始するには?</span><span class="sxs-lookup"><span data-stu-id="b6e52-127">How do I get started?</span></span>

<span data-ttu-id="b6e52-128">はじめに、「[統合の概要](notifications-integration-e2e-overview.md)」セクションを参照し、アプリケーション内にユーザー中心の通知を統合する方法を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b6e52-128">To get started, see the [integration overview](notifications-integration-e2e-overview.md) section to learn how you can integrate user-centric notifications within your application.</span></span>
